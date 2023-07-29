# Comparing `tmp/Subsearch-2.37.1.tar.gz` & `tmp/Subsearch-2.38.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.37.1.tar", last modified: Sun Jul 16 04:38:23 2023, max compression
+gzip compressed data, was "Subsearch-2.38.0rc1.tar", last modified: Sat Jul 29 16:20:14 2023, max compression
```

## Comparing `Subsearch-2.37.1.tar` & `Subsearch-2.38.0rc1.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.778426 Subsearch-2.37.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-16 04:38:03.000000 Subsearch-2.37.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-16 04:38:03.000000 Subsearch-2.37.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-16 04:38:23.778426 Subsearch-2.37.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-16 04:38:03.000000 Subsearch-2.37.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-16 04:38:03.000000 Subsearch-2.37.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:38:23.778426 Subsearch-2.37.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-16 04:38:03.000000 Subsearch-2.37.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.770425 Subsearch-2.37.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.770425 Subsearch-2.37.1/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-16 04:38:23.000000 Subsearch-2.37.1/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-16 04:38:23.000000 Subsearch-2.37.1/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:38:23.000000 Subsearch-2.37.1/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 04:38:23.000000 Subsearch-2.37.1/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:38:23.000000 Subsearch-2.37.1/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-16 04:38:23.000000 Subsearch-2.37.1/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 04:38:23.000000 Subsearch-2.37.1/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.770425 Subsearch-2.37.1/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.774425 Subsearch-2.37.1/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/data/data_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.774425 Subsearch-2.37.1/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/gui_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resource_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.774425 Subsearch-2.37.1/src/subsearch/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.774425 Subsearch-2.37.1/src/subsearch/gui/resources/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/assets/spritesheet.png
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/assets/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.774425 Subsearch-2.37.1/src/subsearch/gui/resources/styles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/styles/sprites.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/styles/style_subsearch.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/resources/styles/theme_setter.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/screen_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.774425 Subsearch-2.37.1/src/subsearch/gui/screens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/screens/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/screens/language_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/screens/search_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/screens/subsearch_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/gui/system_tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.778426 Subsearch-2.37.1/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:23.778426 Subsearch-2.37.1/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/app_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-16 04:38:03.000000 Subsearch-2.37.1/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.880535 Subsearch-2.38.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 16:20:14.000000 Subsearch-2.38.0rc1/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/language_data.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resource_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/spritesheet.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/sprites.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screen_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/gui/screens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/language_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/screens/subsearch_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/system_tray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.884535 Subsearch-2.38.0rc1/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/core_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:20:14.888535 Subsearch-2.38.0rc1/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-29 16:19:59.000000 Subsearch-2.38.0rc1/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.37.1/LICENSE` & `Subsearch-2.38.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.1/PKG-INFO` & `Subsearch-2.38.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.37.1
-Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
+Version: 2.38.0rc1
+Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
 Classifier: Programming Language :: Python :: 3.10
@@ -57,30 +57,29 @@
 - [Contributing](https://github.com/vagabondHustler/SubSearch/blob/main/.github/CONTRIBUTING.md)
 - [Reporting a Vulnerability](https://github.com/vagabondHustler/SubSearch/blob/main/.github/SECURITY.md)
 
 ## About <a name = "about"></a>
 
 #### Key Features
   
-  - Initiate a search for subtitles by simply right-clicking on a media file.
-  - Search for subtitles in 70 different languages
-  - User-friendly GUI for easy customization and configuration
-  - Available in three options, including a compiled executable and source code on GitHub and PyPI
-  - The setup process is straightforward and has minimal reliance on external modules.
+- Initiate a search for subtitles by simply right-clicking on a media file.
+- Search for subtitles in 70 different languages
+- User-friendly GUI for easy customization and configuration
+- Available in three options, including a compiled executable and source code on GitHub and PyPI
+- The setup process is straightforward and has minimal reliance on external modules.
 
-#### Details 
+#### Details
 
 Subsearch is an automated subtitle downloader and extractor that allows users to search and download subtitles for movies and TV shows with a single click from the context menu. The application features a graphical user interface for configuring settings, including options for searching subtitles in 70 different languages from various subtitle sites, filtering hearing-impaired subtitles, and adjusting filename matching criteria.
 
 The application has a user-friendly GUI for all custom settings that can be easily configured. It supports 70 different languages, most of which work on all available subtitle sites. Users can configure it to include hearing impaired subtitles only, non-hearing impaired subtitles only, or both. They can also adjust how strictly the file name matches the search results.
 
 The tool is available in three different options: as a compiled executable that can be run without the need for a Python interpreter and imported modules, as source code on GitHub, and on PyPI. Users can pick the source that suits them best.
 
-Initially created as a personal project to learn Python programming and git version control, this application has evolved into a daily-use tool that I continue to enjoy working on. While there are many similar repositories available that automatically download subtitles from the internet, this project may offer unique features that set it apart. The setup process has been designed to be as straightforward as possible with minimal reliance on external modules. 
-
+Initially created as a personal project to learn Python programming and git version control, this application has evolved into a daily-use tool that I continue to enjoy working on. While there are many similar repositories available that automatically download subtitles from the internet, this project may offer unique features that set it apart. The setup process has been designed to be as straightforward as possible with minimal reliance on external modules.
 
 ## Preview <a name = "preview"></a>
 
 <div align="center">
 
 ![prtsc_example](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/example.gif)
 
@@ -140,7 +139,8 @@
 
 - [othneildrew/Best-README-Template](https://github.com/othneildrew/Best-README-Template)
 - [pimoroni/template-python](https://github.com/pimoroni/template-python/blob/master/.github/CONTRIBUTING.md)
 - [manojmj92/subtitle-downloader](https://github.com/manojmj92/subtitle-downloader)
 - [psf/black](https://github.com/psf/black)
 - [zavoloklom/material-design-iconic-font](https://github.com/zavoloklom/material-design-iconic-font)
 - [rdbende/Sun-Valley-ttk-theme](https://github.com/rdbende/Sun-Valley-ttk-theme)
+- [siddheshsathe/handy-decorators](https://github.com/siddheshsathe/handy-decorators)
```

### Comparing `Subsearch-2.37.1/README.md` & `Subsearch-2.38.0rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,30 +34,29 @@
 - [Contributing](https://github.com/vagabondHustler/SubSearch/blob/main/.github/CONTRIBUTING.md)
 - [Reporting a Vulnerability](https://github.com/vagabondHustler/SubSearch/blob/main/.github/SECURITY.md)
 
 ## About <a name = "about"></a>
 
 #### Key Features
   
-  - Initiate a search for subtitles by simply right-clicking on a media file.
-  - Search for subtitles in 70 different languages
-  - User-friendly GUI for easy customization and configuration
-  - Available in three options, including a compiled executable and source code on GitHub and PyPI
-  - The setup process is straightforward and has minimal reliance on external modules.
+- Initiate a search for subtitles by simply right-clicking on a media file.
+- Search for subtitles in 70 different languages
+- User-friendly GUI for easy customization and configuration
+- Available in three options, including a compiled executable and source code on GitHub and PyPI
+- The setup process is straightforward and has minimal reliance on external modules.
 
-#### Details 
+#### Details
 
 Subsearch is an automated subtitle downloader and extractor that allows users to search and download subtitles for movies and TV shows with a single click from the context menu. The application features a graphical user interface for configuring settings, including options for searching subtitles in 70 different languages from various subtitle sites, filtering hearing-impaired subtitles, and adjusting filename matching criteria.
 
 The application has a user-friendly GUI for all custom settings that can be easily configured. It supports 70 different languages, most of which work on all available subtitle sites. Users can configure it to include hearing impaired subtitles only, non-hearing impaired subtitles only, or both. They can also adjust how strictly the file name matches the search results.
 
 The tool is available in three different options: as a compiled executable that can be run without the need for a Python interpreter and imported modules, as source code on GitHub, and on PyPI. Users can pick the source that suits them best.
 
-Initially created as a personal project to learn Python programming and git version control, this application has evolved into a daily-use tool that I continue to enjoy working on. While there are many similar repositories available that automatically download subtitles from the internet, this project may offer unique features that set it apart. The setup process has been designed to be as straightforward as possible with minimal reliance on external modules. 
-
+Initially created as a personal project to learn Python programming and git version control, this application has evolved into a daily-use tool that I continue to enjoy working on. While there are many similar repositories available that automatically download subtitles from the internet, this project may offer unique features that set it apart. The setup process has been designed to be as straightforward as possible with minimal reliance on external modules.
 
 ## Preview <a name = "preview"></a>
 
 <div align="center">
 
 ![prtsc_example](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/example.gif)
 
@@ -117,7 +116,8 @@
 
 - [othneildrew/Best-README-Template](https://github.com/othneildrew/Best-README-Template)
 - [pimoroni/template-python](https://github.com/pimoroni/template-python/blob/master/.github/CONTRIBUTING.md)
 - [manojmj92/subtitle-downloader](https://github.com/manojmj92/subtitle-downloader)
 - [psf/black](https://github.com/psf/black)
 - [zavoloklom/material-design-iconic-font](https://github.com/zavoloklom/material-design-iconic-font)
 - [rdbende/Sun-Valley-ttk-theme](https://github.com/rdbende/Sun-Valley-ttk-theme)
+- [siddheshsathe/handy-decorators](https://github.com/siddheshsathe/handy-decorators)
```

### Comparing `Subsearch-2.37.1/setup.py` & `Subsearch-2.38.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.1/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.38.0rc1/src/Subsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.37.1
-Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
+Version: 2.38.0rc1
+Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
 Classifier: Programming Language :: Python :: 3.10
@@ -57,30 +57,29 @@
 - [Contributing](https://github.com/vagabondHustler/SubSearch/blob/main/.github/CONTRIBUTING.md)
 - [Reporting a Vulnerability](https://github.com/vagabondHustler/SubSearch/blob/main/.github/SECURITY.md)
 
 ## About <a name = "about"></a>
 
 #### Key Features
   
-  - Initiate a search for subtitles by simply right-clicking on a media file.
-  - Search for subtitles in 70 different languages
-  - User-friendly GUI for easy customization and configuration
-  - Available in three options, including a compiled executable and source code on GitHub and PyPI
-  - The setup process is straightforward and has minimal reliance on external modules.
+- Initiate a search for subtitles by simply right-clicking on a media file.
+- Search for subtitles in 70 different languages
+- User-friendly GUI for easy customization and configuration
+- Available in three options, including a compiled executable and source code on GitHub and PyPI
+- The setup process is straightforward and has minimal reliance on external modules.
 
-#### Details 
+#### Details
 
 Subsearch is an automated subtitle downloader and extractor that allows users to search and download subtitles for movies and TV shows with a single click from the context menu. The application features a graphical user interface for configuring settings, including options for searching subtitles in 70 different languages from various subtitle sites, filtering hearing-impaired subtitles, and adjusting filename matching criteria.
 
 The application has a user-friendly GUI for all custom settings that can be easily configured. It supports 70 different languages, most of which work on all available subtitle sites. Users can configure it to include hearing impaired subtitles only, non-hearing impaired subtitles only, or both. They can also adjust how strictly the file name matches the search results.
 
 The tool is available in three different options: as a compiled executable that can be run without the need for a Python interpreter and imported modules, as source code on GitHub, and on PyPI. Users can pick the source that suits them best.
 
-Initially created as a personal project to learn Python programming and git version control, this application has evolved into a daily-use tool that I continue to enjoy working on. While there are many similar repositories available that automatically download subtitles from the internet, this project may offer unique features that set it apart. The setup process has been designed to be as straightforward as possible with minimal reliance on external modules. 
-
+Initially created as a personal project to learn Python programming and git version control, this application has evolved into a daily-use tool that I continue to enjoy working on. While there are many similar repositories available that automatically download subtitles from the internet, this project may offer unique features that set it apart. The setup process has been designed to be as straightforward as possible with minimal reliance on external modules.
 
 ## Preview <a name = "preview"></a>
 
 <div align="center">
 
 ![prtsc_example](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/example.gif)
 
@@ -140,7 +139,8 @@
 
 - [othneildrew/Best-README-Template](https://github.com/othneildrew/Best-README-Template)
 - [pimoroni/template-python](https://github.com/pimoroni/template-python/blob/master/.github/CONTRIBUTING.md)
 - [manojmj92/subtitle-downloader](https://github.com/manojmj92/subtitle-downloader)
 - [psf/black](https://github.com/psf/black)
 - [zavoloklom/material-design-iconic-font](https://github.com/zavoloklom/material-design-iconic-font)
 - [rdbende/Sun-Valley-ttk-theme](https://github.com/rdbende/Sun-Valley-ttk-theme)
+- [siddheshsathe/handy-decorators](https://github.com/siddheshsathe/handy-decorators)
```

### Comparing `Subsearch-2.37.1/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.38.0rc1/src/Subsearch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,49 +10,48 @@
 src/Subsearch.egg-info/not-zip-safe
 src/Subsearch.egg-info/requires.txt
 src/Subsearch.egg-info/top_level.txt
 src/subsearch/__init__.py
 src/subsearch/__main__.py
 src/subsearch/core.py
 src/subsearch/data/__init__.py
-src/subsearch/data/data_initializer.py
-src/subsearch/data/data_objects.py
+src/subsearch/data/constants.py
+src/subsearch/data/data_classes.py
 src/subsearch/data/guid.py
-src/subsearch/data/languages.json
+src/subsearch/data/language_data.toml
 src/subsearch/data/version.py
 src/subsearch/gui/__init__.py
-src/subsearch/gui/gui_toolkit.py
 src/subsearch/gui/resource_loader.py
 src/subsearch/gui/screen_manager.py
 src/subsearch/gui/system_tray.py
+src/subsearch/gui/utils.py
 src/subsearch/gui/resources/__init__.py
 src/subsearch/gui/resources/config.py
 src/subsearch/gui/resources/assets/__init__.py
 src/subsearch/gui/resources/assets/spritesheet.png
 src/subsearch/gui/resources/assets/subsearch.ico
 src/subsearch/gui/resources/styles/__init__.py
 src/subsearch/gui/resources/styles/sprites.tcl
 src/subsearch/gui/resources/styles/style_subsearch.tcl
 src/subsearch/gui/resources/styles/theme_setter.tcl
 src/subsearch/gui/screens/__init__.py
 src/subsearch/gui/screens/download_manager.py
 src/subsearch/gui/screens/language_options.py
-src/subsearch/gui/screens/search_filters.py
+src/subsearch/gui/screens/search_options.py
 src/subsearch/gui/screens/subsearch_options.py
 src/subsearch/providers/__init__.py
-src/subsearch/providers/generic.py
+src/subsearch/providers/core_provider.py
 src/subsearch/providers/opensubtitles.py
 src/subsearch/providers/subscene.py
 src/subsearch/providers/yifysubtitles.py
 src/subsearch/utils/__init__.py
-src/subsearch/utils/app_integrity.py
-src/subsearch/utils/debug.py
+src/subsearch/utils/decorators.py
 src/subsearch/utils/exceptions.py
-src/subsearch/utils/file_manager.py
 src/subsearch/utils/imdb_lookup.py
-src/subsearch/utils/io_json.py
+src/subsearch/utils/io_app.py
+src/subsearch/utils/io_file_system.py
+src/subsearch/utils/io_log.py
+src/subsearch/utils/io_toml.py
 src/subsearch/utils/io_winreg.py
-src/subsearch/utils/log.py
-src/subsearch/utils/mutex_synchronizer.py
-src/subsearch/utils/state_machine.py
+src/subsearch/utils/state_manager.py
 src/subsearch/utils/string_parser.py
 src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/__init__.py` & `Subsearch-2.38.0rc1/src/subsearch/gui/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 from tkinter import Tk
 
-from subsearch.data import app_paths
+from subsearch.data.constants import APP_PATHS
 
 
 def get_sprites() -> dict:
     pattern = r"\b(\w+)\s+(\d+)\s+(\d+)\s+(\d+)\s+(\d+)\b"
     data = {}
-    file_path = app_paths.gui_styles / "sprites.tcl"
+    file_path = APP_PATHS.gui_styles / "sprites.tcl"
     with file_path.open() as file:
         content = file.read()
         matches = re.findall(pattern, content)
 
         for match in matches:
             key = match[0]
             values = tuple(map(int, match[1:]))
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/gui_toolkit.py` & `Subsearch-2.38.0rc1/src/subsearch/utils/string_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,350 +1,356 @@
-import tkinter as tk
-from tkinter import Label, StringVar, ttk
+import re
+from typing import Any
 
-from subsearch.data import __version__, app_paths
-from subsearch.gui.resources import config as cfg
-from subsearch.utils import file_manager, io_json, io_winreg
+from num2words import num2words
 
-GWL_EXSTYLE = -20
-WS_EX_APPWINDOW = 0x00040000
-WS_EX_TOOLWINDOW = 0x00000080
+from subsearch.data.constants import VIDEO_FILE
+from subsearch.data.data_classes import (
+    AppConfig,
+    LanguageData,
+    ProviderUrls,
+    ReleaseData,
+)
+from subsearch.utils import imdb_lookup
 
-DEFAULT_LABEL_CONFIG = dict(bg=cfg.color.dark_grey, fg=cfg.color.white_grey, font=cfg.font.cas8b)
-DEFAULT_LABEL_GRID = dict(row=0, column=0, sticky="w", padx=2, pady=2)
-DEFAULT_BTN_TOGGLE_GRID = dict(row=0, column=2, pady=2)
 
-
-def calculate_btn_size(cls, width_=18, height_=2) -> tuple[int, int]:
+def find_year(string: str) -> int:
     """
-    Calculate the required size of a button based on its content.
+    Find and return the year from a string.
 
     Args:
-        cls: The class from which the method is being called.
-        width_ (optional): The initial width of the button before calculation. Defaults to 18.
-        height_ (optional): The initial height of the button before calculation. Defaults to 2.
+        string (str): The string where the year has to be looked for.
 
     Returns:
-        A tuple of integer values representing the calculated width and height of the button
+        int: The first 4 digit number that matches the regex pattern or 0000 if no match is found.
     """
-
-    generic_btn = tk.Button(cls, width=width_, height=height_)
-    x, y = generic_btn.winfo_reqwidth(), generic_btn.winfo_reqheight()
-    return x, y
+    re_year = re.findall("^.*\.([1-2][0-9]{3})\.", string)
+    if re_year:
+        year = re_year[0]
+        return int(year)
+    return 0000
 
 
-def calculate_checkbtn_size(cls, width_=16) -> int:
+def find_title_by_year(string: str) -> str:
     """
-    Calculates the required width of a ttk Checkbutton widget in pixels.
+    Find and return the title of a media file by year.
 
     Args:
-        cls (class): The parent class where the Checkbutton will be placed.
-        width_ (int, optional): The desired width of the ttk check button. Defaults to 16.
+        string (str): The file name.
 
     Returns:
-        int: The required width in pixels of a ttk Checkbutton based on its current settings.
+        str: The part of the file name before the year, with '.' replaced by ' ', or "" if no match is found.
+    """
+    re_title = re.findall("^(.*)\.[1-2][0-9]{3}\.", string)
+    if re_title:
+        title: str = re_title[0]
+        title = title.replace(".", " ")
+        return title
+    return ""
+
+
+def find_title_by_show(string: str) -> str:
     """
+    Find and return the title of a media file by show.
+
+    Args:
+        string (str): The file name.
 
-    generic_checkbtn = ttk.Checkbutton(cls, width=width_)
-    return generic_checkbtn.winfo_reqwidth()
+    Returns:
+        str: The part of the filename before the season and episode values, with '.' replaced by ' ', or "" if no match is found.
+    """
+    re_title = re.findall("^(.*)\.[s]\d*[e]\d*\.", string)
+    if re_title:
+        title: str = re_title[0]
+        title = title.replace(".", " ")
+        return title
+    return ""
 
 
-def set_default_grid_size(cls, width_=18) -> None:
+def find_season_episode(string: str) -> str:
     """
-    Set the default grid size for a tkinter GUI window.
+    Find and return the season and episode values of a media file.
 
     Args:
-        cls (object): The class object.
-        width_ (int, optional): The default width. Defaults to 18.
+        string (str): The file name.
 
     Returns:
-        None
+        str: A string consisting of the season and episode values formatted like "s01e01", or "" if no match is found.
+    """
+    re_se = re.findall("\.([s]\d*[e]\d*)\.", string)
+    if re_se:
+        se: str = re_se[0]
+        return se
+    return ""
+
+
+def convert_to_ordinal_string(string: str) -> tuple[str, str, str, str, bool]:
     """
-    btn_size = tk.Button(cls, width=width_, height=2)
-    x, _y = btn_size.winfo_reqwidth(), btn_size.winfo_reqheight()
-    col_count, row_count = cls.grid_size()
-    for col in range(col_count):
-        cls.grid_columnconfigure(col, minsize=x)
+    Converts the numeric TV series values (season and episode numbers) in a filename to their ordinal versions(if any).
 
-    for row in range(row_count):
-        cls.grid_rowconfigure(row, minsize=0)
+    Args:
+        string (str): The TV series values as pulled out from the filename as a single string, e.g., `s01e01`.
+
+    Returns:
+        tuple(str, str, str, str, bool): A tuple containing separated season and episode strings, corresponding ordinal
+            strings, and a Boolean flag indicating whether the input string was matched successfully.
+    """
+    if string == "":
+        season, season_ordinal, episode, episode_ordinal = "", "", "", ""
+        show_bool = False
+    else:
+        season, episode = string.replace("s", "").replace("e", " ").split(" ")
+        season_ordinal = num2words(int(season), lang="en", to="ordinal")
+        episode_ordinal = num2words(int(episode), lang="en", to="ordinal")
+        show_bool = True
+    return season, season_ordinal, episode, episode_ordinal, show_bool
 
 
-class WindowPosition(tk.Frame):
+def find_group(string: str) -> str:
     """
-    A class that creates and manages the positioning of a tkinter frame.
+    Find and return the group from a string.
 
     Args:
-        parent: The parent widget.
+        string (str): The string where the group has to be looked for.
 
-    Attributes:
-        None
+    Returns:
+        str: The group identifier as taken from the end of the string.
+    """
+    group = string.rsplit("-", 1)[-1]
+    return group
+
+
+def find_title(filename: str, year: int, series: bool):
+    """
+    Find and return the media file's title, taking its year and/or TV series values into consideration.
 
-    Methods:
-        set(w=int, h=int, ws_value_offset=int, hs_value_offset=int, other=bool): Sets the window dimension
-            in width and height. It also sets offsets by which to move the window horizontally (ws_value_offset)
-            and vertically (hs_value_offset). If other=True, it allows changing other dimensions not typically
-            touched (eg. height of frame/window title bar)
+    Args:
+        filename (str): The name of the media file.
+        year (int): The relevant year, extracted from the name, passed on from another method.
+        series (bool): Whether the video file is a TV series or not.
 
     Returns:
-       None
+        str: The name of the given media file.
     """
+    if year != 0000:
+        title = find_title_by_year(filename)
+    elif series and year == 0000:
+        title = find_title_by_show(filename)
+    else:
+        title = filename.rsplit("-", 1)[0]
+    return title
 
-    def __init__(self, parent) -> None:
+
+class CreateProviderUrls:
+    def __init__(self, app_config: AppConfig, release_data: ReleaseData, language_data: dict[str, Any]):
         """
-        Constructor Method for WindowPosition Class
+        Initializes a new instance of the CreateProviderUrls class.
 
         Args:
-            parent: The parent widget.
+            app_config (AppConfig): The application configuration
+            release_metadata (ReleaseMetadata): The release metadata
         """
-        tk.Frame.__init__(self, parent)
+        self.app_config = app_config
+        self.release_data = release_data
+        self.language_data = language_data
+        self.current_language_data: LanguageData = LanguageData(**language_data[app_config.language])
 
-    def set(
-        self,
-        w=cfg.size.width,
-        h=cfg.size.height,
-        ws_value_offset=0,
-        hs_value_offset=0,
-        other: bool = False,
-    ):
+    def retrieve_urls(self) -> ProviderUrls:
         """
-        Set the size of the current window/Frame
-
-        Args:
-             w: An optional integer for setting the width of the window/frame
-             h: An optional integer for setting the height of the window/frame
-             ws_value_offset: An optional integer for setting the horizontal offset of the window/frame
-             hs_value_offset: An optional integer for setting the vertical offset of the window/frame
-             other: An optional bool variable to allow changing other dimensions not typically touched
-                    eg. height of frame/window title bar
+        Get the provider urls to search for subtitles.
 
         Returns:
-              None
+            ProviderUrls: A collection of strings that contains urls to search for subtitles from different subtitle providers.
         """
-        ws = self.winfo_screenwidth() + ws_value_offset
-        hs = self.winfo_screenheight() + hs_value_offset
-        x = int((ws / 2) - (w / 2))
-        y = int((hs / 2) - (h / 2))
-        value = f"{w}x{h}+{x}+{y}"
-        if other:
-            return w, h, x, y
-        return value
-
-
-class VarColorPicker:
-    """
-    A class that initializes a color picker for given string variables.
+        return ProviderUrls(self.subscene(), self.opensubtitles(), self.opensubtitles_hash(), self.yifysubtitles())
 
-    Args:
-        string_var: A tkinter StringVar object to represent value of the color.
-        clabel: A tkinter Label object to represent the color label.
-        is_pct: A boolean variable initialized to False indicating if configured level in percentage.
-
-    Attributes:
-        string_var: A tkinter StringVar object representing value of the color.
-        clabel: A tkinter Label object representing the color label.
-        is_pct: A boolean variable to determine percentage threshold.
-
-    Methods:
-        pick(): Method to determine and update the color of clabel based on the string_var value.
-    """
-
-    def __init__(self, string_var: StringVar, clabel: Label, is_pct: bool = False):
-        self.string_var = string_var
-        self.clabel = clabel
-        self.is_pct = is_pct
-        self.pick()
-
-    def pick(self) -> None:
-        if self.string_var.get() == "True":
-            self.clabel.configure(fg=cfg.color.green)
-        elif self.string_var.get() == "False":
-            self.clabel.configure(fg=cfg.color.red)
-        elif self.string_var.get() == "Both":
-            self.clabel.configure(fg=cfg.color.blue)
-        elif self.string_var.get().startswith("Only"):
-            self.clabel.configure(fg=cfg.color.green)
-
-        if self.is_pct:
-            _pct = io_json.get_json_key("percentage_threshold")
-            if _pct in range(75, 101):
-                self.clabel.configure(fg=cfg.color.green)
-            elif _pct in range(50, 75):
-                self.clabel.configure(fg=cfg.color.green_brown)
-            elif _pct in range(25, 50):
-                self.clabel.configure(fg=cfg.color.red_brown)
-            elif _pct in range(0, 25):
-                self.clabel.configure(fg=cfg.color.red)
-
-
-class ToolTip(tk.Toplevel):
-    """
-    A toplevel widget that displays a message when the user hovers over a specified widget
+    def subscene(self) -> str:
+        """
+        Gets the Url for the Subscene website to search for subtitles.
 
-    Args:
-        parent (tkinter.Tk): The parent widget
-        _widget (tkinter.Widget): The widget to attach the tooltip to
-        *_text (str): The text to be displayed in the tooltip
-        _background (str): The background color of the tooltip
-
-    Methods:
-        show(): Creates and displays a toplevel widget containing the text to be displayed in the tooltip
-    """
-
-    def __init__(self, parent, _widget, *_text, _background=cfg.color.light_black):
-        self.parent = parent
-        self.widget = _widget
-        self.text = _text
-        self.background = _background
-
-    def show(self) -> None:
-        tk.Toplevel.__init__(self, self.parent)
-        self.configure(background=cfg.color.light_black)
-        # remove the standard window titlebar from the tooltip
-        self.overrideredirect(True)
-        # unpack *args and put each /n on a new line
-        lines = "\n".join(self.text)
-        frame = tk.Frame(self, background=cfg.color.light_black)
-        label = tk.Label(
-            frame,
-            text=lines,
-            background=self.background,
-            foreground=cfg.color.white_grey,
-            justify="left",
-        )
-        # get size of the label to use later for positioning and sizing of the tooltip
-        x, y = label.winfo_reqwidth(), label.winfo_reqheight()
-        # set the size of the tooltip background to be 1px larger than the label
-        frame.configure(width=x + 1, height=y + 1)
-
-        widget_pos = self.widget.winfo_rootx()
-        widget_width = self.widget.winfo_reqwidth()
-        widget_center = round(widget_width / 2)
-        btn_pos_middle = widget_pos + widget_center
-        frame_width = frame.winfo_reqwidth()
-        frame_center = round(frame_width / 2)
-        center_tip_over_mouse = btn_pos_middle - frame_center
-        # offset the frame 1px from edge of the tooltip corner
-        frame.place(x=1, y=1, anchor="nw")
-        label.place(x=0, y=0, anchor="nw")
-        root_x = center_tip_over_mouse  # offset the tooltip by extra 4px so it doesn't overlap the widget
-        root_y = self.widget.winfo_rooty() - self.widget.winfo_height() - 4
-        # set position of the tooltip, size and add 2px around the tooltip for a 1px border
-        self.geometry(f"{x+2}x{y+2}+{root_x}+{root_y}")
+        Returns:
+            str: The url to search for subtitles on subscene.com
+        """
+        domain = "https://subscene.com"
+        query = "subtitles/searchbytitle?query"
+        search_parameters = self._subscene_search_parameters()
+        url_subscene = f"{domain}/{query}={search_parameters}"
+        return url_subscene.replace(" ", "%20")
 
-    def hide(self) -> None:
-        self.destroy()
+    def opensubtitles(self) -> str:
+        """
+        Gets the Url for the Opensubtitles website to search for subtitles.
 
+        Returns:
+            str: The url to search for subtitles on opensubtitles.org
+        """
+        domain = "https://www.opensubtitles.org"
+        subtitle_type = self._opensubtitles_subtitle_type()
+        search_parameters = self._opensubtitles_search_parameters()
+        return f"{domain}/{subtitle_type}/{search_parameters}/rss_2_00".replace(" ", "%20")
 
-class ToggleableFrameButton(tk.Frame):
-    """
-    A button that toggles a configuration setting on or off.
+    def opensubtitles_hash(self) -> str:
+        """
+        Gets the Url to set a moviehash for the Opensubtitles website to find subtitles.
 
-    Args:
-        parent (tk.Widget): The parent widget.
-        setting_label (str): Name of the setting to be displayed.
-        config_key (str): Key in the configuration file where the state is stored.
-        write_to_reg (bool, optional): Whether to also write the state to registry. Defaults to False.
-        show_if_exe (bool, optional): Only show the button if the program is not running from an executable. Defaults to True.
-    """
-
-    def __init__(self, parent, setting_label: str, config_key: str, **kwargs) -> None:
-        tk.Frame.__init__(self, parent)
-        self.configure(bg=cfg.color.dark_grey)
-        self.string_var = tk.StringVar()
-        self.string_var.set(f"{io_json.get_json_key(config_key)}")
-        self.setting_name = setting_label
-        self.config_key = config_key
-        self.write_to_reg = kwargs.get("write_to_reg", False)
-        self.show_if_exe = kwargs.get("write_to_reg", True)
-        self.tip_text = kwargs.get("tip_text", None)
-        self.tip_present = False
-        if self.show_if_exe is False and file_manager.running_from_exe():
-            return None
-        label = tk.Label(self, text=self.setting_name)
-        label.configure(DEFAULT_LABEL_CONFIG)
-        label.grid(DEFAULT_LABEL_GRID)
-        btn_toggle = ttk.Button(
-            self,
-            textvariable=self.string_var,
-            width=40,
-            style=f"{self.string_var.get()}.TButton",
-        )
-        btn_toggle.grid(DEFAULT_BTN_TOGGLE_GRID, padx=8)
-        btn_toggle.bind("<Enter>", self.enter_button)
-        btn_toggle.bind("<Leave>", self.leave_button)
-        set_default_grid_size(self)
+        Returns:
+            str: the url to set moviehash for opensubtitles.org
+        """
+        domain = "https://www.opensubtitles.org"
+        subtitle_type = self._opensubtitles_subtitle_type()
+        return f"{domain}/{subtitle_type}/moviehash-{VIDEO_FILE.file_hash}"
 
-    def enter_button(self, event) -> None:
+    def yifysubtitles(self) -> str:
         """
-        Function called when the mouse enters the button area.
+        Gets the Url for the YifySubtitles website to search for subtitles for movies.
 
-        Args:
-            event: The tkinter event object.
+        Returns:
+            str: The url to search for subtitles on yifysubtitles.org
         """
-        btn = event.widget
-        if btn["text"] == "True":
-            btn.bind("<ButtonRelease-1>", self.button_set_false)
-        if btn["text"] == "False":
-            btn.bind("<ButtonRelease-1>", self.button_set_true)
-        if self.tip_text is not None and self.tip_present is False:
-            self.tip = ToolTip(btn, btn, self.tip_text)
-            self.tip.show()
-            self.tip_present = True
+        if self.release_data.tvseries:
+            return ""
+        domain = "https://yifysubtitles.org"
+        tt_id = imdb_lookup.FindImdbID(self.release_data.title, self.release_data.year).id
+        return f"{domain}/movie-imdb/{tt_id}" if tt_id is not None else ""
 
-    def leave_button(self, event) -> None:
+    def _subscene_search_parameters(self) -> str:
         """
-        Function called when the mouse leaves the button area.
+        Gets the search parameters for Subscene to search for the appropriate subtitles based on File name and season ordinal.
 
-        Args:
-            event: The tkinter event object.
+        Returns:
+            str: The search parameter value for Subscene to search for the applicable subtitles.
         """
-        btn = event.widget
-        if self.tip_present:
-            self.tip.hide()
-            self.tip_present = False
+        if self.release_data.tvseries:
+            return f"{self.release_data.title} - {self.release_data.season_ordinal} season"
+        return f"{self.release_data.title}"
 
-    def button_set_true(self, event) -> None:
+    def _opensubtitles_subtitle_type(self) -> str:
         """
-        Function called when the button is set to True.
+        Gets the subtitle type and language settings for Opensubtitles based on Application configuration.
 
-        Args:
-            event: The tkinter event object.
+        Returns:
+            str: The subtitle types and language configurations to search for subtitles in Opensubtitles.
         """
-        btn = event.widget
-        self.string_var.set(f"True")
-        btn["style"] = f"{self.string_var.get()}.TButton"
-        io_json.set_config_key_value(self.config_key, True)
-        if self.write_to_reg:
-            io_winreg.add_context_menu()
-            io_winreg.write_all_valuex()
-        self.enter_button(event)
+        alpha_2b = self.current_language_data.alpha_2b
+        if self.app_config.hearing_impaired and self.app_config.non_hearing_impaired is False:
+            return f"en/search/sublanguageid-{alpha_2b}/hearingimpaired-on"
+        return f"en/search/sublanguageid-{alpha_2b}"
 
-    def button_set_false(self, event) -> None:
+    def _opensubtitles_search_parameters(self) -> str:
         """
-        Function called when the button is set to False.
+        Gets the search parameters for Opensubtitles to search for the appropriate subtitles based on Movie title, year, season and episode number.
 
-        Args:
-            event: The tkinter event object.
+        Returns:
+            str: The search parameter value for Opensubtitles to search for the applicable subtitles.
         """
-        btn = event.widget
-        self.string_var.set(f"False")
-        btn["style"] = f"{self.string_var.get()}.TButton"
-        io_json.set_config_key_value(self.config_key, False)
-        if self.write_to_reg:
-            io_winreg.remove_context_menu()
-        self.enter_button(event)
+        if self.release_data.tvseries:
+            return f"searchonlytvseries-on/season-{self.release_data.season}/episode-{self.release_data.episode}/moviename-{self.release_data.title}"
+        return f"searchonlymovies-on/moviename-{self.release_data.title} ({self.release_data.year})"
 
 
-def configure_root(root):
+def get_release_data(filename: str) -> ReleaseData:
     """
-    Initialize the root Tkinter window for the Subsearch application.
+    Collects the necessary data from a filename.
+
+    Args:
+      filename (str): The name of the file to obtain release metadata from.
+
+    Returns:
+      ReleaseMetadata: A ReleaseMetadata object containing the relevant metadata for the inputted file.
+
+    """
+    release = filename.lower()
+    year = find_year(release)
+    season_episode = find_season_episode(release)
+    season, season_ordinal, episode, episode_ordinal, series = convert_to_ordinal_string(season_episode)
+
+    title = find_title(release, year, series)
+    group = find_group(release)
+
+    parameters = ReleaseData(
+        title,
+        year,
+        season,
+        season_ordinal,
+        episode,
+        episode_ordinal,
+        series,
+        release,
+        group,
+    )
+    return parameters
+
+
+def calculate_match(from_user: str, from_website: str) -> int:
+    """
+    Calculates the match between user input and website information
+
+    Args:
+        from_user (str): User input string
+        from_website (str): Website information string
 
     Returns:
-        tk.Tk: The initialized Tkinter root window.
+        int: The percentage of matching between two strings.
     """
-    if io_json.get_json_key("context_menu"):
-        io_winreg.add_context_menu()
-    root.configure(background=cfg.color.dark_grey)
-    root.iconbitmap(app_paths.gui_assets / "subsearch.ico")
-    root.geometry(WindowPosition.set(root))  # type: ignore
-    root.resizable(False, False)
+    max_percentage = 100
+    _from_user: list[str] = mk_lst(from_user)
+    _from_website: list[str] = mk_lst(from_website)
+    lst1, lst2 = make_equal_size(_from_user, _from_website)
+    not_matching = list(set(lst1) - set(lst2))
+    not_matching_value = len(not_matching)
+    number_of_items = len(lst1)
+    percentage_to_remove = round(not_matching_value / number_of_items * max_percentage)
+    pct = round(max_percentage - percentage_to_remove)
+
+    return pct
+
+
+def mk_lst(release: str) -> list[str]:
+    new: list[str] = []
+    qualities = ["720p", "1080p", "1440p", "2160p"]
+    temp = release.split(".")
+
+    for item in temp:
+        if item not in qualities:
+            new.append(item.lower())
+    return new
+
+
+def make_equal_size(lst1, lst2):
+    if len(lst1) == len(lst2):
+        return lst1, lst2
+    elif len(lst1) > len(lst2):
+        lst_big, lst_small = lst1, lst2
+    else:
+        lst_big, lst_small = lst2, lst1
+
+    num_big, num_small = sorted((len(lst1), len(lst2)), reverse=True)
+    difference = num_big - num_small
+    filled_list = fill_shorter_list(lst_big, lst_small, difference)
+    return lst_big, filled_list
+
+
+def fill_shorter_list(big_lst, small_lst, difference):
+    if big_lst > small_lst:
+        for _i in range(difference):
+            small_lst.append(None)
+    return small_lst
+
+
+def valid_filename(input_string) -> bool:
+    forbidden_characters_pattern = r'[<>:"/\\|?*\x00]'
+    return bool(re.search(forbidden_characters_pattern, input_string))
+
+
+def fix_filename(input_string) -> str:
+    forbidden_characters_pattern = r'[<>:"/\\|?*\x00]'
+    return re.sub(forbidden_characters_pattern, ".", input_string)
+
+
+def valid_path(input_str, path_resolution) -> bool:
+    if input_str == "":
+        return False
+    if path_resolution == "relative":
+        pattern = r"^\.{1,2}\\([a-z0-9-_]|\\[a-z0-9-_])+$|^\.{1,2}$"
+    elif path_resolution == "absolute":
+        pattern = r"^[a-zA-Z]{1}:\\([a-z0-9-_]|\\[a-z0-9-_])+$"
+    return bool(re.match(pattern, input_str))
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/resources/assets/subsearch.ico` & `Subsearch-2.38.0rc1/src/subsearch/gui/resources/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.1/src/subsearch/gui/resources/config.py` & `Subsearch-2.38.0rc1/src/subsearch/gui/resources/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         blue: #81a2be
         cyan: #82b3ac
         green: #9fa65d
         green_brown: #a59256
         grey: #4c4c4c
         light_grey: #727272
         silver_grey: #8a8a8a
-        white_grey: #bdbdbd
-        dark_grey: #1a1b1b
-        mid_grey_black: #111111
+        default_fg: #bdbdbd
+        default_bg: #1a1b1b
+        default_bg_dark: #111111
         light_black: #0e0e0e
         black: #151515
         dark_black: #000000
     """
 
     purple: str = "#b294bb"
     red: str = "#bc473b"
@@ -61,17 +61,17 @@
     blue: str = "#81a2be"
     cyan: str = "#82b3ac"
     green: str = "#9fa65d"
     green_brown: str = "#a59256"
     grey: str = "#4c4c4c"
     light_grey: str = "#727272"
     silver_grey: str = "#8a8a8a"
-    white_grey: str = "#bdbdbd"
-    dark_grey: str = "#1a1b1b"
-    mid_grey_black: str = "#111111"
+    default_fg: str = "#bdbdbd"
+    default_bg: str = "#1a1b1b"
+    default_bg_dark: str = "#111111"
     light_black: str = "#0e0e0e"
     black: str = "#151515"
     dark_black: str = "#000000"
 
 
 @dataclass(order=True, frozen=True)
 class Font:
@@ -97,7 +97,12 @@
     cas20b: str = "Cascadia 20 bold"
 
 
 size = Size()
 position = Position()
 font = Font()
 color = Color()
+
+
+DEFAULT_LABEL_CONFIG = dict(bg=color.default_bg, fg=color.default_fg, font=font.cas8b)
+DEFAULT_LABEL_GRID = dict(row=0, column=0, sticky="w", padx=2, pady=2)
+DEFAULT_BTN_TOGGLE_GRID = dict(row=0, column=2, pady=2)
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/resources/styles/sprites.tcl` & `Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/sprites.tcl`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 set ::sprite_data [list \
   download_manager_hover 0 0 51 41 \
   download_manager_press 0 41 51 41 \
   download_manager_rest 51 0 51 41 \
   language_options_hover 51 41 51 41 \
   language_options_press 0 82 51 41 \
   language_options_rest 51 82 51 41 \
-  search_filters_hover 102 0 51 41 \
-  search_filters_press 102 41 51 41 \
-  search_filters_rest 102 82 51 41 \
+  search_options_hover 102 0 51 41 \
+  search_options_press 102 41 51 41 \
+  search_options_rest 102 82 51 41 \
   subsearch_options_hover 0 123 51 41 \
   subsearch_options_press 51 123 51 41 \
   subsearch_options_rest 102 123 51 41 \
   card 153 0 50 50 \
   btn_disabled 153 50 22 35 \
   btn_hover 175 50 22 35 \
   btn_pressed 153 85 22 35 \
@@ -35,14 +35,19 @@
   check_unsel_hover 60 186 20 20 \
   check_unsel_pressed 80 186 20 20 \
   check_unsel_rest 100 184 20 20 \
   scroll_hor_thumb 120 184 20 12 \
   scroll_hor_trough 140 184 20 12 \
   scroll_vert_thumb 160 184 10 20 \
   scroll_vert_trough 170 184 12 20 \
+  textbox_dis 182 184 20 20 \
+  textbox_error 188 164 20 20 \
+  textbox_focus 203 0 20 20 \
+  textbox_hover 203 20 20 20 \
+  textbox_rest 203 40 20 20 \
   sizegrip 120 196 10 10 \
   scroll_down 130 196 8 6 \
   scroll_left 197 50 6 8 \
   scroll_right 197 58 6 8 \
   scroll_up 138 196 8 6 \
   separator 88 184 1 1 \
 ]
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/resources/styles/style_subsearch.tcl` & `Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/style_subsearch.tcl`

 * *Files 10% similar despite different names*

```diff
@@ -141,25 +141,39 @@
         ttk::style layout TLabelframe {
         Labelframe.border {
             Labelframe.padding -expand 1 -children {
             Labelframe.label -side left
                 }
             }
         
+        
         }
-        # Labelframe
+        # LabelframePlain
         ttk::style layout TLabelframePlain {
         Labelframe.plain {
             Labelframe.padding -expand 1 -children {
             Labelframe.label -side left
                 }
             }
         
         }
 
         ttk::style element create Labelframe.border image $sprites(card) -border 5 -padding 4 -sticky nsew
         ttk::style configure TLabelframe.border.Label -font "Cascadia 8 bold" -foreground $colors(-fg) -background $colors(-bg)
         ttk::style configure TLabelframe.plain.Label -font "Cascadia 8 bold" -foreground $colors(-fg) -background $colors(-bg)
 
+        # Entry
+        ttk::style configure TEntry -foreground $colors(-fg) -padding {6 1 4 2}
+        ttk::style map TEntry -foreground [list disabled "#757575" pressed "#cfcfcf"]
+
+        ttk::style element create Entry.field image \
+        [list $sprites(textbox_rest) \
+            {focus hover !invalid} $sprites(textbox_focus) \
+            invalid $sprites(textbox_error) \
+            disabled $sprites(textbox_dis) \
+            {focus !invalid} $sprites(textbox_focus) \
+            hover $sprites(textbox_hover) \
+        ] -border 5 -sticky nsew
+
 
     }
 }
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/resources/styles/theme_setter.tcl` & `Subsearch-2.38.0rc1/src/subsearch/gui/resources/styles/theme_setter.tcl`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     
     ttk::style theme use "style_subsearch"
 
     array set colors {
         -fg             "#bdbdbd"
         -bg             "#1a1b1b"
         -disabledfg     "#59959"
-        -selectfg       "#ffffff"
-        -selectbg       "#2f60d8"
+        -selectfg       "#1a1b1b"
+        -selectbg       "#bdbdbd"
     }
     
     ttk::style configure . \
         -background $colors(-bg) \
         -foreground $colors(-fg) \
         -troughcolor $colors(-bg) \
         -focuscolor $colors(-selectbg) \
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/screen_manager.py` & `Subsearch-2.38.0rc1/src/subsearch/gui/screen_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import tkinter as tk
 from typing import Any
 
 from subsearch.data import __version__
-from subsearch.data.data_objects import PrettifiedDownloadData
-from subsearch.gui import gui_toolkit, resource_loader, root
+from subsearch.data.data_classes import Subtitle
+from subsearch.gui import resource_loader, root, utils
 from subsearch.gui.resources import config as cfg
 from subsearch.gui.screens import (
     download_manager,
     language_options,
-    search_filters,
+    search_options,
     subsearch_options,
 )
 
 
 class ScreenManager(tk.Frame):
     """
     A class used to manage the screens of a parent widget.
@@ -36,18 +36,18 @@
         enter_tab(event): Called when mouse enters a screen button. Bind '<ButtonPress>' event to the button widget.
         leave_tab(event):  Called when mouse leaves a screen button. Unbind '<ButtonPress>' event from the button widget, and call 'activate_screens()' and 'deactivate_screens()' methods.
         get_btn(dict_, event_, equals=True): Helper method to retrieve the button widget and its key.
     """
 
     def __init__(self, parent, available_screens: dict[str, Any], active_screen: str) -> None:
         tk.Frame.__init__(self, parent)
-        self.configure(bg=cfg.color.mid_grey_black, width=cfg.size.width, height=82)
+        self.configure(bg=cfg.color.default_bg_dark, width=cfg.size.width, height=82)
         relx_value = 0.0
         btn_kwargs: dict[str, Any] = dict(
-            master=self, width=54, height=54, bg=cfg.color.mid_grey_black, highlightthickness=0
+            master=self, width=54, height=54, bg=cfg.color.default_bg_dark, highlightthickness=0
         )
         self.parent = parent
         self.available_screens = available_screens
         self.buttons = {}
 
         for tab_key in available_screens.keys():
             self.buttons[tab_key] = tk.Canvas(**btn_kwargs)
@@ -55,15 +55,14 @@
         for btn_key, btn_widget in self.buttons.items():
             relx_value += 0.2
             btn_widget.place(relx=relx_value, rely=0.5, anchor="center")
             btn_widget.bind("<Enter>", self.enter_menu_btn)
             btn_widget.bind("<Leave>", self.leave_menu_btn)
             resource_loader.asset_menu_btn(btn_widget, btn_key, "rest")
 
-        gui_toolkit.set_default_grid_size(self)
         self.active_screen = active_screen
         self.activate_screen()
 
     def activate_screen(self) -> None:
         self.available_screens[self.active_screen].place(x=cfg.position.screen_x, y=cfg.position.screen_y, anchor="center")
         resource_loader.asset_menu_btn(self.buttons[self.active_screen], self.active_screen, "press")
         title_tab = self.active_screen.capitalize().replace("_", " ")
@@ -106,65 +105,72 @@
             if event_.widget == btn_widget and not equals:
                 return btn_key, btn_widget
 
 
 class LanguageOptions(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent, width=cfg.size.width, height=cfg.size.height)
-        self.configure(bg=cfg.color.dark_grey)
+        self.configure(bg=cfg.color.default_bg)
         language_options.SelectLanguage(self).pack(anchor="center", expand=True)
 
 
-class SearchFilters(tk.Frame):
+class SearchOptions(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent, width=cfg.size.width, height=cfg.size.height)
-        self.configure(bg=cfg.color.dark_grey)
-        group_a = tk.Frame(self, bg=cfg.color.dark_grey)
+        self.configure(bg=cfg.color.default_bg)
+        group_a = tk.Frame(self, bg=cfg.color.default_bg)
         group_a.pack(anchor="center", expand=True, fill="both")
-        search_filters.Providers(group_a).pack(side=tk.RIGHT, anchor="center", expand=True, fill="both", padx=2)
-        search_filters.SubtitleOptions(group_a).pack(side=tk.LEFT, anchor="center", expand=True, fill="both", padx=2)
-        tk.Frame(self, height=80, bg=cfg.color.dark_grey).pack(anchor="center", expand=True)
-        search_filters.SearchThreshold(self).pack(anchor="center")
+        search_options.SubtitleFilters(group_a).pack(side=tk.LEFT, anchor="center", expand=True, fill="both", padx=2)
+        search_options.Providers(group_a).pack(side=tk.LEFT, anchor="center", expand=True, fill="both", padx=2)
+        tk.Frame(self, height=30, bg=cfg.color.default_bg).pack(anchor="center", expand=True)
+        search_options.SubtitlePostProcessing(self).pack(anchor="center", expand=True, fill="x")
+        search_options.SubtitlePostProcessingDirectory(self).pack(anchor="center", expand=True, fill="x")
+        tk.Frame(self, height=60, bg=cfg.color.default_bg).pack(anchor="center", expand=True)
+        search_options.SearchThreshold(self).pack(anchor="center")
 
 
 class SubsearchOptions(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent, width=cfg.size.width, height=cfg.size.height)
-        self.configure(bg=cfg.color.dark_grey)
+        self.configure(bg=cfg.color.default_bg)
         subsearch_options.FileExtensions(self).pack(anchor="center", fill="x")
-        tk.Frame(self, height=40, bg=cfg.color.dark_grey).pack(anchor="center", expand=True)
+        tk.Frame(self, height=40, bg=cfg.color.default_bg).pack(anchor="center", expand=True)
         subsearch_options.SubsearchOption(self).pack(anchor="center", fill="x")
-        tk.Frame(self, height=80, bg=cfg.color.dark_grey).pack(anchor="center", expand=True)
+        tk.Frame(self, height=80, bg=cfg.color.default_bg).pack(anchor="center", expand=True)
         subsearch_options.CheckForUpdates(self)
 
 
 class DownloadManager(tk.Frame):
-    def __init__(self, parent, formatted_data: list[PrettifiedDownloadData]) -> None:
+    def __init__(self, parent, subtitles: list[Subtitle]) -> None:
         tk.Frame.__init__(self, parent, width=cfg.size.width, height=cfg.size.height)
-        self.configure(bg=cfg.color.dark_grey)
-        download_manager.DownloadList(self, formatted_data).pack(anchor="center")
+        self.configure(bg=cfg.color.default_bg)
+        download_manager.DownloadManager(self, subtitles).pack(anchor="center")
 
 
 def open_screen(tab_name: str, **kwargs) -> None:
     """
     Opens a new screen depending on the tab_name argument passed in.
 
     Args:
         tab_name (str): A string representing which screen to activate.
 
     Returns:
         None: This function does not return anything, it manipulates the GUI instead.
     """
-
-    data: list | list[PrettifiedDownloadData] = kwargs.get("data", [])
-    gui_toolkit.configure_root(root)
+    root.bind("<KeyPress>", close_mainloop)
+    subtitles: list | list[Subtitle] = kwargs.get("subtitles", [])
+    utils.configure_root(root)
     resource_loader.set_ttk_theme(root)
-    resource_loader.set_custom_btn_styles()
     screens = {
         "language_options": LanguageOptions(root),
-        "search_filters": SearchFilters(root),
+        "search_options": SearchOptions(root),
         "subsearch_options": SubsearchOptions(root),
-        "download_manager": DownloadManager(root, data),
+        "download_manager": DownloadManager(root, subtitles),
     }
     manager = ScreenManager(root, screens, tab_name.lower())
     manager.place(y=cfg.size.height - 82)
     root.mainloop()
+
+
+def close_mainloop(event):
+    if event.keysym == "Escape":
+        root.quit()
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/screens/language_options.py` & `Subsearch-2.38.0rc1/src/subsearch/gui/screens/language_options.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import tkinter as tk
 from tkinter import IntVar, ttk
 
-from subsearch.gui import gui_toolkit
-from subsearch.utils import io_json
+from subsearch.data.constants import FILE_PATHS
+from subsearch.gui import utils
+from subsearch.utils import io_toml
 
 
 class SelectLanguage(ttk.Labelframe):
     def __init__(self, parent) -> None:
         ttk.Labelframe.__init__(self, parent)
         self.configure(text="Languages", padding=10)
         self.active_btn = None
         self.rownum = 0
         self.colnum = 1
         self.checkbox_values = {}
         self.name_find_key = {}
         self.tip_present = False
-        self.languages = io_json.get_available_languages()
-        self.current_language = io_json.get_json_key("current_language")
+        self.languages = io_toml.load_toml_data(FILE_PATHS.language_data)
+        self.current_language = io_toml.load_toml_value(FILE_PATHS.config, "subtitle_filters.language")
         self.checkbuttons: dict[ttk.Checkbutton, IntVar] = {}
         frame = None
         for enum, (language, language_data) in enumerate(self.languages.items()):
             if enum % 14 == 0:
                 frame = ttk.Frame(self)
                 frame.pack(side=tk.LEFT, anchor="n")
 
@@ -38,19 +39,19 @@
 
             btn.bind("<Enter>", self.enter_button)
             btn.bind("<Leave>", self.leave_button)
             self.name_find_key[language_data["name"]] = language
 
     def enter_button(self, event) -> None:
         btn = event.widget
-        json_key = self.name_find_key[btn["text"]]
-        providers = ", ".join(([_i.title() for _i in self.languages[json_key]["incompatibility"]]))
+        toml_key = self.name_find_key[btn["text"]]
+        providers = ", ".join(([_i.title() for _i in self.languages[toml_key]["incompatibility"]]))
         if providers:
             tip_text = f"If enabled, '{providers}' will be automatically skipped."
-            self.tip = gui_toolkit.ToolTip(btn, btn, tip_text)
+            self.tip = utils.ToolTip(btn, btn, tip_text)
             self.tip.show()
             self.tip_present = True
         btn.bind("<ButtonPress-1>", self.press_button)
 
     def leave_button(self, event) -> None:
         btn = event.widget
         if self.tip_present:
@@ -62,9 +63,9 @@
         btn.bind("<ButtonRelease-1>", self.set_current_language)
 
     def set_current_language(self, event) -> None:
         btn = event.widget
         self.checkbox_values[self.active_btn].set(0)  # type: ignore
         self.active_btn.state(["!alternate"])  # type: ignore
         self.active_btn = btn
-        json_key = self.name_find_key[btn["text"]]
-        io_json.set_config_key_value("current_language", json_key)
+        value = self.name_find_key[btn["text"]]
+        io_toml.update_toml_key(FILE_PATHS.config, "subtitle_filters.language", value)
```

### Comparing `Subsearch-2.37.1/src/subsearch/gui/screens/search_filters.py` & `Subsearch-2.38.0rc1/src/subsearch/gui/screens/subsearch_options.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,206 +1,233 @@
 import tkinter as tk
-from tkinter import ttk
-from typing import Any, Iterable
+import webbrowser
+from tkinter import BooleanVar, ttk
+from typing import Any
 
-from subsearch.gui import gui_toolkit
+from subsearch.data import __version__
+from subsearch.data.constants import DEVICE_INFO, FILE_PATHS
 from subsearch.gui.resources import config as cfg
-from subsearch.utils import io_json
+from subsearch.utils import decorators, io_toml, io_winreg, update
 
 
-class Providers(ttk.Labelframe):
+class FileExtensions(ttk.Labelframe):
+    instances: list["FileExtensions"] = []
+
     def __init__(self, parent) -> None:
         ttk.Labelframe.__init__(self, parent)
-        self.configure(text="Search providers", padding=10)
-        self.providers = io_json.get_json_key("providers")
-        self.data = io_json.get_json_data()
-        self.chekboxes = {}
-        self.last_key = ""
+        self.configure(text="File Exstensions", padding=10)
+        FileExtensions.instances.append(self)
+        self.data = io_toml.load_toml_data(FILE_PATHS.config)
+        self.file_extensions = io_toml.load_toml_value(FILE_PATHS.config, "file_extensions")
+
+        self.checkbuttons: dict[ttk.Checkbutton, tuple[str, BooleanVar]] = {}
+
         frame = None
-        for enum, (key, value) in enumerate(self.providers.items()):
+        for enum, (key, value) in enumerate(self.file_extensions.items()):
             if enum % 4 == 0:
-                frame = tk.Frame(self)
-                frame.pack(side=tk.LEFT, anchor="n", expand=True)
-            provider_type = key.split("_")[-1].lower()
-            provider = f"{key.split('_')[0]}".capitalize()
+                frame = ttk.Frame(self)
+                frame.pack(side=tk.LEFT, anchor="n")
+
             boolean = tk.BooleanVar()
             boolean.set(value)
-            btn = ttk.Checkbutton(frame, text=f"{provider} {provider_type}", onvalue=True, offvalue=False, variable=boolean)
-            btn.pack(padx=4, pady=4, ipadx=60)
-            self.chekboxes[btn] = key, boolean
-            if self.data["providers"][key] is True:
-                btn.configure(state="normal")
+            check_btn = ttk.Checkbutton(frame, text=key, onvalue=True, offvalue=False, variable=boolean)
+            if not io_toml.load_toml_value(FILE_PATHS.config, "gui.context_menu"):
+                check_btn.state(["disabled"])
 
-            btn.bind("<Enter>", self.enter_button)
-            btn.bind("<Leave>", self.leave_button)
+            check_btn.pack(padx=4, pady=4, ipadx=10)
+            self.checkbuttons[check_btn] = key, boolean
+            check_btn.bind("<Enter>", self.enter_button)
+        setattr(FileExtensions, "instance_cbtn", self.checkbuttons)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         btn.bind("<ButtonPress-1>", self.press_button)
 
-    def leave_button(self, event) -> None:
-        btn = event.widget
-        self.chekboxes[btn][0]
-
     def press_button(self, event) -> None:
         btn = event.widget
-        btn.bind("<ButtonRelease-1>", self.toggle_types)
+        btn.bind("<ButtonRelease-1>", self.toggle_ext)
 
-    def toggle_types(self, event) -> None:
+    @decorators.check_option_disabled
+    def toggle_ext(self, event) -> None:
         btn = event.widget
-        key = self.chekboxes[btn][0]
-        value = self.chekboxes[btn][1]
-        if value.get() is True:
-            self.data["providers"][key] = False
-        elif value.get() is False:
-            self.data["providers"][key] = True
-        io_json.set_json_data(self.data)
-
-    def toggle_providers(self, event) -> None:
-        btn = event.widget
-        key = btn["text"].replace(" ", "_").lower()
-        if self.data["providers"][key] is True:
-            self.data["providers"][key] = False
-            btn.configure(fg=cfg.color.red)
-        elif self.data["providers"][key] is False:
-            self.data["providers"][key] = True
-            btn.configure(fg=cfg.color.green)
-        io_json.set_json_data(self.data)
+        key = self.checkbuttons[btn][0]
+        value = self.checkbuttons[btn][1]
+        if value.get():
+            self.data["file_extensions"][key] = False
+        elif not value.get():
+            self.data["file_extensions"][key] = True
+        io_toml.dump_toml_data(FILE_PATHS.config, self.data)
+
+        self.update_registry()
+
+    def update_registry(self) -> None:
+        io_winreg.write_all_valuex()
+
+    def update_state(self):
+        for key in self.checkbuttons.keys():
+            if io_toml.load_toml_value(FILE_PATHS.config, "gui.context_menu"):
+                key.state(["!disabled"])
+            else:
+                key.state(["disabled"])
 
 
-class SubtitleOptions(ttk.Labelframe):
+class SubsearchOption(ttk.Labelframe):
     def __init__(self, parent) -> None:
         ttk.Labelframe.__init__(self, parent)
-        self.configure(text="Subtitle Options", padding=10)
-        self.data = io_json.get_json_data()
-        self.subtitle_options: dict = {
-            "hearing_impaired": "Include hearing impaird subtitles",
-            "non_hearing_impaired": "Include regular subtitles",
-            "foreign_only": "Only include subtitles for foreign parts",
-            "rename_best_match": "Rename best match for 'Autoload'",
+        self.configure(text="Subsearch Options", padding=10)
+        self.data = io_toml.load_toml_data(FILE_PATHS.config)
+        self.subsearch_options: dict[str, Any] = {
+            "gui.context_menu": "Context menu",
+            "gui.context_menu_icon": "Context menu icon",
+            "gui.system_tray": "System tray icon",
+            "gui.summary_notification": "Notification when done",
+            "gui.show_terminal": "Terminal while searching",
+            "misc.manual_download_on_fail": "Manual download on fail",
+            "misc.logging": "Create log file",
+            "misc.multithreading": "Multithreading",
+            "misc.single_instance": "Multiple instances",
         }
-        for name, description in self.subtitle_options.items():
-            if "hearing_impaired" in name:
-                subtitle_type = io_json.get_json_key("subtitle_type")
-                self.subtitle_options[name] = [subtitle_type[name], description]
-            else:
-                self.subtitle_options[name] = [io_json.get_json_key(name), description]
+        for name, description in self.subsearch_options.items():
+            self.subsearch_options[name] = [
+                io_toml.load_toml_value(FILE_PATHS.config, name),
+                description,
+            ]
+
+        self.checkbuttons: dict[ttk.Checkbutton, tuple[str, BooleanVar]] = {}
         frame = None
-        self.checkbuttons: dict[ttk.Checkbutton, tuple[str, tk.BooleanVar]] = {}
-        for enum, (key, value) in enumerate(self.subtitle_options.items()):
-            bool_value = value[0]
-            description = value[1]
-            if enum % 4 == 0:
+
+        for enum, (key, value) in enumerate(self.subsearch_options.items()):
+            if enum % 3 == 0:
                 frame = ttk.Frame(self)
                 frame.pack(side=tk.LEFT, anchor="n")
 
             boolean = tk.BooleanVar()
-            boolean.set(bool_value)
-            check_btn = ttk.Checkbutton(frame, text=description, onvalue=True, offvalue=False, variable=boolean)
-            check_btn.pack(padx=4, pady=4, ipadx=60)
+            boolean.set(value[0])
+            check_btn = ttk.Checkbutton(frame, text=value[1], onvalue=True, offvalue=False, variable=boolean)
+            context_menu = io_toml.load_toml_value(FILE_PATHS.config, "gui.context_menu")
+            system_tray = io_toml.load_toml_value(FILE_PATHS.config, "gui.system_tray")
+            if key == "gui.context_menu_icon" and not context_menu:
+                check_btn.state(["disabled"])
+            if key == "gui.show_terminal" and DEVICE_INFO.mode == "executable":
+                check_btn.state(["disabled"])
+            if key == "gui.summary_notification" and not system_tray:
+                check_btn.state(["disabled"])
+            check_btn.pack(padx=4, pady=4, ipadx=40)
+
             self.checkbuttons[check_btn] = key, boolean
             check_btn.bind("<Enter>", self.enter_button)
 
     def enter_button(self, event) -> None:
         btn = event.widget
         btn.bind("<ButtonPress-1>", self.press_button)
 
     def press_button(self, event) -> None:
         btn = event.widget
-        btn.bind("<ButtonRelease-1>", self.toggle_types)
+        btn.bind("<ButtonRelease-1>", self.toggle_btn)
 
-    def toggle_types(self, event) -> None:
+    @decorators.check_option_disabled
+    def toggle_btn(self, event) -> None:
         btn = event.widget
         key = self.checkbuttons[btn][0]
         value = self.checkbuttons[btn][1]
-        if value.get() is True:
-            if "hearing_impaired" in key:
-                self.data["subtitle_type"][key] = False
-            else:
-                self.data[key] = False
-        elif value.get() is False:
-            if "hearing_impaired" in key:
-                self.data["subtitle_type"][key] = True
-            else:
-                self.data[key] = True
-        io_json.set_json_data(self.data)
+        if value.get():
+            io_toml.update_toml_key(FILE_PATHS.config, key, False)
+        elif not value.get():
+            io_toml.update_toml_key(FILE_PATHS.config, key, True)
+        self.update_registry(btn)
+        keys = [("gui.context_menu", "gui.context_menu_icon"), ("gui.system_tray", "gui.summary_notification")]
+        for key_pair in keys:
+            self.disable_check_btn_children(btn, value, key_pair)
+
+    def disable_check_btn_children(self, btn: Any, value: BooleanVar, key_pair: tuple[str, str]):
+        # FileExtension checkboxes
+        parent_key = key_pair[0]
+        child_key = key_pair[1]
+        if btn["text"] != self.subsearch_options[parent_key][1]:
+            return None
+        [instance.update_state() for instance in FileExtensions.instances]
+
+        # SubsearchOptions checkboxes
+        for check_button, tuple_value in self.checkbuttons.items():
+            key = tuple_value[0]
+            if key != child_key:
+                continue
+            elif value.get():
+                check_button.state(["disabled"])
+            elif not value.get():
+                check_button.state(["!disabled"])
+
+    def update_registry(self, btn) -> None:
+        if btn["text"] != self.subsearch_options["gui.context_menu"][1]:
+            return None
+        menu = io_toml.load_toml_value(FILE_PATHS.config, "gui.context_menu")
+        if menu:
+            io_winreg.add_context_menu()
+        else:
+            io_winreg.remove_context_menu()
 
-    def add_missig_json_key(self, name, description):
-        subtitle_type = io_json.get_json_key("subtitle_type")
-        self.subtitle_options[name] = [subtitle_type[name], description]
 
-
-class SearchThreshold(tk.Frame):
+class CheckForUpdates(ttk.Labelframe):
     def __init__(self, parent) -> None:
-        tk.Frame.__init__(self, parent)
-        self.configure(bg=cfg.color.dark_grey)
-        self.pct_threashold = io_json.get_json_key("percentage_threshold")
-
-        self.current_value = tk.IntVar()
-        self.current_value.set(self.pct_threashold)
-        self.string_var = tk.StringVar()
-        self.string_var.set(f"{self.pct_threashold} %")
-
-        frame_text = tk.Frame(self, bg=cfg.color.dark_grey)
-        frame_slider = tk.Frame(self, bg=cfg.color.dark_grey)
-
-        label_description = tk.Label(frame_text, text=f"Include subtitles matching video filename by")
-        label_description.configure(bg=cfg.color.dark_grey, fg=cfg.color.white_grey, font=cfg.font.cas8b)
-        label_description.pack(side=tk.LEFT, anchor="n")
-
-        self.label_pct = tk.Label(frame_text, textvariable=self.string_var, width=4)
-        self.label_pct.configure(bg=cfg.color.dark_grey, font=cfg.font.cas8b)
-        self.label_pct.pack(side=tk.LEFT, anchor="n")
-
-        gui_toolkit.VarColorPicker(self.string_var, self.label_pct, True)
-        x, y = gui_toolkit.calculate_btn_size(self, 36)
-
-        self.slider = ttk.Scale(frame_slider, from_=0, to=100, orient="horizontal", variable=self.current_value, length=500)
-        self.slider.pack(side=tk.LEFT, anchor="n")
-
-        frame_text.pack(side=tk.TOP, anchor="n")
-        frame_slider.pack(side=tk.TOP, anchor="n")
-        self.slider.bind("<Enter>", self.enter_button)
-        self.slider.bind("<Leave>", self.leave_button)
-        gui_toolkit.set_default_grid_size(self)
-
-    def get_value(self):
-        return self.current_value.get()
-
-    def set_value(self, event) -> None:
-        self.string_var.set(f"{self.get_value()} %")
+        ttk.Labelframe.__init__(self, parent)
+        self.configure(text="Update Subsearch", padding=10, style="TLabelframePlain")
+        frame_left = tk.Frame(self, bg=cfg.color.default_bg)
+        frame_right = tk.Frame(self, bg=cfg.color.default_bg)
+
+        self.var_current = tk.StringVar(self, f"Current version:\t\t{__version__}")
+        self.var_latest = tk.StringVar(self, "Latest version: \t\t")
+        self.var_misc = tk.StringVar()
+
+        frame_current = tk.Label(frame_left, textvariable=self.var_current, justify="left")
+        frame_latest = tk.Label(frame_left, textvariable=self.var_latest, justify="left")
+        self.frame_misc = tk.Label(frame_left, textvariable=self.var_misc, justify="left")
+        frame_current.pack(anchor="w")
+        frame_latest.pack(anchor="w")
+        self.frame_misc.pack(pady=16, anchor="w")
+
+        self.btn_search = ttk.Button(
+            frame_right,
+            text="Search",
+            width=20,
+        )
+        self.btn_visit_release_page = ttk.Button(
+            frame_right,
+            text="Open in webbrowser",
+            width=20,
+        )
+        self.btn_search.pack(padx=2, pady=2)
+        self.btn_visit_release_page.pack(padx=2, pady=2)
+        self.btn_visit_release_page.state(["disabled"])
+        self.btn_search.bind("<Enter>", self.enter_button)
+
+        self.pack(anchor="center", fill="x")
+        width = self.winfo_reqwidth()
+        half_width = round(width // 2)
+        frame_left.pack(side=tk.LEFT, anchor="n", expand=True, fill="x", ipadx=half_width)
+        frame_right.pack(side=tk.LEFT, anchor="n", expand=True, fill="x", ipadx=half_width)
 
     def enter_button(self, event) -> None:
         btn = event.widget
-        if btn == self.slider:
-            self.slider.bind("<ButtonPress>", self.press_slider)
-            self.slider.bind("<Double-ButtonRelease-1>", self.dubble_press)
+        if btn == self.btn_search:
+            btn.bind("<ButtonRelease-1>", self.search_button)
 
-    def leave_button(self, event) -> None:
-        btn = event.widget
-        if btn == self.slider:
-            self.slider.configure(command=self.set_value)
-
-    def dubble_press(self, event) -> None:
-        btn = event.widget
-        if btn == self.slider:
-            self.current_value.set(90)
-            self.string_var.set(f"{90} %")
-            self.slider.update()
-            self.update_config()
-
-    def press_slider(self, event) -> None:
-        btn = event.widget
-        if btn == self.slider:
-            self.slider.configure(command=self.set_value)
-            self.slider.bind("<ButtonRelease>", self.release_slider)
+    def search_button(self, event) -> None:
+        new_repo_avail, repo_is_prerelease = update.is_new_version_avail()
+        latest_version = update.get_latest_version()
+        if new_repo_avail:
+            self.var_latest.set(f"Latest version: \t\t{latest_version}")
+            self.btn_search.state(["disabled"])
+            self.btn_visit_release_page.state(["!disabled"])
+            self.btn_visit_release_page.bind("<ButtonRelease-1>", self.visit_repository_button)
+            if repo_is_prerelease:
+                self.var_misc.set(f"Pre-release")
+                self.frame_misc.configure(fg=cfg.color.orange)
+            else:
+                self.var_misc.set(f"Latest")
+                self.frame_misc.configure(fg=cfg.color.green)
 
-    def release_slider(self, event) -> None:
-        btn = event.widget
-        if btn == self.slider:
-            self.slider.configure(command=self.set_value)
-            self.update_config()
+        if not new_repo_avail:
+            self.var_latest.set(f"Latest version: \t\t{latest_version}")
+            self.var_misc.set(f"Latest version already installed")
 
-    def update_config(self) -> None:
-        update_svar = self.current_value.get()
-        io_json.set_config_key_value("percentage_threshold", update_svar)
-        gui_toolkit.VarColorPicker(self.string_var, self.label_pct, True)
+    def visit_repository_button(self, event) -> None:
+        webbrowser.open(f"https://github.com/vagabondHustler/subsearch/releases")
```

### Comparing `Subsearch-2.37.1/src/subsearch/providers/subscene.py` & `Subsearch-2.38.0rc1/src/subsearch/providers/subscene.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from selectolax.parser import Node
 
-from subsearch.data import app_paths
-from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
-from subsearch.providers import generic
-from subsearch.providers.generic import ProviderParameters
-from subsearch.utils import log, string_parser
+from subsearch.data.data_classes import Subtitle
+from subsearch.providers import core_provider
 
 
-class SubsceneScraper:
-    def __init__(self) -> None:
-        ...
+class SubsceneScraper(core_provider.ProviderHelper):
+    def __init__(self, **kwargs) -> None:
+        core_provider.ProviderHelper.__init__(self, **kwargs)
 
     def find_title(self, url: str, current_language: str, definitive_match: list[str]) -> str | None:
-        tree = generic.get_html_parser(url)
+        tree = core_provider.get_html_parser(url)
         products = tree.css("div.title")
         for item in products:
             node = item.css_first("a")
             result_href = node.attributes["href"]
             result_title = str(node.child.html).lower()
             if result_title not in definitive_match:
                 continue
@@ -32,82 +29,50 @@
             return True
         elif regular_sub is False and item.css_matches("td.a41"):
             return True
         return False
 
     def find_subtitles(self, url: str, hi_sub: bool, regular_sub: bool, subscene_header) -> dict[str, str]:
         subtitles: dict[str, str] = {}
-        tree = generic.get_html_parser(url, subscene_header)
+        tree = core_provider.get_html_parser(url, subscene_header)
         products = tree.css("tr")
         for item in products[1:]:
             if self.skip_item(item, hi_sub, regular_sub):
                 continue
             node = item.css_first("a")
             if node.child.text_content == "upload":
                 continue
             subtitle_href = node.attributes["href"]
             filename = item.css_first("span:nth-child(2)").child.text_content.strip()
             subtitles[filename] = f"https://subscene.com{subtitle_href}"
         return subtitles
 
-    def get_download_url(self, url: str) -> str:
-        tree = generic.get_html_parser(url)
-        href = tree.css_first("#downloadButton").attributes["href"]
-        download_url = f"https://subscene.com/{href}"
-        return download_url
 
-
-class Subscene(ProviderParameters, SubsceneScraper):
+class Subscene(SubsceneScraper):
     def __init__(self, **kwargs):
-        ProviderParameters.__init__(self, **kwargs)
-        SubsceneScraper.__init__(self)
-        self.logged_and_sorted: list[PrettifiedDownloadData] = []
+        SubsceneScraper.__init__(self, **kwargs)
+        self.provider_name = self.__class__.__name__.lower()
 
-    def _definitive_match(self) -> list[str]:
-        if self.tvseries:
-            return [f"{self.title} - {self.season_ordinal} season"]
-        return [f"{self.title} ({self.year})", f"{self.title} ({(self.year-1)})"]
-
-    def parse_site_results(self) -> list | list[DownloadData]:
-        to_be_sorted: list[PrettifiedDownloadData] = []
-        _to_be_downloaded: dict[str, str] = {}
-        to_be_downloaded: dict[str, str] = {}
-        custom_subscene_header = generic.CustomSubsceneHeader(self.app_config)
+    def start_search(self):
+        custom_subscene_header = core_provider.CustomSubsceneHeader(self.app_config)
         header = custom_subscene_header.create_header()
-        # find title
         definitive_match = self._definitive_match()
         found_title_url = self.find_title(self.url_subscene, self.current_language, definitive_match)
+
         if not found_title_url:
             return []
 
-        # search for subtitles
         subtitle_data = self.find_subtitles(found_title_url, self.hi_sub, self.non_hi_sub, header)
-        for key, value in subtitle_data.items():
-            pct_result = string_parser.calculate_match(key, self.release)
-            log.output_match("subscene", pct_result, key)
-            formatted_data = generic.prettify_download_data("subscene", key, value, pct_result)
-            to_be_sorted.append(formatted_data)
-            if self.is_threshold_met(key, pct_result) is False or self.manual_download_mode:
-                continue
-            if key in _to_be_downloaded.keys():
-                continue
-            _to_be_downloaded[key] = value
+        self._process_subtitle_data(self.provider_name, subtitle_data)
 
-        self.sorted_metadata = generic.sort_prettified_data(to_be_sorted)
-        log.downlod_metadata("subscene", self.sorted_metadata, self.percentage_threashold)
-        if not _to_be_downloaded:
-            return []
-
-        # gather subtitle download url
-        for release, subtitle_url in _to_be_downloaded.items():
-            zip_url = self.get_download_url(subtitle_url)
-            to_be_downloaded[release] = zip_url
-
-        if not to_be_downloaded:
-            return []
-
-        # pack download data
-        download_info = generic.create_download_data("subscene", app_paths.tmpdir, to_be_downloaded)
-        return download_info
+    def _definitive_match(self) -> list[str]:
+        if self.tvseries:
+            return [f"{self.title} - {self.season_ordinal} season"]
+        return [f"{self.title} ({self.year})", f"{self.title} ({(self.year-1)})"]
 
-    def _sorted_list(self) -> list[PrettifiedDownloadData]:
-        return self.sorted_metadata
+    @property
+    def accepted_subtitles(self) -> list[Subtitle]:
+        return self._accepted_subtitles
+
+    @property
+    def rejected_subtitles(self) -> list[Subtitle]:
+        return self._rejected_subtitles
```

### Comparing `Subsearch-2.37.1/src/subsearch/utils/exceptions.py` & `Subsearch-2.38.0rc1/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.37.1/src/subsearch/utils/file_manager.py` & `Subsearch-2.38.0rc1/src/subsearch/utils/io_file_system.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,152 @@
 import shutil
 import struct
-import sys
 import zipfile
 from pathlib import Path
 
-from subsearch.data import __guid__, video_data
-from subsearch.data.data_objects import DownloadData
-from subsearch.providers.generic import get_cloudscraper
-from subsearch.utils import log, string_parser
+from subsearch.data.constants import VIDEO_FILE
+from subsearch.data.data_classes import Subtitle
+from subsearch.providers.core_provider import get_cloudscraper
+from subsearch.utils import io_log, string_parser
+
+
+def create_path_from_string(string: str, path_resolution: str) -> Path:
+    if path_resolution == "relative":
+        if string == ".":
+            path = VIDEO_FILE.file_directory
+        elif string.startswith(".\\") and len(string) > 2:
+            path = VIDEO_FILE.file_directory.joinpath(string[2:])
+        elif string == "..":
+            path = VIDEO_FILE.file_directory.parent
+        elif string.startswith("..\\") and len(string) > 3:
+            path = VIDEO_FILE.file_directory.parent.joinpath(string[3:])
+    elif path_resolution == "absolute":
+        path = Path(string)
 
-
-def running_from_exe() -> bool:
-    """
-    Checks if the module is running from an executable file.
-
-    Returns:
-        bool: True if the module is running from an executable file, False otherwise.
-    """
-    if sys.argv[0].endswith(".exe"):
-        return True
-    return False
+    path.mkdir(parents=True, exist_ok=True)
+    return path
 
 
-def download_subtitle(data: DownloadData) -> int:
+def download_subtitle(subtitle: Subtitle, index_position: int, index_size: int):
     """
     Download the subtitle from the given url.
 
     Args:
       data: A DownloadMetaData object that has information about the subtitle file to be downloaded.
 
     Returns:
       An integer value that represents the index number of the subtitle that was downloaded.
 
     Raises:
       Any exception raised by the get_cloudscraper or IOError during writing of the subtitle file.
     """
-    log.output(f"{data.provider}: {data.idx_num}/{data.idx_lenght}: {data.name}")
+    io_log.stdout(f"{subtitle.provider}: {index_position}/{index_size}: {subtitle.release_name}")
     scraper = get_cloudscraper()
-    r = scraper.get(data.url, stream=True)
-    with open(data.file_path, "wb") as fd:
+    r = scraper.get(subtitle.download_url, stream=True)
+    file_name = f"{subtitle.provider}_{subtitle.release_name}_{index_position}.zip"
+    download_path = VIDEO_FILE.tmp_dir / file_name
+    with open(download_path, "wb") as fd:
         for chunk in r.iter_content(chunk_size=1024):
             fd.write(chunk)
 
-    return data.idx_num
-
 
-def extract_files(src: Path, dst: Path, extension: str) -> None:
+def extract_files_in_dir(src: Path, dst: Path, extension: str = ".zip") -> None:
     """
     Extract files from a directory to a specified Destination.
 
     Args:
         src (Path): Source path to extract files
         dst (Path): Destination path to extract files
         extension (str): Extension of files to be extracted
 
     Returns:
         None.
     """
-    for file in Path(src).glob(f"*{extension}"):
-        filename = Path(src) / file
-        log.path_action("extract", file, dst)
+    for file in src.glob(f"*{extension}"):
+        filename = src / file
+        io_log.stdout_path_action(action_type="extract", src=file, dst=dst)
         zip_ref = zipfile.ZipFile(filename)
         zip_ref.extractall(dst)
         zip_ref.close()
 
 
-def rename_best_match(release_name: str, cwd: Path, extension: str) -> None:
-    """
-    Function renames and moves the best matching subtitle file, based on the release name, to the specified path. If no match is found nothing happens.
-
-    Args:
-        release_name (str): The name of the video release whose subtitle is being renamed.
-        cwd (Path): The path to the working directory.
-        extension (str): The file type of the subtitles i.e ".srt".
-
-    Returns:
-        None.
-    """
-    if video_data is None:
-        return None
-    best_match = (0, Path())
-    for file in Path(video_data.subs_directory).glob(f"*{extension}"):
+def autoload_rename(release_name: str, extension: str = ".srt") -> Path:
+    best_match = (0, Path("."))
+    for file in VIDEO_FILE.subs_dir.glob(f"*{extension}"):
         value = string_parser.calculate_match(file.name, release_name)
         if value >= best_match[0]:
             best_match = value, file
-    if not best_match[1]:
-        return None
-    file_to_rename = best_match[1]
-    old_name_src = Path(video_data.subs_directory) / file_to_rename
-    new_name_dst = Path(video_data.subs_directory) / release_name
-    log.path_action("rename", file_to_rename, new_name_dst)
-    old_name_src.rename(new_name_dst)
-    move_src = new_name_dst
-    move_dst = Path(cwd) / release_name
-    log.path_action("move", move_src, cwd)
-    if move_dst.exists():
-        move_dst.unlink()
-    shutil.move(move_src, move_dst)
+
+    old_file_path = best_match[1]
+    new_file_path = old_file_path.with_name(f"{release_name}{extension}")
+    io_log.stdout_path_action(action_type="rename", src=old_file_path, dst=new_file_path)
+    old_file_path.rename(new_file_path)
+    return new_file_path
+
+
+def move_all(src: Path, dst: Path, extension: str = ".srt"):
+    for file in src.glob(f"*{extension}"):
+        move_and_replace(file.absolute(), dst)
+
+
+def move_and_replace(source_file: Path, destination_directory: Path) -> None:
+    source_file.replace(destination_directory / source_file.name)
 
 
-def clean_up_files(cwd: Path, extension: str) -> None:
+def del_file_type(cwd: Path, extension: str) -> None:
     """
     Removes files with specific extensions in a given directory
 
     Args:
         cwd (pathlib.Path): The directory path where the files to be deleted reside.
         extension (str): The file extension of the files to be deleted.
 
     Returns:
         None
     """
     for file in Path(cwd).glob(f"*{extension}"):
-        log.path_action("remove", file)
+        io_log.stdout_path_action(action_type="remove", src=file)
         file_path = Path(cwd) / file
         file_path.unlink()
 
 
 def del_directory(directory: Path) -> None:
     """
     Remove a directory and its contents.
 
     Args:
         directory: A Path object representing the directory to be removed.
 
     Returns:
         None
     """
-    log.path_action("remove", directory)
+    io_log.stdout_path_action(action_type="remove", src=directory)
     shutil.rmtree(directory)
 
 
 def directory_is_empty(directory: Path) -> bool:
     if not any(directory.iterdir()):
         return True
     return False
 
 
-def get_hash(file_path: Path | None) -> str:
+def del_directory_content(directory: Path):
+    for item in directory.iterdir():
+        io_log.stdout_path_action(action_type="remove", src=item)
+        if item.is_file():
+            item.unlink()
+        if item.is_dir():
+            shutil.rmtree(item)
+
+
+def create_directory(path: Path):
+    path.mkdir(exist_ok=True)
+
+
+def get_file_hash(file_path: Path | None) -> str:
     """
     Calculates and returns the hash value of given file path.
 
     Args:
         file_path: A Path object indicating the location of the input file. If None, returns an all-zero string.
 
     Returns:
@@ -155,15 +161,15 @@
     try:
         longlongformat = "<q"
         bytesize = struct.calcsize(longlongformat)
         with open(file_path, "rb") as f:
             filesize = file_path.stat().st_size
             hash = filesize
             if filesize < 65536 * 2:
-                log.output(f"SizeError: filesize is {filesize} bytes", False)
+                io_log.stdout(f"SizeError: filesize is {filesize} bytes", level="error")
                 return ""
             n1 = 65536 // bytesize
             for _x in range(n1):
                 buffer = f.read(bytesize)
                 (l_value,) = struct.unpack(longlongformat, buffer)
                 hash += l_value
                 hash = hash & 0xFFFFFFFFFFFFFFFF
@@ -176,20 +182,7 @@
                 hash = hash & 0xFFFFFFFFFFFFFFFF
 
         returnedhash = "%016x" % hash
         return returnedhash
 
     except IOError:
         return ""
-
-
-def delete_temp_files(temp_path: Path):
-    for item in temp_path.iterdir():
-        log.path_action("remove", item)
-        if item.is_file():
-            item.unlink()
-        if item.is_dir():
-            shutil.rmtree(item)
-
-
-def create_directory(path: Path):
-    path.mkdir(exist_ok=True)
```

### Comparing `Subsearch-2.37.1/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.38.0rc1/src/subsearch/utils/imdb_lookup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from subsearch.providers import generic
+from subsearch.providers import core_provider
 
 
 class AdvTitleSearch:
     """
     A class representing an advanced title search.
 
     Attributes:
@@ -84,15 +84,15 @@
         self.title = title.lower()
         self.year = year
         self.id = None
 
         adv_search = AdvTitleSearch(self.title, self.year)
 
         url = adv_search.get_url()
-        tree = generic.get_html_parser(url)
+        tree = core_provider.get_html_parser(url)
         product = tree.select("div.lister-item-content")
 
         for item in product.matches:
             self.data = item.css_first("h3.lister-item-header")
 
             if self.title != self.find_imdb_title():
                 continue
```

### Comparing `Subsearch-2.37.1/src/subsearch/utils/io_winreg.py` & `Subsearch-2.38.0rc1/src/subsearch/utils/io_winreg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import socket
 import sys
 import winreg
 from pathlib import Path
 
-from subsearch.data import app_paths
-from subsearch.utils import file_manager
+from subsearch.data.constants import APP_PATHS, DEVICE_INFO, FILE_PATHS
+from subsearch.utils import io_toml
 
 COMPUTER_NAME = socket.gethostname()
 CLASSES_PATH = r"Software\Classes"
 ASTERISK_PATH = r"Software\Classes\*"
 SHELL_PATH = r"Software\Classes\*\shell"
 SUBSEARCH_PATH = r"Software\Classes\*\shell\Subsearch"
 COMMAND_PATH = r"Software\Classes\*\shell\Subsearch\command"
@@ -79,35 +79,29 @@
                 # write valuex to matching value name
                 winreg.SetValueEx(sk, value_name, 0, winreg.REG_SZ, value)
     except FileNotFoundError:
         pass
 
 
 def get_command_value() -> str:
-    """
-    Returns the command to execute when the context menu is used on a file for SubSearch.
+    # get latest toml value from file
+    from subsearch.utils import io_toml
 
-    Returns:
-        A string containing the command to execute for the corresponding value.
-    """
-    # get latest json value from file
-    from subsearch.utils import io_json
-
-    if file_manager.running_from_exe():
+    if DEVICE_INFO.mode == "executable":
         value = f'"{sys.argv[0]}" "%1"'
         # if SubSearch is compiled we dont need anything besides this
-    elif file_manager.running_from_exe() is False:
-        show_terminal = io_json.get_json_key("show_terminal")
+    elif DEVICE_INFO.mode == "interpreter":
+        show_terminal = io_toml.load_toml_value(FILE_PATHS.config, "gui.show_terminal")
         # gets the location to the python executable
         python_path = Path(sys.executable).parent
         # sys.args[-1] is going to be the path to the file we right clicked on
         # import_sys = "import sys; media_file_path = sys.argv[-1];"
         set_title = "import ctypes; ctypes.windll.kernel32.SetConsoleTitleW('subsearch');"
         # gets the path of the root directory of subsearch
-        set_wd = f"import os; os.chdir(r'{app_paths.home}');"
+        set_wd = f"import os; os.chdir(r'{APP_PATHS.home}');"
         import_main = "import subsearch; subsearch.main()"
         if show_terminal is True:
             value = f'{python_path}\python.exe -c "{set_title} {set_wd} {import_main}" "%1"'
         if show_terminal is False:
             value = f'{python_path}\pythonw.exe -c "{set_title} {set_wd} {import_main}" "%1"'
 
     return value
@@ -117,40 +111,28 @@
     """
     Returns the icon path to use in the context menu, or an empty string if configuration specifies it should not be shown
 
     Returns:
         str: Path of the icon file to be used in the context menu, or an empty string if the configuration specifies
              that it should not be shown.
     """
-    from subsearch.utils import io_json
-
-    show_icon: str = io_json.get_json_key("context_menu_icon")
+    show_icon: str = io_toml.load_toml_value(FILE_PATHS.config, "gui.context_menu_icon")
     if show_icon:
-        return str(app_paths.gui_assets / "subsearch.ico")
+        return str(APP_PATHS.gui_assets / "subsearch.ico")
     else:
         return ""
 
 
 def get_appliesto_value() -> str:
-    """
-    Retrieve the latest json value from file `raw_json`.
-
-    Returns:
-        str: A string of file types to show the SubSearch context entry on
-            The file types are concatenated with `" OR "` in between.
-    """
-    # get latest json value from file
-    from subsearch.utils import io_json
-
-    file_ext = io_json.get_json_key("file_extensions")
+    file_ext = io_toml.load_toml_value(FILE_PATHS.config, "file_extensions")
     # for which file types to show the SubSearch context entry on
     value = ""
-    for k, v in zip(file_ext.keys(), file_ext.values()):
+    for ext, v in zip(file_ext.keys(), file_ext.values()):
         if v is True:
-            value += "".join(f'"{k}" OR ')
+            value += "".join(f'".{ext}" OR ')
     if value.endswith(" OR "):  # remove last OR
         value = value[:-4]
 
     return value
 
 
 def remove_context_menu() -> None:
```

### Comparing `Subsearch-2.37.1/src/subsearch/utils/string_parser.py` & `Subsearch-2.38.0rc1/src/subsearch/data/data_classes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,336 +1,270 @@
-import re
-
-from num2words import num2words
-
-from subsearch.data.data_objects import (
-    AppConfig,
-    LanguageData,
-    ProviderUrls,
-    ReleaseData,
-)
-from subsearch.utils import imdb_lookup
-
-
-def find_year(string: str) -> int:
-    """
-    Find and return the year from a string.
-
-    Args:
-        string (str): The string where the year has to be looked for.
-
-    Returns:
-        int: The first 4 digit number that matches the regex pattern or 0000 if no match is found.
-    """
-    re_year = re.findall("^.*\.([1-2][0-9]{3})\.", string)
-    if re_year:
-        year = re_year[0]
-        return int(year)
-    return 0000
-
-
-def find_title_by_year(string: str) -> str:
-    """
-    Find and return the title of a media file by year.
-
-    Args:
-        string (str): The file name.
-
-    Returns:
-        str: The part of the file name before the year, with '.' replaced by ' ', or "" if no match is found.
-    """
-    re_title = re.findall("^(.*)\.[1-2][0-9]{3}\.", string)
-    if re_title:
-        title: str = re_title[0]
-        title = title.replace(".", " ")
-        return title
-    return ""
-
-
-def find_title_by_show(string: str) -> str:
-    """
-    Find and return the title of a media file by show.
-
-    Args:
-        string (str): The file name.
-
-    Returns:
-        str: The part of the filename before the season and episode values, with '.' replaced by ' ', or "" if no match is found.
-    """
-    re_title = re.findall("^(.*)\.[s]\d*[e]\d*\.", string)
-    if re_title:
-        title: str = re_title[0]
-        title = title.replace(".", " ")
-        return title
-    return ""
-
-
-def find_season_episode(string: str) -> str:
-    """
-    Find and return the season and episode values of a media file.
-
-    Args:
-        string (str): The file name.
-
-    Returns:
-        str: A string consisting of the season and episode values formatted like "s01e01", or "" if no match is found.
-    """
-    re_se = re.findall("\.([s]\d*[e]\d*)\.", string)
-    if re_se:
-        se: str = re_se[0]
-        return se
-    return ""
-
-
-def convert_to_ordinal_string(string: str) -> tuple[str, str, str, str, bool]:
-    """
-    Converts the numeric TV series values (season and episode numbers) in a filename to their ordinal versions(if any).
-
-    Args:
-        string (str): The TV series values as pulled out from the filename as a single string, e.g., `s01e01`.
-
-    Returns:
-        tuple(str, str, str, str, bool): A tuple containing separated season and episode strings, corresponding ordinal
-            strings, and a Boolean flag indicating whether the input string was matched successfully.
-    """
-    if string == "":
-        season, season_ordinal, episode, episode_ordinal = "", "", "", ""
-        show_bool = False
-    else:
-        season, episode = string.replace("s", "").replace("e", " ").split(" ")
-        season_ordinal = num2words(int(season), lang="en", to="ordinal")
-        episode_ordinal = num2words(int(episode), lang="en", to="ordinal")
-        show_bool = True
-    return season, season_ordinal, episode, episode_ordinal, show_bool
-
-
-def find_group(string: str) -> str:
-    """
-    Find and return the group from a string.
-
-    Args:
-        string (str): The string where the group has to be looked for.
-
-    Returns:
-        str: The group identifier as taken from the end of the string.
-    """
-    group = string.rsplit("-", 1)[-1]
-    return group
-
-
-def find_title(filename: str, year: int, series: bool):
-    """
-    Find and return the media file's title, taking its year and/or TV series values into consideration.
-
-    Args:
-        filename (str): The name of the media file.
-        year (int): The relevant year, extracted from the name, passed on from another method.
-        series (bool): Whether the video file is a TV series or not.
-
-    Returns:
-        str: The name of the given media file.
-    """
-    if year != 0000:
-        title = find_title_by_year(filename)
-    elif series and year == 0000:
-        title = find_title_by_show(filename)
-    else:
-        title = filename.rsplit("-", 1)[0]
-    return title
-
-
-class CreateProviderUrls:
-    def __init__(self, file_hash: str, app_config: AppConfig, release_data: ReleaseData, language_data: LanguageData):
-        """
-        Initializes a new instance of the CreateProviderUrls class.
-
-        Args:
-            file_hash (str): The file hash.
-            app_config (AppConfig): The application configuration
-            release_metadata (ReleaseMetadata): The release metadata
-        """
-        self.file_hash = file_hash
-        self.app_config = app_config
-        self.release_data = release_data
-        self.language_data = language_data
-
-    def retrieve_urls(self) -> ProviderUrls:
-        """
-        Get the provider urls to search for subtitles.
-
-        Returns:
-            ProviderUrls: A collection of strings that contains urls to search for subtitles from different subtitle providers.
-        """
-        return ProviderUrls(self.subscene(), self.opensubtitles(), self.opensubtitles_hash(), self.yifysubtitles())
-
-    def subscene(self) -> str:
-        """
-        Gets the Url for the Subscene website to search for subtitles.
-
-        Returns:
-            str: The url to search for subtitles on subscene.com
-        """
-        domain = "https://subscene.com"
-        query = "subtitles/searchbytitle?query"
-        search_parameters = self._subscene_search_parameters()
-        url_subscene = f"{domain}/{query}={search_parameters}"
-        return url_subscene.replace(" ", "%20")
-
-    def opensubtitles(self) -> str:
-        """
-        Gets the Url for the Opensubtitles website to search for subtitles.
-
-        Returns:
-            str: The url to search for subtitles on opensubtitles.org
-        """
-        domain = "https://www.opensubtitles.org"
-        subtitle_type = self._opensubtitles_subtitle_type()
-        search_parameters = self._opensubtitles_search_parameters()
-        return f"{domain}/{subtitle_type}/{search_parameters}/rss_2_00".replace(" ", "%20")
-
-    def opensubtitles_hash(self) -> str:
-        """
-        Gets the Url to set a moviehash for the Opensubtitles website to find subtitles.
-
-        Returns:
-            str: the url to set moviehash for opensubtitles.org
-        """
-        domain = "https://www.opensubtitles.org"
-        subtitle_type = self._opensubtitles_subtitle_type()
-        return f"{domain}/{subtitle_type}/moviehash-{self.file_hash}"
-
-    def yifysubtitles(self) -> str:
-        """
-        Gets the Url for the YifySubtitles website to search for subtitles for movies.
-
-        Returns:
-            str: The url to search for subtitles on yifysubtitles.org
-        """
-        if self.release_data.tvseries:
-            return ""
-        domain = "https://yifysubtitles.org"
-        tt_id = imdb_lookup.FindImdbID(self.release_data.title, self.release_data.year).id
-        return f"{domain}/movie-imdb/{tt_id}" if tt_id is not None else ""
-
-    def _subscene_search_parameters(self) -> str:
-        """
-        Gets the search parameters for Subscene to search for the appropriate subtitles based on File name and season ordinal.
-
-        Returns:
-            str: The search parameter value for Subscene to search for the applicable subtitles.
-        """
-        if self.release_data.tvseries:
-            return f"{self.release_data.title} - {self.release_data.season_ordinal} season"
-        return f"{self.release_data.title}"
-
-    def _opensubtitles_subtitle_type(self) -> str:
-        """
-        Gets the subtitle type and language settings for Opensubtitles based on Application configuration.
-
-        Returns:
-            str: The subtitle types and language configurations to search for subtitles in Opensubtitles.
-        """
-        if self.app_config.hearing_impaired and self.app_config.non_hearing_impaired is False:
-            return f"en/search/sublanguageid-{self.language_data.alpha_2b}/hearingimpaired-on"
-        return f"en/search/sublanguageid-{self.language_data.alpha_2b}"
-
-    def _opensubtitles_search_parameters(self) -> str:
-        """
-        Gets the search parameters for Opensubtitles to search for the appropriate subtitles based on Movie title, year, season and episode number.
-
-        Returns:
-            str: The search parameter value for Opensubtitles to search for the applicable subtitles.
-        """
-        if self.release_data.tvseries:
-            return f"searchonlytvseries-on/season-{self.release_data.season}/episode-{self.release_data.episode}/moviename-{self.release_data.title}"
-        return f"searchonlymovies-on/moviename-{self.release_data.title} ({self.release_data.year})"
-
-
-def get_release_metadata(filename: str, file_hash: str) -> ReleaseData:
-    """
-    Collects the necessary metadata from a filename.
-
-    Args:
-      filename (str): The name of the file to obtain release metadata from.
-      file_hash (str): The hash value of the file.
-
-    Returns:
-      ReleaseMetadata: A ReleaseMetadata object containing the relevant metadata for the inputted file.
-
-    """
-    filename = filename.lower()
-    year = find_year(filename)
-    season_episode = find_season_episode(filename)
-    season, season_ordinal, episode, episode_ordinal, series = convert_to_ordinal_string(season_episode)
-
-    title = find_title(filename, year, series)
-    group = find_group(filename)
-
-    parameters = ReleaseData(
-        title,
-        year,
-        season,
-        season_ordinal,
-        episode,
-        episode_ordinal,
-        series,
-        filename,
-        group,
-        file_hash,
-    )
-    return parameters
-
-
-def calculate_match(from_user: str, from_website: str) -> int:
-    """
-    Calculates the match between user input and website information
-
-    Args:
-        from_user (str): User input string
-        from_website (str): Website information string
-
-    Returns:
-        int: The percentage of matching between two strings.
-    """
-    max_percentage = 100
-    _from_user: list[str] = mk_lst(from_user)
-    _from_website: list[str] = mk_lst(from_website)
-    lst1, lst2 = make_equal_size(_from_user, _from_website)
-    not_matching = list(set(lst1) - set(lst2))
-    not_matching_value = len(not_matching)
-    number_of_items = len(lst1)
-    percentage_to_remove = round(not_matching_value / number_of_items * max_percentage)
-    pct = round(max_percentage - percentage_to_remove)
-
-    return pct
-
-
-def mk_lst(release: str) -> list[str]:
-    new: list[str] = []
-    qualities = ["720p", "1080p", "1440p", "2160p"]
-    temp = release.split(".")
-
-    for item in temp:
-        if item not in qualities:
-            new.append(item.lower())
-    return new
-
-
-def make_equal_size(lst1, lst2):
-    if len(lst1) == len(lst2):
-        return lst1, lst2
-    elif len(lst1) > len(lst2):
-        lst_big, lst_small = lst1, lst2
-    else:
-        lst_big, lst_small = lst2, lst1
-
-    num_big, num_small = sorted((len(lst1), len(lst2)), reverse=True)
-    difference = num_big - num_small
-    filled_list = fill_shorter_list(lst_big, lst_small, difference)
-    return lst_big, filled_list
-
-
-def fill_shorter_list(big_lst, small_lst, difference):
-    if big_lst > small_lst:
-        for _i in range(difference):
-            small_lst.append(None)
-    return small_lst
+from dataclasses import dataclass
+from pathlib import Path
+from typing import Union
+
+
+@dataclass(order=True)
+class LanguageData:
+    name: str
+    alpha_1: str
+    alpha_2b: str
+    incompatibility: list[str]
+    subscene_id: int
+
+
+@dataclass(order=True, slots=True)
+class ProviderAlphaCodeData:
+    provider: str
+    alpha_code: str
+
+
+@dataclass(order=True, slots=True)
+class AppPaths:
+    """
+    A dataclass representing the paths used in the application.
+
+    Attributes:
+        home (Path): The root directory of the application.
+        data (Path): The directory where data related to the application is stored.
+        gui (Path): The directory containing GUI modules and files.
+        providers (Path): The directory containing subtitle provider modules.
+        utils (Path): The directory containing utility modules.
+        tmp_dir(Path): The directory containing temporary files & folders.
+        appdata_subsearch(Path): The directory containing the persistent application files.
+    """
+
+    home: Path
+    data: Path
+    gui: Path
+    gui_assets: Path
+    gui_styles: Path
+    providers: Path
+    utils: Path
+    tmp_dir: Path
+    appdata_subsearch: Path
+
+
+@dataclass(order=True, slots=True)
+class FilePaths:
+    """
+    A dataclass representing the files used in the application.
+
+    Attributes:
+        subsearch_log (Path): The default subsearch_log.log file location
+        subsearch_config (Path): The default subsearch_config.toml file location
+        language_data (Path): The default language_data.toml file location
+    """
+
+    log: Path
+    config: Path
+    language_data: Path
+
+
+@dataclass(order=True, slots=True)
+class VideoFile:
+    """
+     Class representing file information.
+
+    Attributes:
+        filename (str): Name of the file.
+        file_extension (str): Extension of the file.
+        file_path (pathlib.Path): Path of the file.
+        directory (pathlib.Path): Directory path of the file.
+        subs_directory (pathlib.Path): Subtitles directory path.
+        tmp_directory (pathlib.Path): Temporary directory path.
+    """
+
+    filename: str
+    file_hash: str
+    file_extension: str
+    file_path: Path
+    file_directory: Path
+    subs_dir: Path
+    tmp_dir: Path
+
+
+@dataclass(order=True, slots=True)
+class AppConfig:
+    """
+    This class is a data structure used to store various configuration options for an application.
+    These options include preferences related to subtitle filters, file extensions, providers,
+    automatic actions, context menu options, logging, and other features.
+
+    Attributes:
+        language (str): The language setting for the application.
+        accept_threshold (int): The threshold value for accepting subtitles.
+        hearing_impaired (bool): A flag indicating whether to include hearing-impaired subtitles.
+        non_hearing_impaired (bool): A flag indicating whether to include non-hearing-impaired subtitles.
+        only_foreign_parts (bool): A flag indicating whether to include only foreign parts subtitles.
+        context_menu (bool): A flag indicating whether to enable context menu options.
+        context_menu_icon (bool): A flag indicating whether to display icons in the context menu.
+        system_tray (bool): A flag indicating whether to enable the application in the system tray.
+        summary_notification (bool): A flag indicating whether to display summary notifications.
+        show_terminal (bool): A flag indicating whether to show the terminal in the application.
+        autoload (dict[str, Union[bool, str]]): A dictionary containing autoload options.
+        file_extensions (dict[str, bool]): A dictionary containing file extensions.
+        providers (dict[str, bool]): A dictionary containing provider options.
+        manual_download_on_fail (bool): A flag indicating whether to enable manual downloads on failure.
+        multithreading (bool): A flag indicating whether to enable multithreading.
+        single_instance (bool): A flag indicating whether to enable single-instance mode.
+        logging (bool): A flag indicating whether to enable logging for the application.
+
+    Examples:
+        >>> config = AppConfig(
+        ...     language="english",
+        ...     accept_threshold=False,
+        ...     hearing_impaired=90,
+        ...     non_hearing_impaired=True,
+        ...     only_foreign_parts=True,
+        ...     context_menu=True,
+        ...     context_menu_icon=True,
+        ...     system_tray=True,
+        ...     summary_notification=True,
+        ...     show_terminal=False,
+        ...     autoload={"rename": True, "move": True, "target_path": "."},
+        ...     file_extensions=False,
+        ...     providers=True,
+        ...     manual_download_on_fail={"mkv": True, "avi": False ...},
+        ...     multithreading={"subscene_site": True, "opensubtitles_site": True, "opensubtitles_hash": True ...},
+        ...     single_instance=False,
+        ...     logging=True,
+        ... )
+    """
+
+    language: str
+    accept_threshold: int
+    hearing_impaired: bool
+    non_hearing_impaired: bool
+    only_foreign_parts: bool
+    context_menu: bool
+    context_menu_icon: bool
+    system_tray: bool
+    summary_notification: bool
+    show_terminal: bool
+    subtitle_post_processing: dict[str, Union[bool, str]]
+    file_extensions: dict[str, bool]
+    providers: dict[str, bool]
+    manual_download_on_fail: bool
+    multithreading: bool
+    single_instance: bool
+    logging: bool
+
+
+@dataclass(order=True, slots=True)
+class SubsceneCookie:
+    """
+    Represents Subscene website preferences stored in a cookie.
+
+    Store various preferences of a user's Subscene preferences.
+    The cookie preferences include settings for dark theme, sorting subtitles by date,
+    language filter, hearing impaired filter, and foreign subtitles only.
+
+    Attributes:
+        dark_theme (bool): True if the user has enabled dark theme, False otherwise.
+        sort_subtitle_by_date (str): The preferred sorting option for subtitles by date.
+        language_filter (int): The language filter setting for subtitles.
+        hearing_impaired (int): The hearing impaired filter setting for subtitles.
+        foreign_only (bool): True if the user prefers foreign subtitles only, False otherwise.
+
+    Examples:
+        Creating a `SubsceneCookie` instance:
+
+        >>> cookie = SubsceneCookie(dark_theme=True, sort_subtitle_by_date=false,
+        ...                         language_filter=1, hearing_impaired=0, foreign_only=False)
+    """
+
+    dark_theme: bool
+    sort_subtitle_by_date: str
+    language_filter: int
+    hearing_impaired: int
+    foreigen_only: bool
+
+
+@dataclass(order=True, slots=True)
+class ReleaseData:
+    """
+    Data class representing data associated with a media release.
+
+    Attributes:
+        title (str): Title of the media.
+        year (int): Year of the media release.
+        season (str): Season of the media.
+        season_ordinal (str): Ordinal of the season.
+        episode (str): Episode of the media.
+        episode_ordinal (str): Ordinal of the episode.
+        tvseries (bool): Boolean flag indicating if the media is a TV series.
+        release (str): Name of the media release.
+        group (str): Name of the release group.
+    """
+
+    title: str
+    year: int
+    season: str
+    season_ordinal: str
+    episode: str
+    episode_ordinal: str
+    tvseries: bool
+    release: str
+    group: str
+
+
+@dataclass(order=True, slots=True)
+class ProviderUrls:
+    """
+    A dataclass to represent URLs for different subtitle providers.
+
+    Attributes:
+        subscene(str): URL of the subscene provider.
+        opensubtitles(str): URL of the opensubtitles provider.
+        opensubtitles_hash(str): Hash URL of the opensubtitles provider.
+        yifysubtitles(str): URL of the yifysubtitles provider.
+    """
+
+    subscene: str
+    opensubtitles: str
+    opensubtitles_hash: str
+    yifysubtitles: str
+
+
+@dataclass(order=True, slots=True)
+class Subtitle:
+    """
+    A data class representing download data for subtitle.
+
+    Attributes:
+        pct_result (str): How closely the release_name matches the release name of the video file.
+        provider (str): The subtitle provider used to obtain the subtitle file.
+        file_path (str): The path to the subtitle file on the local filesystem.
+        download_url (str): The URL from which the subtitle file can be downloaded from.
+    """
+
+    pct_result: int
+    provider: str
+    release_name: str
+    download_url: str
+
+
+@dataclass(order=True, frozen=True)
+class SystemInfo:
+    """
+    Represents system information.
+
+    This class is a data structure used to hold information about the system,
+    including the platform, mode, Python version, and subsearch.
+
+    Attributes:
+        platform (str): The platform or operating system of the system.
+        mode (str): The mode or state of the system.
+        python (str): The version of Python installed on the system.
+        subsearch (str): The subsearch associated with the system.
+
+    Examples:
+        Creating a `SystemInfo` instance:
+
+        >>> system_info = SystemInfo(platform="windows-10-10.0.22624-sp0", mode="interpreter", python="3.11.4", subsearch="2.37.1")
+    """
+
+    platform: str
+    mode: str
+    python: str
+    subsearch: str
```

### Comparing `Subsearch-2.37.1/src/subsearch/utils/update.py` & `Subsearch-2.38.0rc1/src/subsearch/utils/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import re
 
 import cloudscraper
-import requests
-import selectolax
 from packaging.version import Version
 
 from subsearch.data import __guid__, __version__
 
 
 def find_semantic_version(version: str) -> str:
     """
```

