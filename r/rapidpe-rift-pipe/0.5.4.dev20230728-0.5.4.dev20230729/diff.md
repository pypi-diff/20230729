# Comparing `tmp/rapidpe_rift_pipe-0.5.4.dev20230728.tar.gz` & `tmp/rapidpe_rift_pipe-0.5.4.dev20230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230728.tar", last modified: Fri Jul 28 05:15:21 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230729.tar", last modified: Sat Jul 29 05:16:02 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.5.4.dev20230728.tar` & `rapidpe_rift_pipe-0.5.4.dev20230729.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.253297 rapidpe_rift_pipe-0.5.4.dev20230728/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-28 05:15:21.253297 rapidpe_rift_pipe-0.5.4.dev20230728/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.246297 rapidpe_rift_pipe-0.5.4.dev20230728/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.248297 rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-28 05:15:21.253297 rapidpe_rift_pipe-0.5.4.dev20230728/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.246297 rapidpe_rift_pipe-0.5.4.dev20230728/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.251297 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.252297 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 05:15:08.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.252297 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 05:15:08.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31210 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.252297 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 05:15:08.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 05:15:21.252297 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-28 05:15:21.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-28 05:15:21.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 05:15:21.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-28 05:15:21.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-28 05:15:21.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 05:15:21.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 05:15:21.000000 rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.445280 rapidpe_rift_pipe-0.5.4.dev20230729/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-29 05:16:02.445280 rapidpe_rift_pipe-0.5.4.dev20230729/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.438280 rapidpe_rift_pipe-0.5.4.dev20230729/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.440280 rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-29 05:16:02.446280 rapidpe_rift_pipe-0.5.4.dev20230729/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.438280 rapidpe_rift_pipe-0.5.4.dev20230729/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.443280 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.444280 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.445280 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31210 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.445280 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 05:15:50.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-26 05:13:43.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:16:02.444280 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-29 05:16:02.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-29 05:16:02.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 05:16:02.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-29 05:16:02.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-29 05:16:02.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 05:16:02.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 05:16:02.000000 rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/COPYING` & `rapidpe_rift_pipe-0.5.4.dev20230729/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230729/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.5.4.dev20230728
+Version: 0.5.4.dev20230729
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/setup.cfg` & `rapidpe_rift_pipe-0.5.4.dev20230729/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230728
+tag_build = dev.20230729
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.5.4.dev20230728
+Version: 0.5.4.dev20230729
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230728/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.5.4.dev20230729/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

