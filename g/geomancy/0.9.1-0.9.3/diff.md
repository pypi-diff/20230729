# Comparing `tmp/geomancy-0.9.1.tar.gz` & `tmp/geomancy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-0.9.1.tar", last modified: Wed Jul 26 14:44:17 2023, max compression
+gzip compressed data, was "geomancy-0.9.3.tar", last modified: Sat Jul 29 16:59:32 2023, max compression
```

## Comparing `geomancy-0.9.1.tar` & `geomancy-0.9.3.tar`

### file list

```diff
@@ -1,74 +1,86 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.303730 geomancy-0.9.1/
--rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-26 14:41:25.000000 geomancy-0.9.1/.editorconfig
--rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.9.1/.gitignore
--rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.9.1/.readthedocs.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1023 2023-07-26 00:50:48.000000 geomancy-0.9.1/LICENSE
--rw-r--r--   0 jlorieau   (501) staff       (20)     5792 2023-07-26 14:44:17.303147 geomancy-0.9.1/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     4612 2023-07-26 14:41:25.000000 geomancy-0.9.1/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     1711 2023-07-26 14:41:25.000000 geomancy-0.9.1/Taskfile.yaml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.279383 geomancy-0.9.1/changelog/
--rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.9.1/changelog/changelog_template.jinja
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.281240 geomancy-0.9.1/docs/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.282444 geomancy-0.9.1/docs/_static/
--rw-r--r--   0 jlorieau   (501) staff       (20)      466 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/_static/custom.css
--rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.9.1/docs/_static/geomancy_logo.png
--rw-r--r--   0 jlorieau   (501) staff       (20)     1858 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/_static/geomancy_logo.svg
--rw-r--r--   0 jlorieau   (501) staff       (20)     1281 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/changelog.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     2120 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/conf.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      563 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/index.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.9.1/docs/quickstart.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.282744 geomancy-0.9.1/docs/usage/
--rw-r--r--   0 jlorieau   (501) staff       (20)     9995 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/usage/index.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.284199 geomancy-0.9.1/examples/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1485 2023-07-24 19:24:24.000000 geomancy-0.9.1/examples/geomancy.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1280 2023-07-26 14:41:25.000000 geomancy-0.9.1/examples/geomancy.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)      272 2023-07-26 14:41:25.000000 geomancy-0.9.1/examples/geomancy_flat.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.9.1/examples/pyproject.toml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.285208 geomancy-0.9.1/geomancy/
--rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.9.1/geomancy/__description__.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-26 14:43:56.000000 geomancy-0.9.1/geomancy/__init__.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.291693 geomancy-0.9.1/geomancy/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.9.1/geomancy/checks/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    11675 2023-07-24 19:29:23.000000 geomancy-0.9.1/geomancy/checks/base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-24 18:15:32.000000 geomancy-0.9.1/geomancy/checks/env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.9.1/geomancy/checks/exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.9.1/geomancy/checks/path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2912 2023-07-24 15:55:58.000000 geomancy-0.9.1/geomancy/checks/python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     5888 2023-07-24 20:38:18.000000 geomancy-0.9.1/geomancy/checks/utils.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2336 2023-07-24 15:55:27.000000 geomancy-0.9.1/geomancy/checks/version.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.293198 geomancy-0.9.1/geomancy/cli/
--rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.9.1/geomancy/cli/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.9.1/geomancy/cli/term.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.294801 geomancy-0.9.1/geomancy/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.9.1/geomancy/config/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9901 2023-07-26 14:41:25.000000 geomancy-0.9.1/geomancy/config/config.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.296296 geomancy-0.9.1/geomancy/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-25 01:07:06.000000 geomancy-0.9.1/geomancy/environment/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     4140 2023-07-25 01:16:29.000000 geomancy-0.9.1/geomancy/environment/load_environment.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     6683 2023-07-26 14:41:25.000000 geomancy-0.9.1/geomancy/main.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.287484 geomancy-0.9.1/geomancy.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     5792 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     1340 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      136 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/top_level.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)     2793 2023-07-26 14:41:25.000000 geomancy-0.9.1/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-26 14:44:17.303868 geomancy-0.9.1/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.297353 geomancy-0.9.1/tests/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.300348 geomancy-0.9.1/tests/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)     2955 2023-07-24 19:21:58.000000 geomancy-0.9.1/tests/checks/test_base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.9.1/tests/checks/test_env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1461 2023-07-24 15:35:23.000000 geomancy-0.9.1/tests/checks/test_exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.9.1/tests/checks/test_path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2442 2023-07-24 15:31:44.000000 geomancy-0.9.1/tests/checks/test_python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.9.1/tests/checks/test_utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.301264 geomancy-0.9.1/tests/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.9.1/tests/config/config1.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.9.1/tests/config/test_config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.9.1/tests/conftest.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.301708 geomancy-0.9.1/tests/data/
--rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.9.1/tests/data/test.env
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.302170 geomancy-0.9.1/tests/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)     3181 2023-07-25 04:09:51.000000 geomancy-0.9.1/tests/environment/test_load_environment.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2802 2023-07-26 14:41:25.000000 geomancy-0.9.1/tests/test_main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.052968 geomancy-0.9.3/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-26 14:41:25.000000 geomancy-0.9.3/.editorconfig
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.026954 geomancy-0.9.3/.github/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.033491 geomancy-0.9.3/.github/workflows/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      760 2023-07-29 16:55:41.000000 geomancy-0.9.3/.github/workflows/tests.yml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.9.3/.gitignore
+-rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.9.3/.readthedocs.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1023 2023-07-26 00:50:48.000000 geomancy-0.9.3/LICENSE
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6029 2023-07-29 16:59:32.052605 geomancy-0.9.3/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4849 2023-07-29 16:55:41.000000 geomancy-0.9.3/README.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1711 2023-07-26 14:41:25.000000 geomancy-0.9.3/Taskfile.yaml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.033913 geomancy-0.9.3/changelog/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.9.3/changelog/changelog_template.jinja
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.035364 geomancy-0.9.3/docs/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.036396 geomancy-0.9.3/docs/_static/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      466 2023-07-26 14:41:25.000000 geomancy-0.9.3/docs/_static/custom.css
+-rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.9.3/docs/_static/geomancy_logo.png
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6346 2023-07-28 19:38:01.000000 geomancy-0.9.3/docs/_static/geomancy_logo.svg
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3205 2023-07-29 16:57:58.000000 geomancy-0.9.3/docs/changelog.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2121 2023-07-29 16:55:41.000000 geomancy-0.9.3/docs/conf.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      651 2023-07-28 19:38:01.000000 geomancy-0.9.3/docs/index.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.9.3/docs/quickstart.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.037336 geomancy-0.9.3/docs/usage/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     8813 2023-07-29 16:55:41.000000 geomancy-0.9.3/docs/usage/cmd_checks.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1437 2023-07-28 19:38:01.000000 geomancy-0.9.3/docs/usage/cmd_run.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)    11313 2023-07-29 16:55:41.000000 geomancy-0.9.3/docs/usage/format.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.038435 geomancy-0.9.3/examples/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1483 2023-07-29 16:55:41.000000 geomancy-0.9.3/examples/geomancy.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1278 2023-07-29 16:55:41.000000 geomancy-0.9.3/examples/geomancy.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      272 2023-07-26 14:41:25.000000 geomancy-0.9.3/examples/geomancy_flat.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      510 2023-07-29 16:55:41.000000 geomancy-0.9.3/examples/pyproject.toml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.039006 geomancy-0.9.3/geomancy/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.9.3/geomancy/__description__.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-29 16:59:23.000000 geomancy-0.9.3/geomancy/__init__.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.044252 geomancy-0.9.3/geomancy/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.9.3/geomancy/checks/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    11987 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/checks/base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1696 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/checks/env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.9.3/geomancy/checks/exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.9.3/geomancy/checks/path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3422 2023-07-29 02:10:42.000000 geomancy-0.9.3/geomancy/checks/python.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5242 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/checks/utils.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2336 2023-07-24 15:55:27.000000 geomancy-0.9.3/geomancy/checks/version.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.044912 geomancy-0.9.3/geomancy/cli/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-27 16:55:31.000000 geomancy-0.9.3/geomancy/cli/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6640 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/cli/term.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.045648 geomancy-0.9.3/geomancy/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.9.3/geomancy/config/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    13410 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/config/config.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.047940 geomancy-0.9.3/geomancy/entrypoints/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3423 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/entrypoints/check.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      546 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4136 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/environment.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1427 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/geo.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      487 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/run.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      904 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.048606 geomancy-0.9.3/geomancy/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/environment/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     8587 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/environment/dotenv.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.041086 geomancy-0.9.3/geomancy.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6029 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1579 2023-07-29 16:59:32.000000 geomancy-0.9.3/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       53 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      167 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2836 2023-07-28 19:38:01.000000 geomancy-0.9.3/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-29 16:59:32.053070 geomancy-0.9.3/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.048886 geomancy-0.9.3/tests/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.050343 geomancy-0.9.3/tests/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5181 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/checks/test_base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2690 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/checks/test_env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1074 2023-07-29 02:10:42.000000 geomancy-0.9.3/tests/checks/test_exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2193 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/checks/test_path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2442 2023-07-24 15:31:44.000000 geomancy-0.9.3/tests/checks/test_python.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.050960 geomancy-0.9.3/tests/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.9.3/tests/config/config1.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     7826 2023-07-28 19:38:01.000000 geomancy-0.9.3/tests/config/test_config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.9.3/tests/conftest.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.051367 geomancy-0.9.3/tests/data/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.9.3/tests/data/test.env
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.051640 geomancy-0.9.3/tests/entrypoints/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4417 2023-07-28 19:38:01.000000 geomancy-0.9.3/tests/entrypoints/test_geo.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.051905 geomancy-0.9.3/tests/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6043 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/environment/test_dotenv.py
```

### Comparing `geomancy-0.9.1/.gitignore` & `geomancy-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/LICENSE` & `geomancy-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/PKG-INFO` & `geomancy-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.9.1
+Version: 0.9.3
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -55,15 +55,15 @@
     ```yaml
     checks:
       Environment:
         desc: Check environment variables common to all development environments
 
         Username:
           desc: The current username
-          checkEnv: "{USER}"
+          checkEnv: "$USER"
           regex: "[a-z_][a-z0-9_-]*[$]?"
 
       Paths:
         desc: Checks the existence of needed files and directories
         subchecks: any  # at least one of the files must be present
 
           Geomancy:
@@ -86,49 +86,56 @@
 2. Use ``geo`` to run the checks.
 
     ```shell
     $ geo
     =============================== .geomancy.toml ================================
         checks (9 checks)
     [✔]   Environment (1 checks)
-    [✔]     Check environment variable '{USER}'...passed
+    [✔]     Check environment variable '$USER'...passed
     [✔]   Paths (2 checks)
     [✔]     Check path 'examples/geomancy.toml'...passed
     [✔]     Check path 'examples/pyproject.toml'...passed
     [✔]   Executables (1 checks)
     [✔]     Check executable 'python3>=3.11'...passed
     ========================== PASSED.  8 checks in 0.01s =========================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 ## Features
 <!-- start features -->
-``geomancy`` can:
+Geomancy checks include:
 
-- __Environment variables__. Check environment variables are properly set and,
-  optionally, check that they have valid values
+- __Environment variables__ are properly set and, optionally,
+  check that they have valid values with regular expressions
   ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
-- __Paths__. Check file and directory path existence
+- __Paths__ exist and whether they're files or directories
   ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
-- __Executables__. Check executables are available and, optionally, have the
-  minimum or correct versions
+- __Executables__ are available and, optionally, have the minimum or correct
+  versions
   ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
-- __Python Packages__. Check python packages are available and, optionally,
-  have the minimum or correct versions
+- __Python packages__ are available and, optionally, have the minimum or
+  correct versions
   ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
-- __Group Checks__. Nested group checks with conditional (all or any) pass
+- __Group checks__ to nested groups of checks with conditional (all or any) pass
   criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
-- __Environment Substitution__. Substitute parameter values from environment
-  variables. ex: ``checkPath: {HOME}/.geomancy.toml``
-- __Multiple Formats__. Checks files can be in yaml (e.g. ``.geomancy.yaml``)
-  or in [toml](https://toml.io/en/) (e.g. ``.geomancy.toml`` or
-  ``pyproject.toml``)
+
+Additionally, geomancy can:
+
+- __Load environment files__ for
+  [checks](https://geomancy.readthedocs.io/en/latest/usage/cmd_checks.html#environment-files)
+  or for [running](https://geomancy.readthedocs.io/en/latest/usage/cmd_run.html#running-environments)
+  shell commands
+- __Substitute environment variables__ in check values e.g.:
+  ``checkPath: {HOME}/.geomancy.toml``
+- __Load checks in multiple formats__ including [yaml](https://yaml.org)
+  (e.g. ``.geomancy.yaml``) or in [toml](https://toml.io/en/)
+  (e.g. ``.geomancy.toml`` or ``pyproject.toml``)
 <!-- end features -->
 
 ## Documentation
 
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
```

### Comparing `geomancy-0.9.1/README.md` & `geomancy-0.9.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     ```yaml
     checks:
       Environment:
         desc: Check environment variables common to all development environments
 
         Username:
           desc: The current username
-          checkEnv: "{USER}"
+          checkEnv: "$USER"
           regex: "[a-z_][a-z0-9_-]*[$]?"
 
       Paths:
         desc: Checks the existence of needed files and directories
         subchecks: any  # at least one of the files must be present
 
           Geomancy:
@@ -57,49 +57,56 @@
 2. Use ``geo`` to run the checks.
 
     ```shell
     $ geo
     =============================== .geomancy.toml ================================
         checks (9 checks)
     [✔]   Environment (1 checks)
-    [✔]     Check environment variable '{USER}'...passed
+    [✔]     Check environment variable '$USER'...passed
     [✔]   Paths (2 checks)
     [✔]     Check path 'examples/geomancy.toml'...passed
     [✔]     Check path 'examples/pyproject.toml'...passed
     [✔]   Executables (1 checks)
     [✔]     Check executable 'python3>=3.11'...passed
     ========================== PASSED.  8 checks in 0.01s =========================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 ## Features
 <!-- start features -->
-``geomancy`` can:
+Geomancy checks include:
 
-- __Environment variables__. Check environment variables are properly set and,
-  optionally, check that they have valid values
+- __Environment variables__ are properly set and, optionally,
+  check that they have valid values with regular expressions
   ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
-- __Paths__. Check file and directory path existence
+- __Paths__ exist and whether they're files or directories
   ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
-- __Executables__. Check executables are available and, optionally, have the
-  minimum or correct versions
+- __Executables__ are available and, optionally, have the minimum or correct
+  versions
   ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
-- __Python Packages__. Check python packages are available and, optionally,
-  have the minimum or correct versions
+- __Python packages__ are available and, optionally, have the minimum or
+  correct versions
   ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
-- __Group Checks__. Nested group checks with conditional (all or any) pass
+- __Group checks__ to nested groups of checks with conditional (all or any) pass
   criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
-- __Environment Substitution__. Substitute parameter values from environment
-  variables. ex: ``checkPath: {HOME}/.geomancy.toml``
-- __Multiple Formats__. Checks files can be in yaml (e.g. ``.geomancy.yaml``)
-  or in [toml](https://toml.io/en/) (e.g. ``.geomancy.toml`` or
-  ``pyproject.toml``)
+
+Additionally, geomancy can:
+
+- __Load environment files__ for
+  [checks](https://geomancy.readthedocs.io/en/latest/usage/cmd_checks.html#environment-files)
+  or for [running](https://geomancy.readthedocs.io/en/latest/usage/cmd_run.html#running-environments)
+  shell commands
+- __Substitute environment variables__ in check values e.g.:
+  ``checkPath: {HOME}/.geomancy.toml``
+- __Load checks in multiple formats__ including [yaml](https://yaml.org)
+  (e.g. ``.geomancy.yaml``) or in [toml](https://toml.io/en/)
+  (e.g. ``.geomancy.toml`` or ``pyproject.toml``)
 <!-- end features -->
 
 ## Documentation
 
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
```

### Comparing `geomancy-0.9.1/Taskfile.yaml` & `geomancy-0.9.3/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/docs/_static/geomancy_logo.png` & `geomancy-0.9.3/docs/_static/geomancy_logo.png`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/docs/conf.py` & `geomancy-0.9.3/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,15 @@
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- MyST options ------------------------------------------------------------
-myst_enable_extensions = [
-    "colon_fence",
-    "deflist",
-    "fieldlist",
-]
+myst_enable_extensions = ["colon_fence", "deflist", "fieldlist", "substitution"]
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_book_theme"
```

### Comparing `geomancy-0.9.1/docs/index.md` & `geomancy-0.9.3/docs/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,23 @@
 :end-before: <!-- end features -->
 ```
 
 ```{toctree}
 :hidden:
 
 quickstart
-usage/index
+```
+```{toctree}
+:hidden:
+:caption: Usage
+:maxdepth: 1
+
+usage/cmd_checks
+usage/cmd_run
+usage/format
 ```
 ```{toctree}
 :hidden:
 :caption: About the Project
 :maxdepth: 1
 
 changelog
```

### Comparing `geomancy-0.9.1/docs/usage/index.md` & `geomancy-0.9.3/docs/usage/format.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,63 @@
-# Usage
+---
+myst:
+  substitutions:
+    check_base_args: |
+      `desc`: str (Optional)
+      : The description for the check
+
+      `substitute`: bool (Optional)
+      : Whether to [substitute](#environment-substitution) environment variables in
+        check values<br>
+        __default__: True<br>
+        __aliases__: ``substitute``, ``env_substitute``
+---
+(file-format)=
+# Checks Files
 
-## Format
-
-The checks file is formatted in [YAML](https://yaml.org) or [TOML](https://toml.io/en/),
+The checks file is formatted in [yaml](https://yaml.org) or [toml](https://toml.io/en/),
 and it contains a listing of checks and, optionally, configuration options
 for ``geomancy``.
 
-### Filenames
+## Filenames
 
 The checks file may be a dedicated file for ``geomancy``, such as a
 ``.geomancy.yaml`` or ``.geomancy.toml`` file in the project root
 directory, or it may be incorporated as part of a ``pyproject.toml`` file
 under the ``[tool.geomancy]`` section.
 
 ::::{tab-set}
 :::{tab-item} geomancy.yaml
 ```yaml
 checks:
   Username:
     desc: The current username
-    checkEnv: "{USER}"
+    checkEnv: "$USER"
     regex: "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
 :::{tab-item} geomancy.toml
 ```toml
 [checks.Username]
 desc = "The current username"
-checkEnv = "{USER}"
+checkEnv = "$USER"
 regex = "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
 :::{tab-item} pyproject.toml
 ```toml
 [tool.geomancy.checks.Username]
 desc = "The current username"
-checkEnv = "{USER}"
+checkEnv = "$USER"
 regex = "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
 ::::
 
-### Nesting and Listing Checks
+## Nesting and Listing Checks
 
 Checks can be grouped into sections of related checks, and the pass condition
 for child checks can be customized.
 
 ::::{tab-set}
 :::{tab-item} geomancy.yaml
 By default, all child checks must pass for the parent check to pass.
@@ -125,17 +137,18 @@
 checkPath = "examples/geomancy.yaml"
 type = "file"
 ```
 
 :::
 ::::
 
-### Configuration
+## Configuration
 
-Checks files may optionally include configuration settings for ``geomancy``.
+Checks files may optionally include configuration settings for geomancy. The
+[config](#configuration) lists the current default configuration.
 
 ::::{tab-set}
 :::{tab-item} geomancy.yaml
 Configuration settings are specified the ``config`` section.
 ```yaml
 config:
   CHECKBASE:
@@ -156,52 +169,59 @@
 [tool.geomancy.config]
 [tool.geomancy.config.CHECKBASE]
 ENV_SUBSTITUTE_DEFAULT = true
 ```
 :::
 ::::
 
-:::{tip}
-All configuration options and their defaults can be listed in
-[TOML](https://toml.io/en/) format using the ``geo --config`` command.
-:::
-
 ## Checks
 
 The following describes the various checks and their options.
 
+:::{versionchanged} 0.9.3
+Environment variables are now referenced by the name preceded by a ``$`` and
+optional braces. e.g. ``$USER`` or ``${USER}``
+:::
+
 ### checkEnv
 
 Check the existence and, optionally, the value of an environment variable.
 
-:checkEnv: Environment variable to check, wrapped in curly braces for
-substitution. <br>
-__aliases__: ``checkEnv``, ``CheckEnv``
-:desc: _(Optional)_ The description for the check
-:regex: _(Optional)_ A regular expression to check against the environment
-variable value
+:::{card}
+Parameters
+^^^
+`checkEnv`: str
+: Environment variable to check, wrapped in curly braces for substitution. <br>
+  __aliases__: ``checkEnv``, ``CheckEnv``
+
+{{check_base_args}}
+
+`regex`: str (Optional)
+: A regular expression to check against the environment variable
+  value
+:::
 
 ::::{tab-set}
 :::{tab-item} Example 1 (yaml)
 The ``checkEnv`` check in YAML format.
 ```yaml
 checks:
   Environment:
     Username:
       desc: The current username
-      checkEnv: "{USER}"
+      checkEnv: "$USER"
       regex: "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
 :::{tab-item} Example 2 (toml)
 The ``checkEnv`` check in TOML format.
 ```toml
 [checks.Environment.Username]
 desc = "The current username"
-checkEnv = "{USER}"
+checkEnv = "$USER"
 regex = "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
 :::{tab-item} Example 3 (toml)
 The ``checkEnv`` check in abbreviated TOML format.
 ```toml
 [checks.Environment]
@@ -211,18 +231,24 @@
 ::::
 
 ### checkExec
 
 Check the existence and, optionally, the version of available executables or
 commands.
 
-:checkExec: Executable to check. Additionally, an optional version check
-can be added with a test operator. <br>
-__aliases__: ``checkExec``, ``CheckExec``
-:desc: _(Optional)_ The description for the check
+:::{card}
+Parameters
+^^^
+`checkExec`: str
+: Executable to check. Additionally, an optional version check can be added
+  with a test operator. <br>
+  __aliases__: ``checkExec``, ``CheckExec``
+
+{{check_base_args}}
+:::
 
 ::::{tab-set}
 :::{tab-item} Example 1 (yaml)
 The ``checkExec`` check in YAML format.
 ```yaml
 checks:
   Ls:
@@ -254,22 +280,29 @@
 Python = { checkExec = "python3>=3.11" }
 ```
 :::
 ::::
 
 ### checkPath
 
-Check the existence and, optionally, the type of a path.
+Check the existence and, optionally, the type of path.
 
-:checkPath: Path to check, which may include environment variables wrapped
-in curly braces for substitution. <br>
-__aliases__: ``checkPath``, ``CheckPath``
-:desc: _(Optional)_ The description for the check
-:type: _(Optional)_ Additionally check whether the path corresponds to a
-valid ``'file'`` or ``'dir'``.
+:::{card}
+Parameters
+^^^
+`checkPath`: str
+: Path to check, which may include environment variables for substitution. <br>
+  __aliases__: ``checkPath``, ``CheckPath``
+
+{{check_base_args}}
+
+`type`: str (Optional)
+: Additionally check whether the path corresponds to a valid ``'file'`` or
+  ``'dir'``.
+:::
 
 ::::{tab-set}
 :::{tab-item} Example 1 (yaml)
 The ``checkPath`` check in YAML format.
 ```yaml
 checks:
   Pyproject:
@@ -297,19 +330,25 @@
 ::::
 
 ### checkPythonPkg
 
 Checks whether the python package is installed and, optionally, check its
 version.
 
-:checkPythonPkg: Python package to check. Additionally, an optional version
-check can be added with a test operator. <br>
-__aliases__: ``checkPythonPkg``, ``CheckPythonPkg``,
-``checkPythonPackage``, ``CheckPythonPackage``
-:desc: _(Optional)_ The description for the check
+:::{card}
+Parameters
+^^^
+`checkPythonPkg`: str
+: Python package to check. Additionally, an optional version check can be added
+  with a test operator. <br>
+  __aliases__: ``checkPythonPkg``, ``CheckPythonPkg``, ``checkPythonPackage``,
+  ``CheckPythonPackage``
+
+{{check_base_args}}
+:::
 
 ::::{tab-set}
 :::{tab-item} Example 1 (yaml)
 The ``checkPythonPkg`` check in YAML format.
 ```yaml
 checks:
   PythonPackages:
@@ -335,27 +374,36 @@
 :::
 ::::
 
 ### Check Groups
 
 Check groups are sections which contain one or more child checks.
 
-:desc: _(Optional)_ The description for the check section
-:subchecks: _(Optional)_ Either ``'all'`` to require that all sub-checks
-pass or ``'any'`` to require that only one sub-check passes.<br>
-Default: ``'all'``<br>
-__aliases__: ``condition``
+:::{card}
+Parameters
+^^^
+`desc`: str (Optional)
+: The description for the check group
+
+`subchecks`: str (Optional)
+: The pass condition for the sub-checks of the group. Can be either ``'all'``
+  to require that all sub-checks pass or ``'any'`` to require that only one
+  sub-check passes.<br>
+  __default__: ``'all'``<br>
+  __aliases__: ``condition``
+:::
 
 ::::{tab-set}
 :::{tab-item} Example 1 (yaml)
 The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
 ``Pyproject``.
 ```yaml
 checksFiles:
   desc: Checks that at least one checks file exists
+  subchecks: any
 
   Geomancy:
     desc: Check for the 'geomancy.toml' file
     checkPath: examples/geomancy.toml
     type: file
   Pyproject:
     desc: Check for 'pyproject.toml' file
@@ -390,7 +438,47 @@
 subchecks = "any"
 
 Geomancy = { checkPath = "examples/geomancy.toml", type = "file" }
 Pyproject = { checkPath = "examples/pyproject.toml", type = "file" }
 ```
 :::
 ::::
+
+
+## Tips and Tricks
+
+### Unwanted environment substitution
+
+Environment variables are substituted by default in the values passed to
+checks. This can be avoided by setting ``substitute`` to False or by
+using a literal with single quotes.
+
+::::{tab-set}
+:::{tab-item} Substitute (yaml)
+```yaml
+MyOddFilename:
+  checkPath: myfile$.txt
+  substitution: False
+```
+:::
+:::{tab-item} Literal string (yaml)
+Use triple (3) single quotes
+```yaml
+MyOddFilename:
+  checkPath: '''myfile$.txt'''
+```
+:::
+:::{tab-item} Substitute (toml)
+```yaml
+[MyOddFilename]
+checkpath='myfile$.txt'
+substitution=false
+```
+:::
+:::{tab-item} Literal string (toml)
+Use triple (4) single quotes
+```yaml
+[MyOddFilename]
+checkpath=''''myfile$.txt''''
+```
+:::
+::::
```

### Comparing `geomancy-0.9.1/examples/geomancy.toml` & `geomancy-0.9.3/examples/geomancy.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   ENV_SUBSTITUTE_DEFAULT=true
 
 [checks.Environment]
 desc = "Check environment variables common to all development environments"
 
     [checks.Environment.Path]
     desc = "Paths to search for executables"
-    checkEnv = "{PATH}"
+    checkEnv = "$PATH"
 
     [checks.Environment.Username]
     desc = "The current username"
-    checkEnv = "{USER}"
+    checkEnv = "$USER"
     regex = "[a-z_][a-z0-9_-]*[$]?"
 
 [checks.Paths]
 desc = "Checks the existence of needed files and directories"
 
     [checks.Paths.ChecksFile]
     desc = "Checks that at least one checks file exists"
```

### Comparing `geomancy-0.9.1/examples/geomancy.yaml` & `geomancy-0.9.3/examples/geomancy.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # Nested changes
 checks:
   Environment:
     desc: Check environment variables common to all development environments
 
     Path:
       decs: Paths to search for executables
-      checkEnv: "{PATH}"
+      checkEnv: "$PATH"
     Username:
       desc: The current username
-      checkEnv: "{USER}"
+      checkEnv: "$USER"
       regex: "[a-z_][a-z0-9_-]*[$]?"
 
   Paths:
     desc: Checks the existence of needed files and directories
 
     ChecksFile:
       desc: Checks that at least one checks file exists
```

### Comparing `geomancy-0.9.1/geomancy/checks/base.py` & `geomancy-0.9.3/geomancy/checks/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,38 @@
 """
 import typing as t
 from abc import ABC
 from inspect import isabstract
 from collections import namedtuple
 from time import process_time
 
-from .utils import sub_env, all_subclasses, pop_first
+from .utils import all_subclasses, pop_first
 from ..config import Parameter
+from ..environment import sub_env
 from ..cli import Term
 
 __all__ = ("CheckBase", "CheckException", "CheckResult")
 
 
 class CheckException(Exception):
     """Exception raised when an error is encountered in the setup of a check."""
 
 
 # Storage class for the results of checks
 CheckResult = namedtuple("CheckResult", "passed msg status", defaults=("", ""))
 
 
 class CheckBase(ABC):
-    """Check base class and grouper"""
+    """Check base class and grouper
+
+    .. versionchanged:: 0.9.3
+        Switch to :meth:`environment.sub_env` for value substitutions, which
+        require a '$' character  and allow different expansion rules like
+        defaults, errors and replacements.
+    """
 
     # Unprocessed value for the check
     raw_value: str
 
     # Description of the check
     desc: str = ""
 
@@ -46,19 +53,21 @@
     # If True (default), environment variables in variable_name or
     # variable_value are substituted with the values of other environment
     # variables.
     env_substitute: bool
 
     # The condition for children results to be considered a pass
     condition: t.Callable = all
-    condition_aliases = ("condition", "subchecks")  # other names for variable
+    condition_aliases = ("subchecks", "condition")  # other names for variable
 
     # The default value for env_substitute
     env_substitute_default = Parameter("CHECKBASE.ENV_SUBSTITUTE_DEFAULT", default=True)
-    env_substitute_aliases = ("env_substitute",)  # other names for variable
+
+    # Alternative parameter names for env_substitute
+    env_substitute_aliases = ("substitute", "env_substitute")
 
     # The maximum recursion depth of the load function
     max_level = Parameter("CHECKBASE.MAX_LEVEL", default=10)
 
     def __init__(
         self,
         name: str,
@@ -70,17 +79,16 @@
         self.name = name
         self.value = value
         self.desc = desc
         self.children = list(children) if children is not None else []
 
         # Parse kwargs, which may use different aliases
         condition = pop_first(kwargs, *self.condition_aliases, default=None)
-        self.env_substitute = (
-            pop_first(kwargs, *self.env_substitute_aliases, default=None)
-            or self.env_substitute_default
+        self.env_substitute = pop_first(
+            kwargs, *self.env_substitute_aliases, default=self.env_substitute_default
         )
 
         # Make sure the condition values are allowed
         if condition is None:
             pass
         elif condition in ("all", "All", "ALL"):
             self.condition = all
@@ -99,41 +107,41 @@
         return f"{self.__class__.__name__}({self.name})"
 
     def __len__(self):
         """The number of children"""
         return len(self.children)
 
     @property
+    def value(self) -> t.Any:
+        """Check's value with optional environment substitution"""
+        if self.env_substitute and self.raw_value is not None:
+            subbed = sub_env(self.raw_value)
+            return subbed if subbed is not None else self.raw_value
+        else:
+            return self.raw_value
+
+    @value.setter
+    def value(self, v):
+        self.raw_value = str(v) if v is not None else None
+
+    @property
     def count(self, all: bool = True) -> int:
         """The number of children
 
         Parameters
         ----------
         all
             If True, count all the immediate and nested level children.
             If False, only count the immediate level children.
         """
         # flatten() returns this check, so the count is subtracted by 1 to only
         # count sub-checks
         return len(self.flatten()) - 1 if all else len(self.children)
 
     @property
-    def value(self) -> t.Any:
-        """Check's value with optional environment substitution"""
-        if self.env_substitute and self.raw_value is not None:
-            subbed = sub_env(self.raw_value)
-            return subbed if subbed is not None else self.raw_value
-        else:
-            return self.raw_value
-
-    @value.setter
-    def value(self, v):
-        self.raw_value = str(v) if v is not None else None
-
-    @property
     def is_collection(self) -> bool:
         """Evaluate whether this is a collection check--i.e. it's only a
         check that holds other check groups (BaseCheck instances).
 
         Collection checks have headings that are printed before the results of
         the children are evaluated.
         """
@@ -167,15 +175,15 @@
         elif self.is_collection:
             # Collection checks print right away since we don't need to wait to
             # see the results of "check" for children
             term.p_h2(
                 msg=msg,
                 level=level,
                 status=f" ({self.count} checks)",
-                color_status=term.RESET,
+                style_status={"reset": True},
             )
 
         # Run all children checks
         results = []
         for child in self.children:
             result = child.check(level=level + 1)
             results.append(result)
@@ -184,25 +192,25 @@
         passed = self.condition(result.passed for result in results)
 
         # Print this check's results
         if passed and not self.is_collection:
             term.p_pass(
                 msg=msg,
                 level=level,
-                color_msg=term.BOLD,
                 status=f" ({self.count} checks)",
-                color_status=term.RESET,
+                style_status={"reset": True},
+                style_msg={"bold": True},
             )
         elif not passed and not self.is_collection:
             term.p_fail(
                 msg=msg,
                 level=level,
-                color_msg=term.BOLD,
                 status=f" ({self.count} checks)",
-                color_status=term.RESET,
+                style_status={"reset": True},
+                style_msg={"bold": True},
             )
 
         for result in results:
             if result.msg == "":
                 # This result has already been handled and printed
                 continue
             elif result.passed:
@@ -222,18 +230,19 @@
 
             # Add timing info, if available
             if start_time is not None:
                 total_time = process_time() - start_time
                 msg += f" in {total_time:.2f}s"
 
             # Determine the message color
-            color_msg = term.BOLD + term.GREEN if passed else term.BOLD + term.RED
+            style_msg = {"bold": True}
+            style_msg["fg"] = "green" if passed else "red"
 
             # Print the message
-            term.p_h1(msg, color_msg=color_msg)
+            term.p_h1(msg, style_msg=style_msg)
 
         return CheckResult(passed=passed, msg="", status="")
 
     def flatten(self) -> t.List["CheckBase"]:
         """Return a flattened list of this check (first item) and children
         checks"""
         flattened = [self]
```

### Comparing `geomancy-0.9.1/geomancy/checks/env.py` & `geomancy-0.9.3/geomancy/checks/env.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Checks for environment variables
 """
 import typing as t
 import re
 
 from .base import CheckBase, CheckResult
-from .utils import sub_env
+from ..environment import sub_env
 from ..config import Parameter
 
 
 class CheckEnv(CheckBase):
     """Check the current environment variables."""
 
     # (Optional) regex to match the environment variable value
@@ -38,15 +38,15 @@
             # If the value is None, the environment variable doesn't exist.
             status = "missing"
         elif value == "":
             # An empty string environment variable is considered not set
             status = "empty string"
         elif isinstance(self.regex, str) and re.match(self.regex, value) is None:
             # Check the regex, if specified
-            status = "value does not match regex " "'{regex}'".format(regex=self.regex)
+            status = f"does not match regex '{self.regex}'"
         else:
             # All checks passed!
             status = "passed"
             passed = True
 
         msg = self.msg.format(check=self, status=status)
         return CheckResult(passed=passed, msg=msg, status=status)
```

### Comparing `geomancy-0.9.1/geomancy/checks/exec.py` & `geomancy-0.9.3/geomancy/checks/exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/geomancy/checks/path.py` & `geomancy-0.9.3/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/geomancy/checks/python.py` & `geomancy-0.9.3/geomancy/checks/python.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 Checks for python environment and packages
 """
 import typing as t
 import sys
 import subprocess
+import logging
 import re
 
 from .version import CheckVersion
 from .utils import version_to_tuple
 from ..config import Parameter
 
 __all__ = ("CheckPythonPackage",)
 
+logger = logging.getLogger(__name__)
+
 
 class CheckPythonPackage(CheckVersion):
     """Check the availability and version of a python package"""
 
     # use the pip freeze method
     use_pip_freeze: bool = True
 
     # The regex to use for parsing python package names
-    pip_pkg_str = r"^(?P<name>{pkg_name})==(?P<ver>[\d\w.]+)$"
+    pip_pkg_str = r"^(?P<name>{pkg_name})\s*==\s*(?P<ver>[\d\w.]+)$"
 
     # The results of pip freeze
     pip_freeze: t.Union[str, None]
 
     # The message for checking python packages
     msg = Parameter(
         "CHECKPYTHONPACKAGE.MSG",
@@ -43,40 +46,49 @@
 
         # Method 1 -- try pip freeze
         # First, try loading the freeze.
         if self.use_pip_freeze and not hasattr(self, "pip_freeze"):
             # "pip list" is used instead of "pip freeze" because "pip list"
             # will not show paths--just package names--for packages installed
             # from a local repository
-            proc = subprocess.run(
-                args=(python, "-m", "pip", "list", "--format=freeze"),
-                capture_output=True,
-            )
+            args = (python, "-m", "pip", "list", "--format=freeze")
+            proc = subprocess.run(args=args, capture_output=True)
 
             if proc.returncode != 0:
                 # This command didn't work. Set the class attribute for all
                 # instances
                 CheckPythonPackage.pip_freeze = None
+                logger.debug(f"Trying to use pip_freeze but couldn't run "
+                             f"'{args}'")
             else:
                 CheckPythonPackage.pip_freeze = proc.stdout.decode("UTF-8")
 
         # Parse the pip freeze
         if getattr(self, "pip_freeze", None) is not None:
             pattern = self.pip_pkg_str.format(pkg_name=pkg_name)
             match = re.search(pattern, self.pip_freeze, re.MULTILINE)
 
             # Convert the regex match to a version tuple
             version = match.groupdict()["ver"] if match is not None else None
-            return version_to_tuple(version) if version is not None else None
+            version = version_to_tuple(version) if version is not None else None
+
+            logger.debug(f"Found '{pkg_name}' package version '{version}' with "
+                         f"pip freeze.")
+            if version is not None:
+                return version
 
         # Method 2 -- try importing and getting it from the __version__ string
         code = f"import {pkg_name}; print({pkg_name}.__version__)"
         proc = subprocess.run(args=(python, "-c", code), capture_output=True)
 
         if proc.returncode == 0:
             version_str = (
                 proc.stdout.decode("UTF-8").strip() if proc.stdout is not None else None
             )
-            return version_to_tuple(version_str) if version_str is not None else None
+            version = version_to_tuple(version_str) if version_str is not None else None
+
+            logger.debug(f"Found '{pkg_name}' package version '{version}' with "
+                         f"{pkg_name}.__version__")
+            return version
 
         # I'm out of ideas. Version couldn't be parsed
         return None
```

### Comparing `geomancy-0.9.1/geomancy/checks/utils.py` & `geomancy-0.9.3/geomancy/checks/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Utility functions"""
 import typing as t
-import os
 import operator
 import re
 
-__all__ = ("all_subclasses", "sub_env", "version_to_tuple", "name_and_version")
+__all__ = ("all_subclasses", "version_to_tuple", "name_and_version")
 
 __missing__ = object()  # used an argument for missing values
 
 
 def all_subclasses(cls) -> t.List[t.Type]:
     """Retrieve all subclasses, sub-subclasses and so on for a class
 
@@ -31,34 +30,14 @@
     [<class 'geomancy.checks.utils.B'>, <class 'geomancy.checks.utils.C'>]
     """
     return cls.__subclasses__() + [
         g for s in cls.__subclasses__() for g in all_subclasses(s)
     ]
 
 
-def sub_env(obj):
-    """Substitutes environment variables of the form {VARIABLE_NAME} in
-    strings.
-    """
-    if isinstance(obj, str):
-        try:
-            # Substitute environment variables
-            return obj.format(**os.environ)
-        except KeyError:
-            # Could find the environment variable; return None
-            return None
-    elif hasattr(obj, "__iter__"):
-        # Iterate over items to substitute environment variables
-        o_type = type(obj)
-        items = obj.items() if hasattr(obj, "items") else obj
-        return o_type(sub_env(i) for i in items)
-    else:
-        return obj
-
-
 def pop_first(d: dict, *keys, del_remaining: bool = True, default: t.Any = __missing__):
     """Pop the first key found in the dict.
 
     Parameters
     ----------
     d
         The dict to search for keys to pop
```

### Comparing `geomancy-0.9.1/geomancy/checks/version.py` & `geomancy-0.9.3/geomancy/checks/version.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/geomancy/config/config.py` & `geomancy-0.9.3/geomancy/config/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """An instance-wide configuration"""
 import typing as t
 from threading import Lock
 from pathlib import Path
 from collections.abc import Mapping
 import re
 import tomllib
+import yaml
 import logging
 
 __all__ = ("ConfigException", "Config", "Parameter")
 
 logger = logging.getLogger(__name__)
 
 
@@ -40,14 +41,17 @@
 
     # The thread lock
     _lock: Lock = Lock()
 
     # The regex to validate key names
     key_regex = re.compile(r"^[_A-Za-z][_A-Za-z0-9]*$")
 
+    # Different names for subsections in a dict which could contain config settings
+    section_aliases = ("config", "Config")
+
     def __new__(cls, root: bool = True):
         # Create the singleton instance if it hasn't been created
         if cls._instance is None:
             # Lock the thread
             with cls._lock:
                 # Prevent another thread from creating the instance in the
                 # interim
@@ -80,14 +84,20 @@
             return super().__getattribute__(key)
 
     def __setattr__(self, key, value):
         """Set attributes in the Config"""
         Config.validate(key)
         super().__setattr__(key, value)
 
+    def __eq__(self, other):
+        """Test whether this Config is equal to another"""
+        if not type(self) == type(other):
+            return False
+        return self.__dict__ == other.__dict__
+
     def __len__(self):
         """The number of items in this Config"""
         return len(self.__dict__)
 
     @classmethod
     def validate(cls, key):
         """Ensure that the given key is valid"""
@@ -172,45 +182,53 @@
                 # Otherwise just store the value
                 logger.debug(f"Config.load(): set {k}={v}")
                 setattr(config, k, v)
 
         return config
 
     @classmethod
-    def toml_loads(cls, s: str) -> "Config":
-        """Load config from a string formatted in TOML format.
+    def load_toml(cls, filename: Path) -> "Config":
+        """Load config from a file formatted in TOML format.
 
         Returns
         -------
         config
             The root config instance with parameters loaded
         """
-        d = tomllib.loads(s)
+        with open(filename, "rb") as f:
+            d = tomllib.load(f)
+
+        # If the config dict is an item in 'd', get that instead
+        for alt_name in cls.section_aliases:
+            d = d[alt_name] if alt_name in d else d
         return cls.load(d)
 
     @classmethod
-    def toml_load(cls, filename: Path) -> "Config":
-        """Load config from a file formatted in TOML format.
+    def loads_toml(cls, s: str) -> "Config":
+        """Load config from a string formatted in TOML format.
 
         Returns
         -------
         config
             The root config instance with parameters loaded
         """
-        with open(filename, "rb") as f:
-            d = tomllib.load(f)
+        d = tomllib.loads(s)
+
+        # If the config dict is an item in 'd', get that instead
+        for alt_name in cls.section_aliases:
+            d = d[alt_name] if alt_name in d else d
         return cls.load(d)
 
-    def toml_dumps(self, name="config", level=0) -> str:
+    def dumps_toml(self, name: str = "config", level: int = 0) -> str:
         """Produce a string of the current config in TOML format.
 
         Parameters
         ----------
         name
-            Name of the current section. Sub-sections are identified with '.'
+            Name of the current section. Subsections are identified with '.'
             characters
         level
             Current level of the hierarchy
         """
         indent = " " * 2 * level  # indentation
         text = f"{indent}[{name}]\n"  # section heading
 
@@ -238,23 +256,111 @@
 
         # Next process sections (sub configs)
         items = [
             (k, v) for k, v in sorted(self.__dict__.items()) if isinstance(v, Config)
         ]
         for key, value in items:
             text += indent  # Add indentation
-            text += value.toml_dumps(name=".".join((name, key)), level=level + 1)
+            text += value.dumps_toml(name=".".join((name, key)), level=level + 1)
+
+        if level == 0:
+            text = text.rstrip("\n") + "\n"  # Remove multiple terminal newlines
+        return text
+
+    @classmethod
+    def load_yaml(cls, filename: Path) -> "Config":
+        """Load config from a file formatted in YAML format.
+
+        Returns
+        -------
+        config
+            The root config instance with parameters loaded
+        """
+        with open(filename, "r") as f:
+            d = yaml.load(f, yaml.SafeLoader)
+
+        # If the config dict is an item in 'd', get that instead
+        for alt_name in cls.section_aliases:
+            d = d[alt_name] if alt_name in d else d
+        return cls.load(d)
+
+    @classmethod
+    def loads_yaml(cls, s: str) -> "Config":
+        """Load config from a string formatted in YAML format.
+
+        Returns
+        -------
+        config
+            The root config instance with parameters loaded
+        """
+        d = yaml.load(s, yaml.SafeLoader)
+
+        # If the config dict is an item in 'd', get that instead
+        for alt_name in cls.section_aliases:
+            d = d[alt_name] if alt_name in d else d
+        return cls.load(d)
+
+    def dumps_yaml(
+        self, name: str = "config", indent_spaces: int = 2, level: int = 0
+    ) -> str:
+        """Produce a string of the current config in YAML format.
+
+        Parameters
+        ----------
+        name
+            Name of the current section.
+        indent_spaces
+            Number of spaces to indent subsections.
+        level
+            Current level of the hierarchy
+        """
+        indent = " " * indent_spaces * level  # indentation
+        text = f"{indent}{name}:\n"  # section heading
+
+        # Process general parameters before sections (sub configs)
+        items = [
+            (k, v)
+            for k, v in sorted(self.__dict__.items())
+            if not isinstance(v, Config)
+        ]
+        for key, value in items:
+            text += indent + " " * indent_spaces  # Add indentation
+
+            # Different simple parameter formats for TOML
+            if isinstance(value, str) and "'" not in value:
+                text += f"{key}: '{value}'\n"
+            elif isinstance(value, str):
+                text += f'{key}: "{value}"\n'
+            elif isinstance(value, bool):
+                text += f"{key}: {value}\n"
+            else:
+                text += f"{key}: {value}\n"
+
+        if len(items) > 0:
+            text += "\n"
+
+        # Next process sections (sub configs)
+        items = [
+            (k, v) for k, v in sorted(self.__dict__.items()) if isinstance(v, Config)
+        ]
+        for key, value in items:
+            text += indent  # Add indentation
+            text += value.dumps_yaml(name=key, level=level + 1)
 
         if level == 0:
             text = text.rstrip("\n") + "\n"  # Remove multiple terminal newlines
         return text
 
     def pprint_toml(self):
         """Pretty print in TOML format."""
-        print(self.toml_dumps())
+        print(self.dumps_toml())
+
+    def pprint_yaml(self):
+        """Pretty print in YAML format"""
+        print(self.dumps_yaml())
 
 
 # dummy placeholder object
 missing = object()
 
 
 class Parameter:
```

### Comparing `geomancy-0.9.1/geomancy/environment/load_environment.py` & `geomancy-0.9.3/tests/entrypoints/test_geo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,147 @@
-"""Functions to load dotenv files"""
+"""Test the main CLI entrypoint"""
 import typing as t
-import os
-import re
-import logging
 from pathlib import Path
+from itertools import chain
+import os
 
-__all__ = ("parse_env_str", "load_env")
+from click.testing import CliRunner
+import pytest
 
-logger = logging.getLogger(__name__)
+from geomancy.entrypoints import geo_cli
+from geomancy.config import Config
+
+
+def get_checks_files():
+    """Return a list of checks files to check"""
+    checks_files = []
+
+    # examples/
+    for ext in ("toml", "yaml"):
+        checks_files += list(Path("examples").glob(f"*.{ext}"))
+
+    return checks_files
+
+
+@pytest.fixture
+def run() -> t.Callable:
+    """Run the CLI with the given option, check for the expected exit
+    code and return the output"""
+
+    def runcmd(args, expected_code: int = 0):
+        args = [args] if isinstance(args, str) else args
+
+        runner = CliRunner()
+        result = runner.invoke(geo_cli, args)
+        if result.exit_code != expected_code:
+            print(result.output)
+        assert result.exit_code == expected_code
+        return result
+
+    runcmd.__doc__ = run.__doc__
+    return runcmd
+
+
+@pytest.fixture
+def config() -> Config:
+    return Config()
+
+
+@pytest.mark.parametrize("options", ("--help",))
+def test_cli_help(run, options):
+    """Test the --help message"""
+    result = run(options)
+    assert "Show this message and exit" in result.output
 
-# Regex to match "name=value" pairs from an env file
-env_re = re.compile(
-    r"""
-    ^\s*(?P<name>[a-zA-Z_]+[a-zA-Z0-9_]*)  # Variable name
-    \s*=\s*  # operator to assign value
-    ((?P<quote>["|']{1,3})\s*(?P<qvalue>.+?)\s*(?P=quote)|  # quoted value
-     (?P<value>[^'"\n]+))  # non-quoted value
-    \s*$
-    """,
-    re.MULTILINE | re.VERBOSE | re.DOTALL,
-)
-
-# Regex to strip comments to the end of a line--# and not escaped values, \#
-comment_re = re.compile(r"([^\\])(#.+)$")
-
-# Regex to match environment variables for subsitution--e.g. {NAME} or ${NAME}
-sub_re = re.compile(r"[$]?{\s*(?P<name>[A-Za-z_]\w*)\s*}")  # Match env variables
-
-
-def parse_env_str(
-    string: str,
-    strip_values: bool = True,
-    substitute: bool = True,
-) -> dict:
-    """Parse a string in env format into a dict
-
-    Parameters
-    ----------
-    string
-        The string in env format to parse
-    strip_values
-        Remove whitespace at the start and end of non-quoted values
-    substitute
-        Try substituting environment variable values in the form of '${NAME}'
-        or '{NAME}' if available in the environment
-
-    Returns
-    -------
-    env_vars
-        The parsed environment variables from the string. The variable names
-        are dict keys and the variable values are dict values.
-    """
-    # Strip comments (everything after #, but not \#
-    string = comment_re.sub(r"\1", string)
 
-    # Convert string into a dict
-    env_vars = dict()
-    for match in env_re.finditer(string):
-        groupdict = match.groupdict()
-        name = groupdict["name"]
-
-        if "value" in groupdict and groupdict["value"]:
-            # Parse non-quoted values
-            env_vars[name] = (
-                groupdict["value"].strip() if strip_values else groupdict["value"]
-            )
-        elif "qvalue" in groupdict and groupdict["qvalue"]:
-            # Parse quoted value
-            env_vars[name] = groupdict["qvalue"]
-        else:
-            continue
-
-    # Substitute environment variables in values
-    def sub_func(m: re.Match):
-        """Substitute a regex match from the environment variables, if possible,
-        or return unmodified"""
-        name = m.groupdict()["name"]
-        if name in os.environ:
-            return os.environ[name]
-        elif name in env_vars:
-            return env_vars[name]
-        else:
-            return m.group()
-
-    items = env_vars.items()
-    for k, v in items:
-        # Substitute environment variables
-        if substitute:
-            env_vars[k] = sub_re.sub(sub_func, v)
-    return env_vars
-
-
-def load_env(
-    filepath: t.Union[str, Path], overwrite: bool = False, *args, **kwargs
-) -> int:
-    """Load an environment file.
-
-    Parameters
-    ----------
-    filepath
-        The path to the file with environment settings to load
-    overwrite
-        If True, overwrite environment variables that already exist
-        If False (default), only load environment variables that don't already exist
-    args, kwargs
-        Arguments and keyword arguments passed to :func:`parse_env_str`
-
-    Returns
-    -------
-    env_substituted
-        The number of environment variables substituted
+@pytest.mark.parametrize("options", get_checks_files())
+def test_cli_check(run, options):
+    """Test CLI with all the checks files individually in the examples directory"""
+    result = run(str(options))
+
+    # Check, for example, that environment variables were checked
+    assert any(
+        msg in result.output for msg in ("Check environment variable", "Check path")
+    )
+
+
+@pytest.mark.parametrize("options", ("examples/geomancy.*",))
+def test_cli_check_glob(run, options):
+    """Test the CLI with glob patterns"""
+    result = run(str(options))
+
+    # Check, for example, that environment variables were checked
+    assert any(
+        msg in result.output for msg in ("Check environment variable", "Check path")
+    )
+
+
+@pytest.mark.parametrize("flag", ("", "--toml", "--yaml"))
+def test_cli_config(run, flag):
+    """Test the --config option"""
+    if flag:
+        result = run(("config", flag))
+    else:
+        result = run(("config",))
+    assert "config" in result.output  # config output in TOML/yaml format
+
+
+@pytest.mark.parametrize("flag", ("-e", "--env"))
+def test_cli_handle_env(run, flag, test_env_file):
+    """Test the handling of -e/--env and --overwrite flags for loading
+    environment variables.
+
+    See ./conftest.py for details on the 'test_env_file' fixture
     """
-    # Try loading the file
-    filepath = Path(filepath)
-    try:
-        string = filepath.read_text()
-    except FileNotFoundError:
-        logger.error(f"Could not file the file '{filepath}'")
-        return 0
-
-    # Parse the environment
-    env_vars = parse_env_str(string=string, *args, **kwargs)
-
-    # Load the environment variables
-    count = 0
-    for name, value in env_vars.items():
-        # Do nothing if the variable already exists, and overwrite isn't specified
-        if name in os.environ and not overwrite:
-            continue
+    # Get a single checks file to test against
+    checks_file = get_checks_files()[0]
+
+    # Set up the env files
+    env_filepath = test_env_file["filepath"]
+    variables = test_env_file["variables"]
+
+    # running '--overwrite' without '-e/--env' gives an error
+    result = run("--overwrite", expected_code=2)
+
+    with pytest.MonkeyPatch.context() as mp:
+        # Reset env variables
+        for name in variables.keys():
+            mp.delenv(name, raising=False)
 
-        os.environ[name] = value
-        count += 1
+        # The variables are in the environment (os.environ)
+        for name, value in variables.items():
+            assert name not in os.environ
 
-        logger.debug(f"Substituted environment variable {name}={value}")
-    logger.debug(f"Substituted {count} environment variables from {filepath}")
+        # running "-e/--env" should load environment variables, which are logged
+        # in debug mode
+        options = ("-d", flag, env_filepath, "checks", str(checks_file))
+        result = run(options)
 
-    return count
+        # The variables are loaded in the current process
+        for name, value in variables.items():
+            assert os.environ[name] == value
+
+
+def test_cli_run(run, test_env_file):
+    """Test the 'run' subcommand and the handle_env function.
+
+    See ./conftest.py for details on the 'test_env_file' fixture.
+    """
+    # Set up the env files
+    filepath = test_env_file["filepath"]
+    variables = test_env_file["variables"]
+
+    with pytest.MonkeyPatch.context() as mp:
+        # Reset env variables
+        for name in variables.keys():
+            mp.delenv(name, raising=False)
+
+        # The variables are in the environment (os.environ)
+        for name, value in variables.items():
+            assert name not in os.environ
+
+        # Run the command with the 'run' subcommand
+        result = run(("run", "-e", filepath, "echo", "here!"))
+
+        # The variables are loaded in the current process
+        for name, value in variables.items():
+            assert os.environ[name] == value
```

### Comparing `geomancy-0.9.1/geomancy.egg-info/PKG-INFO` & `geomancy-0.9.3/geomancy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.9.1
+Version: 0.9.3
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -55,15 +55,15 @@
     ```yaml
     checks:
       Environment:
         desc: Check environment variables common to all development environments
 
         Username:
           desc: The current username
-          checkEnv: "{USER}"
+          checkEnv: "$USER"
           regex: "[a-z_][a-z0-9_-]*[$]?"
 
       Paths:
         desc: Checks the existence of needed files and directories
         subchecks: any  # at least one of the files must be present
 
           Geomancy:
@@ -86,49 +86,56 @@
 2. Use ``geo`` to run the checks.
 
     ```shell
     $ geo
     =============================== .geomancy.toml ================================
         checks (9 checks)
     [✔]   Environment (1 checks)
-    [✔]     Check environment variable '{USER}'...passed
+    [✔]     Check environment variable '$USER'...passed
     [✔]   Paths (2 checks)
     [✔]     Check path 'examples/geomancy.toml'...passed
     [✔]     Check path 'examples/pyproject.toml'...passed
     [✔]   Executables (1 checks)
     [✔]     Check executable 'python3>=3.11'...passed
     ========================== PASSED.  8 checks in 0.01s =========================
     ```
 
     (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 ## Features
 <!-- start features -->
-``geomancy`` can:
+Geomancy checks include:
 
-- __Environment variables__. Check environment variables are properly set and,
-  optionally, check that they have valid values
+- __Environment variables__ are properly set and, optionally,
+  check that they have valid values with regular expressions
   ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
-- __Paths__. Check file and directory path existence
+- __Paths__ exist and whether they're files or directories
   ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
-- __Executables__. Check executables are available and, optionally, have the
-  minimum or correct versions
+- __Executables__ are available and, optionally, have the minimum or correct
+  versions
   ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
-- __Python Packages__. Check python packages are available and, optionally,
-  have the minimum or correct versions
+- __Python packages__ are available and, optionally, have the minimum or
+  correct versions
   ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
-- __Group Checks__. Nested group checks with conditional (all or any) pass
+- __Group checks__ to nested groups of checks with conditional (all or any) pass
   criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
-- __Environment Substitution__. Substitute parameter values from environment
-  variables. ex: ``checkPath: {HOME}/.geomancy.toml``
-- __Multiple Formats__. Checks files can be in yaml (e.g. ``.geomancy.yaml``)
-  or in [toml](https://toml.io/en/) (e.g. ``.geomancy.toml`` or
-  ``pyproject.toml``)
+
+Additionally, geomancy can:
+
+- __Load environment files__ for
+  [checks](https://geomancy.readthedocs.io/en/latest/usage/cmd_checks.html#environment-files)
+  or for [running](https://geomancy.readthedocs.io/en/latest/usage/cmd_run.html#running-environments)
+  shell commands
+- __Substitute environment variables__ in check values e.g.:
+  ``checkPath: {HOME}/.geomancy.toml``
+- __Load checks in multiple formats__ including [yaml](https://yaml.org)
+  (e.g. ``.geomancy.yaml``) or in [toml](https://toml.io/en/)
+  (e.g. ``.geomancy.toml`` or ``pyproject.toml``)
 <!-- end features -->
 
 ## Documentation
 
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
```

### Comparing `geomancy-0.9.1/geomancy.egg-info/SOURCES.txt` & `geomancy-0.9.3/geomancy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 .editorconfig
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
 Taskfile.yaml
 pyproject.toml
+.github/workflows/tests.yml
 changelog/changelog_template.jinja
 docs/changelog.md
 docs/conf.py
 docs/index.md
 docs/quickstart.md
 docs/_static/custom.css
 docs/_static/geomancy_logo.png
 docs/_static/geomancy_logo.svg
-docs/usage/index.md
+docs/usage/cmd_checks.md
+docs/usage/cmd_run.md
+docs/usage/format.md
 examples/geomancy.toml
 examples/geomancy.yaml
 examples/geomancy_flat.yaml
 examples/pyproject.toml
 geomancy/__description__.txt
 geomancy/__init__.py
-geomancy/main.py
 geomancy.egg-info/PKG-INFO
 geomancy.egg-info/SOURCES.txt
 geomancy.egg-info/dependency_links.txt
 geomancy.egg-info/entry_points.txt
 geomancy.egg-info/requires.txt
 geomancy.egg-info/top_level.txt
 geomancy/checks/__init__.py
@@ -35,21 +37,27 @@
 geomancy/checks/python.py
 geomancy/checks/utils.py
 geomancy/checks/version.py
 geomancy/cli/__init__.py
 geomancy/cli/term.py
 geomancy/config/__init__.py
 geomancy/config/config.py
+geomancy/entrypoints/__init__.py
+geomancy/entrypoints/check.py
+geomancy/entrypoints/config.py
+geomancy/entrypoints/environment.py
+geomancy/entrypoints/geo.py
+geomancy/entrypoints/run.py
+geomancy/entrypoints/utils.py
 geomancy/environment/__init__.py
-geomancy/environment/load_environment.py
+geomancy/environment/dotenv.py
 tests/conftest.py
-tests/test_main.py
 tests/checks/test_base.py
 tests/checks/test_env.py
 tests/checks/test_exec.py
 tests/checks/test_path.py
 tests/checks/test_python.py
-tests/checks/test_utils.py
 tests/config/config1.toml
 tests/config/test_config.py
 tests/data/test.env
-tests/environment/test_load_environment.py
+tests/entrypoints/test_geo.py
+tests/environment/test_dotenv.py
```

### Comparing `geomancy-0.9.1/pyproject.toml` & `geomancy-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Topic :: Software Development :: Testing :: Acceptance",
     "Topic :: System :: Monitoring",
     "Topic :: System :: Systems Administration",
     "Topic :: Utilities",
     "Development Status :: 4 - Beta",
     ]
 dynamic = ["version", "description"]
-dependencies = ["pyyaml>=6.0"]
+dependencies = ["pyyaml>=6.0", "click>=8.1", "click-default-group"]
 
 [tool.setuptools]
 packages = ["geomancy"]
 
 [tool.setuptools.dynamic]
 version = {attr = "geomancy.__version__"}
 description = {file = "geomancy/__description__.txt"}
@@ -51,15 +51,15 @@
     "sphinx-book-theme",
     "sphinx_design>=0.4",
     "myst-parser>=2.0",
     "towncrier",
 ]
 
 [project.scripts]
-geo = "geomancy.main:main_cli"
+geo = "geomancy.entrypoints:geo_cli"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
 [tool.towncrier]
 package = "geomancy"
 filename = "docs/changelog.md"
```

### Comparing `geomancy-0.9.1/tests/checks/test_env.py` & `geomancy-0.9.3/tests/checks/test_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from geomancy.checks import CheckEnv
 
 
 def test_check_env_missing():
     """Test CheckEnv for a missing environment variable"""
     with MonkeyPatch.context() as mp:
         mp.delenv("MISSING", raising=False)
-        check = CheckEnv(name="missing", value="{MISSING}")
+        check = CheckEnv(name="missing", value="${MISSING}")
         assert not check.check().passed
 
 
 def test_check_env_present():
     """Test CheckEnv for a present environment variable"""
     with MonkeyPatch.context() as mp:
         mp.setenv("PRESENT", "VALUE")
 
-        check = CheckEnv(name="PRESENT", value="{PRESENT}")
+        check = CheckEnv(name="PRESENT", value="${PRESENT}")
         assert check.name == "PRESENT"
         assert check.value == "VALUE"
         assert check.check().passed
 
 
 def test_check_env_name_substitution(
     variable_name="VARIABLE_NAME", variable_value="PATH"
@@ -35,19 +35,20 @@
     # Set the VariableName environment variable to be the name of another
     # environment variable that exists
     with MonkeyPatch.context() as mp:
         mp.setenv(variable_name, variable_value)
 
         # Setup the check to use the variable name with environment variable
         # substitution--i.e. wrap it in curly braces
-        check = CheckEnv(name="substitution", value="{" + variable_name + "}")
+        check = CheckEnv(name="substitution", value=f"${variable_name}")
 
         # Check that the subsitution is correct
         assert check.name == "substitution"
-        assert check.raw_value == "{" + variable_name + "}"  # hidden var
+        assert check.raw_value == f"${variable_name}"  # unprocessed value
+        assert check.value == variable_value
 
         assert check.check().passed
 
 
 def test_check_env_regex(
     variable_name="VARIABLE_NAME", variable_value="dev", regex="dev|prod|local"
 ):
@@ -55,23 +56,23 @@
     assert variable_name not in os.environ
 
     # Place the variable in the environment and test the regex
     with MonkeyPatch.context() as mp:
         mp.setenv(variable_name, variable_value)
 
         # The regex should match
-        check1 = CheckEnv(name="regex1", value="{" + variable_name + "}", regex=regex)
+        check1 = CheckEnv(name="regex1", value=f"${variable_name}", regex=regex)
         assert check1.check().passed
 
         # Change the variable value to something else in which the regex will
         # fail
-        mp.setenv(variable_name, "!" + variable_value + "!")
+        mp.setenv(variable_name, f"!{variable_value}!")
 
         # The regex should not match
-        check2 = CheckEnv(name="regex2", value="{" + variable_name + "}", regex=regex)
+        check2 = CheckEnv(name="regex2", value=f"${variable_name}", regex=regex)
         assert not check2.check().passed
 
 
 def test_check_base_types_dict():
     """Test the CheckBase.types_dict() method for the CheckEnv class."""
     types = CheckEnv.types_dict()
```

### Comparing `geomancy-0.9.1/tests/checks/test_path.py` & `geomancy-0.9.3/tests/checks/test_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,24 +55,21 @@
     """Test CheckPath with environmental subsitution"""
     # Create the test files and dirs
     ENV = "dev"
     tmp_file = tmp_path / ENV / "exists.txt"
     tmp_file.parent.mkdir()
     tmp_file.touch()
 
-    path = tmp_path / "{ENV}" / "exists.txt"
-    assert "{ENV}" in str(path)  # not substituted yet
+    path = tmp_path / "$ENV" / "exists.txt"
+    assert "$ENV" in str(path)  # not substituted yet
 
     with pytest.MonkeyPatch.context() as mp:
         # Make sure the ENV variable hasn't been created yet
         mp.delenv("ENV", raising=False)
 
         # The variable doesn't exist so the check should fail
         check = CheckPath(name="PathEnvVariable", value=path)
-        assert "{ENV}" in check.value  # Not substituted yet
         assert not check.check().passed
 
         # Set the ENV variable, and it should now work
         mp.setenv("ENV", ENV)
-        assert "{ENV}" not in check.value  # Substituted
-        assert ENV in check.value
         assert check.check().passed
```

### Comparing `geomancy-0.9.1/tests/checks/test_python.py` & `geomancy-0.9.3/tests/checks/test_python.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.1/tests/config/test_config.py` & `geomancy-0.9.3/tests/config/test_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -193,17 +193,67 @@
     # Try a bad update that eliminates a section
     with pytest.raises(ConfigException):
         config.update(bad_updates)
 
     assert config.section1.subsection1 == 1  # config remains
 
 
+@pytest.mark.parametrize(
+    "ext,save_file",
+    (
+        ("toml", False),
+        ("toml", True),
+        ("yaml", False),
+        ("yaml", True),
+    ),
+)
+def test_config_parsing_strings(reset_config, tmp_path, ext, save_file):
+    """Test Config load/dump string methods"""
+    # Setup a config
+    config = Config()
+    config.a = 1
+    config.b = "string"
+    config.c = True
+    config.d.a = "subsection1"
+    config.d.b = "subsection2"
+
+    # Create a string from the default config
+    dict_copy = dict(config.__dict__)
+    assert len(dict_copy) == 4  # 'a', 'b', 'c'  and 'd'
+
+    # Create a string from the config
+    meth = getattr(config, f"dumps_{ext}")
+    config_str = meth()
+    assert config_str.strip() != ""
+
+    # Optionally save the string to a file
+    if save_file:
+        filepath = (tmp_path / "test").with_stem("." + ext)
+        filepath.write_text(config_str)
+    else:
+        filepath = None
+
+    Config._instance = None  # reset singleton
+
+    # Try reloading the string
+    if save_file:
+        meth = getattr(Config, f"load_{ext}")
+        new_config = meth(filepath)
+    else:
+        meth = getattr(Config, f"loads_{ext}")
+        new_config = meth(config_str)
+
+    # Make sure the new dict matches the old
+    assert len(dict_copy) == 4 and len(new_config.__dict__) == 4
+    assert dict_copy == new_config.__dict__
+
+
 def test_config_toml_parsing(reset_config):
     """Test Config with the parsing of TOML strings and files"""
     # Load the toml file
     filename = Path(__file__).parent / "config1.toml"
-    config = Config.toml_load(filename)
+    config = Config.load_toml(filename)
 
     # Check the parsed config
     assert config.checkEnv.env_substitute
     assert config.checkEnv.msg == "A test message"
     assert config.checkEnv.value.nested == 1
```

### Comparing `geomancy-0.9.1/tests/conftest.py` & `geomancy-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

