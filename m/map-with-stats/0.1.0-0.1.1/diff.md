# Comparing `tmp/map_with_stats-0.1.0.tar.gz` & `tmp/map_with_stats-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_with_stats-0.1.0.tar", last modified: Tue May  9 12:34:21 2023, max compression
+gzip compressed data, was "map_with_stats-0.1.1.tar", last modified: Sat Jul 29 13:45:39 2023, max compression
```

## Comparing `map_with_stats-0.1.0.tar` & `map_with_stats-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/publish_prod.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/publish_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (123)  1021823 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/figs/map_screenshot.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/linux.env
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/environment/windows.env
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.892114 map_with_stats-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/src/map_with_stats/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/map.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/src/map_with_stats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/src/map_with_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 12:34:21.000000 map_with_stats-0.1.0/src/map_with_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:34:21.896114 map_with_stats-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-09 12:34:12.000000 map_with_stats-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.190817 map_with_stats-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.194817 map_with_stats-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/publish_prod.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/publish_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/assets/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/assets/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1021823 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/figs/map_screenshot.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/quick_start.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/linux.env
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/requirements_lib.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/windows.env
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.194817 map_with_stats-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/src/map_with_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/src/map_with_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/tests/test_utils.py
```

### Comparing `map_with_stats-0.1.0/.github/workflows/docs.yml` & `map_with_stats-0.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/.github/workflows/publish_template.yml` & `map_with_stats-0.1.1/.github/workflows/publish_template.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/.github/workflows/test.yml` & `map_with_stats-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/.gitignore` & `map_with_stats-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/.pre-commit-config.yaml` & `map_with_stats-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/.vscode/settings.json` & `map_with_stats-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/LICENSE` & `map_with_stats-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/PKG-INFO` & `map_with_stats-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: map_with_stats
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interactive map with a choropleth displaying some statistics as color per hectare
 Author: Mischa Lisovyi
 License: MIT License
         
         Copyright (c) 2023 Mischa Lisovyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,58 +54,22 @@
 [![typing](https://img.shields.io/badge/code%20typing-mypy-blue.svg)](http://mypy-lang.org/)
 [![docs](https://img.shields.io/badge/documentation-mkdocs--material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
 [![versioning](https://img.shields.io/badge/versioning-setuptools--scm-blue.svg)](https://github.com/pypa/setuptools_scm)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![documentation](https://img.shields.io/badge/_-documentation-blueviolet?logo=githubpages)](https://mlisovyi.github.io/map_with_stats)
 
 
-The package allows to display an interactive map with a choropleth
-displaying some statistics as color per hectare (100x100 meter square).
-
-The package is created and tested to work for the **Switzerland coordinates**,
-however, one could try to use it for any other map with hectare statistics.
+The package allows to display an **interactive map with a choropleth
+displaying some statistics as color per hectare** (100x100 meter square).
 
 ![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.jpeg)
 
+!!! question "What is the use-case?"
+
+      The typical use-case would be to visualise and do plausibility checks of hectare-level data
+      as well as to compare statistics between geographic areas.
+
+The package is created and tested to work for the **Switzerland coordinates**,
+however, one could try to use it for any other map with hectare statistics.
 
-## Installation
 
-```bash
-pip install map_with_stats
-```
-
-## Quick guide
-
-For visualisation you will need some statistics per hectare.
-Individual hectares are defined by the X,Y coordinates
-in the [LV03](https://en.wikipedia.org/wiki/Swiss_coordinate_system#LV03) coordinate system
-of the bottom-left (=south-west) corner.
-
-1. Such data could be for example downloaded from
-   the [BFS website](https://www.bfs.admin.ch/bfs/de/home/dienstleistungen/geostat/geodaten-bundesstatistik).
-   * For example, one can get population data per hectare for year 2021 from
-     [here](https://www.bfs.admin.ch/bfs/de/home/dienstleistungen/geostat/geodaten-bundesstatistik/gebaeude-wohnungen-haushalte-personen/bevoelkerung-haushalte-ab-2010.assetdetail.23528269.html).
-2. Download and extract _STATPOP2021.csv_ from the archive.
-3. Generate the HTML with the map:
-   ```python
-   import pandas as pd
-
-   import map_with_stats as mws
-
-
-   data_raw = pd.read_csv("STATPOP2021.csv", sep=";")
-   data = data_raw[["RELI", "B21BTOT"]]
-   # `hectare2xy` is a helper function that extracts X,Y coordinates from the hectare ID
-   data = mws.hectare2xy(data, "RELI")
-   # `create_geo_df_with_hectar_polygons` is a helper function that creates GeoDataFrame with a polygon for each hectare
-   gdf_stats = mws.create_geo_df_with_hectar_polygons(data, "B21BTOT", crs_out="EPSG:4326")
-
-   # restrict data to the Zürich neighbourhood - this step is optional
-   mask_x = data["X"].between(6700_00, 7000_00)
-   mask_y = data["Y"].between(2330_00, 2630_00)
-   gdf = gdf_stats[mask_x & mask_y]
-
-   # `build_map` is the main helper function that will create a map with a coropleth layer
-   title = "Dummy data"  # the to be used as data description in the tooltip and colormap
-   map = mws.build_map(gdf, title, "equidistant", n_bins=5)
-   map.save("map.html")
-   ```
+Read about usage in [Quick start guide](https://mlisovyi.github.io/map_with_stats/quick_start)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `map_with_stats-0.1.0/README.md` & `map_with_stats-0.1.1/src/map_with_stats.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,49 @@
+Metadata-Version: 2.1
+Name: map-with-stats
+Version: 0.1.1
+Summary: Interactive map with a choropleth displaying some statistics as color per hectare
+Author: Mischa Lisovyi
+License: MIT License
+        
+        Copyright (c) 2023 Mischa Lisovyi
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/mlisovyi/map_with_stats
+Project-URL: Documentation, https://mlisovyi.github.io/map_with_stats/
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Map with statistics
 
 
 <!-- [![coverage report](https://git.intern.migros.net/analytics/optimizers/store_profile_common/badges/main/coverage.svg)](https://git.intern.migros.net/analytics/optimizers/store_profile_common/-/commits/main) -->
 [![release @ PYPI](http://img.shields.io/pypi/v/map_with_stats?color=brightgreen&logo=pypi&logoColor=949DA5)](https://pypi.python.org/pypi/map_with_stats)
 [![python version](https://img.shields.io/badge/python-3.7,3.8,3.9,3.10,3.11-blue.svg?logo=python&logoColor=949DA5)](https://www.python.org/downloads/)
 ![platform](https://img.shields.io/badge/platform-linux%20|%20macos%20|%20windows-lightgray.svg)
@@ -12,58 +54,22 @@
 [![typing](https://img.shields.io/badge/code%20typing-mypy-blue.svg)](http://mypy-lang.org/)
 [![docs](https://img.shields.io/badge/documentation-mkdocs--material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
 [![versioning](https://img.shields.io/badge/versioning-setuptools--scm-blue.svg)](https://github.com/pypa/setuptools_scm)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![documentation](https://img.shields.io/badge/_-documentation-blueviolet?logo=githubpages)](https://mlisovyi.github.io/map_with_stats)
 
 
-The package allows to display an interactive map with a choropleth
-displaying some statistics as color per hectare (100x100 meter square).
-
-The package is created and tested to work for the **Switzerland coordinates**,
-however, one could try to use it for any other map with hectare statistics.
+The package allows to display an **interactive map with a choropleth
+displaying some statistics as color per hectare** (100x100 meter square).
 
 ![Example map](https://github.com/mlisovyi/map_with_stats/raw/main/docs/figs/map_screenshot.jpeg)
 
+!!! question "What is the use-case?"
+
+      The typical use-case would be to visualise and do plausibility checks of hectare-level data
+      as well as to compare statistics between geographic areas.
+
+The package is created and tested to work for the **Switzerland coordinates**,
+however, one could try to use it for any other map with hectare statistics.
 
-## Installation
 
-```bash
-pip install map_with_stats
-```
-
-## Quick guide
-
-For visualisation you will need some statistics per hectare.
-Individual hectares are defined by the X,Y coordinates
-in the [LV03](https://en.wikipedia.org/wiki/Swiss_coordinate_system#LV03) coordinate system
-of the bottom-left (=south-west) corner.
-
-1. Such data could be for example downloaded from
-   the [BFS website](https://www.bfs.admin.ch/bfs/de/home/dienstleistungen/geostat/geodaten-bundesstatistik).
-   * For example, one can get population data per hectare for year 2021 from
-     [here](https://www.bfs.admin.ch/bfs/de/home/dienstleistungen/geostat/geodaten-bundesstatistik/gebaeude-wohnungen-haushalte-personen/bevoelkerung-haushalte-ab-2010.assetdetail.23528269.html).
-2. Download and extract _STATPOP2021.csv_ from the archive.
-3. Generate the HTML with the map:
-   ```python
-   import pandas as pd
-
-   import map_with_stats as mws
-
-
-   data_raw = pd.read_csv("STATPOP2021.csv", sep=";")
-   data = data_raw[["RELI", "B21BTOT"]]
-   # `hectare2xy` is a helper function that extracts X,Y coordinates from the hectare ID
-   data = mws.hectare2xy(data, "RELI")
-   # `create_geo_df_with_hectar_polygons` is a helper function that creates GeoDataFrame with a polygon for each hectare
-   gdf_stats = mws.create_geo_df_with_hectar_polygons(data, "B21BTOT", crs_out="EPSG:4326")
-
-   # restrict data to the Zürich neighbourhood - this step is optional
-   mask_x = data["X"].between(6700_00, 7000_00)
-   mask_y = data["Y"].between(2330_00, 2630_00)
-   gdf = gdf_stats[mask_x & mask_y]
-
-   # `build_map` is the main helper function that will create a map with a coropleth layer
-   title = "Dummy data"  # the to be used as data description in the tooltip and colormap
-   map = mws.build_map(gdf, title, "equidistant", n_bins=5)
-   map.save("map.html")
-   ```
+Read about usage in [Quick start guide](https://mlisovyi.github.io/map_with_stats/quick_start)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `map_with_stats-0.1.0/docs/figs/map_screenshot.jpeg` & `map_with_stats-0.1.1/docs/figs/map_screenshot.jpeg`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/mkdocs.yml` & `map_with_stats-0.1.1/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 # the title to use for the git repo link
 repo_name: "map_with_stats"
 # relative path to the markdown files on github
 edit_uri: blob/main/docs/
 
 nav:
   - Introduction: "index.md"
+  - Quick start guide: "quick_start.md"
   - FAQ: "faq.md"
   - API: "api.md"
 
 theme:
   name: material
-  # icon:
-  #   repo: fontawesome/brands/gitlab
   features:
     # enables annotations, see https://squidfunk.github.io/mkdocs-material/reference/code-blocks/#code-annotations
     - content.code.annotate
     # for navigation features see https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/
     - navigation.top
     - navigation.tracking
     # keep all sections in the navigation expanded by default
     - navigation.expand
     # add icon and link to the document on gihub for each page
     - content.action.edit
   icon:
+    logo: fontawesome/solid/map
     # icon for the git repository link on the top-right
     repo: fontawesome/brands/github
     # icon for the view of the current page in the repository
     edit: material/eye
+  favicon: assets/favicon-32x32.png
   palette:
     # light mode
     - media: "(prefers-color-scheme: light)"
       scheme: default
       # main theme color
       primary: deep orange
       # the color to change to for a hover on an interactive element
@@ -77,7 +78,12 @@
       handlers:
         python:
           # where to look for python modules. not strictly required, but helps, if building from an arbitrary folder
           paths: [src]
           options:
             docstring_style: google
             show_if_no_docstring: True
+            show_root_toc_entry: False
+
+# auto-reload on changes in the following folders outside of the docs (for development of docs)
+watch:
+  - src
```

### Comparing `map_with_stats-0.1.0/pyproject.toml` & `map_with_stats-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -55,30 +55,16 @@
 filterwarnings = ["ignore::FutureWarning", "ignore::pytest.PytestDeprecationWarning"]
 testpaths=["tests"]
 
 [tool.coverage.run]
 # skip module and any further custom files
 omit =["*/__init__.py", "_version.py"]
 
-# # Tool to install the package and run test in various python versions
-# [tox:tox]
-# # various python environments to run in. The names here have to be aligned with tox execution in CI/CD
-# envlist = python3.6,python3.7,python3.8,python3.10
-# # required for a package that can be installed
-# isolated_build = True
-
-# [testenv]
-# deps =
-#     pytest
-#     pytest-cov
-# commands = pytest {posargs} # substitute with tox' positional arguments
-
 [tool.mypy]
 # What files should be included.
-# This is a list of files/folders.
 files =["src"]
 # We want to be as strict as possible but allow reexports
 strict = true
 implicit_reexport = true
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `map_with_stats-0.1.0/src/map_with_stats.egg-info/SOURCES.txt` & `map_with_stats-0.1.1/src/map_with_stats.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 .github/workflows/publish_template.yml
 .github/workflows/publish_test.yml
 .github/workflows/test.yml
 .vscode/settings.json
 docs/api.md
 docs/faq.md
 docs/index.md
+docs/quick_start.md
+docs/assets/favicon-16x16.png
+docs/assets/favicon-32x32.png
 docs/figs/map_screenshot.jpeg
 environment/linux.env
 environment/requirements_dev.txt
 environment/requirements_lib.txt
 environment/windows.env
 src/map_with_stats/__init__.py
 src/map_with_stats/_version.py
```

### Comparing `map_with_stats-0.1.0/tests/test_data.py` & `map_with_stats-0.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.0/tests/test_utils.py` & `map_with_stats-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

