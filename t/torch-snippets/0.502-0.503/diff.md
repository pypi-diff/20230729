# Comparing `tmp/torch_snippets-0.502.tar.gz` & `tmp/torch_snippets-0.503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_snippets-0.502.tar", last modified: Thu Jul 27 07:13:37 2023, max compression
+gzip compressed data, was "torch_snippets-0.503.tar", last modified: Sat Jul 29 08:46:50 2023, max compression
```

## Comparing `torch_snippets-0.502.tar` & `torch_snippets-0.503.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-27 07:13:37.476980 torch_snippets-0.502/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.502/LICENSE
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.502/LICENSE.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.502/MANIFEST.in
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-27 07:13:37.477219 torch_snippets-0.502/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.502/README.md
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      862 2023-07-27 07:11:45.000000 torch_snippets-0.502/settings.ini
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2023-07-27 07:13:37.478426 torch_snippets-0.502/setup.cfg
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.502/setup.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-27 07:13:37.469390 torch_snippets-0.502/torch_snippets/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      307 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    46129 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/_modidx.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.502/torch_snippets/_nbdev.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/adapters.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12112 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/bb_utils.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/bokeh_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/charts.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1539 2023-07-26 06:38:17.000000 torch_snippets-0.502/torch_snippets/dates.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/decorators.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.502/torch_snippets/fastcores.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/imgaug_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/inspector.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8376 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/interactive_show.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4662 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/ipython.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/load_defaults.py
--rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    20928 2023-07-26 06:29:56.000000 torch_snippets-0.502/torch_snippets/loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3840 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/logger.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7573 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/markup.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1657 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/misc.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9763 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/paths.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1370 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/pdf_loader.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/registry.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/sklegos.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2023-06-10 19:35:22.000000 torch_snippets-0.502/torch_snippets/text_utils.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-27 07:13:37.474580 torch_snippets-0.502/torch_snippets/thinc_parser/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/thinc_parser/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.502/torch_snippets/thinc_parser/parser.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.502/torch_snippets/torch_loader.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-27 07:13:37.476238 torch_snippets-0.502/torch_snippets/trainer/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/trainer/__init__.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6802 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/trainer/capsule.py
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1537 2023-07-27 07:13:35.000000 torch_snippets-0.502/torch_snippets/trainer/config.py
-drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-27 07:13:37.473378 torch_snippets-0.502/torch_snippets.egg-info/
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-27 07:13:37.000000 torch_snippets-0.502/torch_snippets.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1165 2023-07-27 07:13:37.000000 torch_snippets-0.502/torch_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2023-07-27 07:13:37.000000 torch_snippets-0.502/torch_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.502/torch_snippets.egg-info/not-zip-safe
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      272 2023-07-27 07:13:37.000000 torch_snippets-0.502/torch_snippets.egg-info/requires.txt
--rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2023-07-27 07:13:37.000000 torch_snippets-0.502/torch_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-29 08:46:50.192240 torch_snippets-0.503/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    11357 2021-12-31 15:06:08.000000 torch_snippets-0.503/LICENSE
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1062 2023-01-17 16:58:23.000000 torch_snippets-0.503/LICENSE.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      111 2021-12-31 15:06:08.000000 torch_snippets-0.503/MANIFEST.in
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-29 08:46:50.192514 torch_snippets-0.503/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4999 2023-01-17 16:58:23.000000 torch_snippets-0.503/README.md
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      862 2023-07-29 08:46:12.000000 torch_snippets-0.503/settings.ini
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       79 2023-07-29 08:46:50.193375 torch_snippets-0.503/setup.cfg
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     2001 2022-06-03 13:10:38.000000 torch_snippets-0.503/setup.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-29 08:46:50.183663 torch_snippets-0.503/torch_snippets/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      307 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    46129 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/_modidx.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4482 2023-01-17 16:58:25.000000 torch_snippets-0.503/torch_snippets/_nbdev.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6211 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/adapters.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    12112 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/bb_utils.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1436 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/bokeh_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1672 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/charts.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1776 2023-07-28 07:38:37.000000 torch_snippets-0.503/torch_snippets/dates.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1206 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/decorators.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       73 2022-05-07 11:30:59.000000 torch_snippets-0.503/torch_snippets/fastcores.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4126 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/imgaug_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3429 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/inspector.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     8376 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/interactive_show.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     4662 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/ipython.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      597 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/load_defaults.py
+-rwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    20970 2023-07-27 07:32:05.000000 torch_snippets-0.503/torch_snippets/loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     3840 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/logger.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     7573 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/markup.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1657 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/misc.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     9763 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/paths.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1465 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/pdf_loader.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      822 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/registry.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6144 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/sklegos.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    14237 2023-06-10 19:35:22.000000 torch_snippets-0.503/torch_snippets/text_utils.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-29 08:46:50.189713 torch_snippets-0.503/torch_snippets/thinc_parser/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/thinc_parser/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1082 2022-10-16 17:20:20.000000 torch_snippets-0.503/torch_snippets/thinc_parser/parser.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)    13258 2022-11-08 11:22:58.000000 torch_snippets-0.503/torch_snippets/torch_loader.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-29 08:46:50.191610 torch_snippets-0.503/torch_snippets/trainer/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       23 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/trainer/__init__.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     6802 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/trainer/capsule.py
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1537 2023-07-29 08:46:47.000000 torch_snippets-0.503/torch_snippets/trainer/config.py
+drwxr-xr-x   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-07-29 08:46:50.188012 torch_snippets-0.503/torch_snippets.egg-info/
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     5691 2023-07-29 08:46:49.000000 torch_snippets-0.503/torch_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)     1165 2023-07-29 08:46:50.000000 torch_snippets-0.503/torch_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        1 2023-07-29 08:46:49.000000 torch_snippets-0.503/torch_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)        0 2023-01-17 16:58:23.000000 torch_snippets-0.503/torch_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)      272 2023-07-29 08:46:49.000000 torch_snippets-0.503/torch_snippets.egg-info/requires.txt
+-rw-r--r--   0 yeshwanth.y (1703077310) IN\Domain Users (826136866)       15 2023-07-29 08:46:49.000000 torch_snippets-0.503/torch_snippets.egg-info/top_level.txt
```

### Comparing `torch_snippets-0.502/LICENSE` & `torch_snippets-0.503/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/LICENSE.txt` & `torch_snippets-0.503/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/PKG-INFO` & `torch_snippets-0.503/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_snippets
-Version: 0.502
+Version: 0.503
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.502/README.md` & `torch_snippets-0.503/README.md`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/settings.ini` & `torch_snippets-0.503/settings.ini`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = sizhky
 description = One line functions for common tasks
 keywords = snippets, torch
 author = Yeshwanth Reddy
 author_email = 1992chinna@gmail.com
 copyright = sizhky
 branch = master
-version = 0.502
+version = 0.503
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = fastcore matplotlib Pillow altair dill ipython loguru numpy pandas tqdm rich PyYAML catalogue confection pydantic typing srsly typing_extensions wasabi jsonlines imgaug>=0.4.0 xmltodict fuzzywuzzy scikit-learn nltk python-Levenshtein pre-commit pymupdf nbconvert nbformat
```

### Comparing `torch_snippets-0.502/setup.py` & `torch_snippets-0.503/setup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/_modidx.py` & `torch_snippets-0.503/torch_snippets/_modidx.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/_nbdev.py` & `torch_snippets-0.503/torch_snippets/_nbdev.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/adapters.py` & `torch_snippets-0.503/torch_snippets/adapters.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/bb_utils.py` & `torch_snippets-0.503/torch_snippets/bb_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/bokeh_loader.py` & `torch_snippets-0.503/torch_snippets/bokeh_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/charts.py` & `torch_snippets-0.503/torch_snippets/charts.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/dates.py` & `torch_snippets-0.503/torch_snippets/dates.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import datetime
+from datetime import datetime
 from torch_snippets.loader import flatten, Debug
 from itertools import combinations_with_replacement
-from torch_snippets import io
 
 x = flatten(
     [
         [
             "%d{s1}%m{s2}%Y".format(s1=s1, s2=s2),
             "%Y{s1}%m{s2}%d".format(s1=s1, s2=s2),
             "%d{s1}%b{s2}%Y".format(s1=s1, s2=s2),
@@ -19,29 +18,42 @@
 x = x + [_x.replace("%Y", "%y") for _x in x]
 x = x + [_x.replace("%d", "%-d") for _x in x]
 x = x + [_x.replace("%m", "%-m") for _x in x]
 
 ALL_DATE_FORMATS = x + ["%Y-%m-%d %H:%M:%S"]
 
 
-@io
 def make_uniform_date_format(value, target_fmt="%d.%m.%Y", mode="raise"):
     available_modes = ["raise", "return", "default"]
-    if isinstance(value, datetime.datetime):
+    if isinstance(value, datetime):
         return value.strftime(target_fmt)
     for fmt in ALL_DATE_FORMATS:
         try:
-            output = datetime.datetime.strptime(value, fmt).strftime(target_fmt)
+            output = datetime.strptime(value, fmt).strftime(target_fmt)
             Debug(f"{value=}, {output=}, {fmt=}")
             return output
         except:
             ...
     if mode == "raise":
         raise NotImplementedError(f"Unable to give a proper date for `{value}`")
     elif mode in {"return"}:
         return None
     elif mode == "default":
         return "01.01.1900"
     else:
         raise NotImplementedError(
             f"`mode` can only be one of {available_modes} (Case sensitive)"
         )
+
+
+def are_dates_equal(date1, date2):
+    try:
+        date1 = make_uniform_date_format(date1)
+        date2 = make_uniform_date_format(date2)
+
+        return date1 == date2
+    except:
+        return False
+
+
+def today(fmt="%Y%m%d"):
+    return datetime.today().strftime(fmt)
```

### Comparing `torch_snippets-0.502/torch_snippets/decorators.py` & `torch_snippets-0.503/torch_snippets/decorators.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/imgaug_loader.py` & `torch_snippets-0.503/torch_snippets/imgaug_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/inspector.py` & `torch_snippets-0.503/torch_snippets/inspector.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/interactive_show.py` & `torch_snippets-0.503/torch_snippets/interactive_show.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/ipython.py` & `torch_snippets-0.503/torch_snippets/ipython.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/load_defaults.py` & `torch_snippets-0.503/torch_snippets/load_defaults.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/loader.py` & `torch_snippets-0.503/torch_snippets/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,15 @@
     **kwargs,
 ):
     "show an image"
 
     try:
         if isinstance(img, (str, Path)):
             img = read(str(img), 1)
+        if isinstance(img, torch.Tensor):
             img = img.cpu().detach().numpy().copy()
         if isinstance(img, PIL.Image.Image):
             img = np.array(img)
 
     except Exception as e:
         print(e)
     if isinstance(img, pd.DataFrame):
```

### Comparing `torch_snippets-0.502/torch_snippets/logger.py` & `torch_snippets-0.503/torch_snippets/logger.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/markup.py` & `torch_snippets-0.503/torch_snippets/markup.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/misc.py` & `torch_snippets-0.503/torch_snippets/misc.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/paths.py` & `torch_snippets-0.503/torch_snippets/paths.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/pdf_loader.py` & `torch_snippets-0.503/torch_snippets/pdf_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/pdf.ipynb.
 
 # %% auto 0
 __all__ = ['PDF']
 
 # %% ../nbs/pdf.ipynb 2
 from .loader import np, subplots, show, resize, L, Image
+from fastcore.basics import ifnone
 import fitz
 
 # %% ../nbs/pdf.ipynb 3
 class PDF:
     """Load a PDF file from `path` as a list of images
     Use `show` function to see the images
     **WIP**"""
 
-    def __init__(self, path, dfs=None):
+    def __init__(self, path, dfs=None, dpi=150):
         self.path = path
+        self.dpi = dpi
         self.doc = fitz.open(path)
         self.ims = L([self.get_image(page_no) for page_no in range(len(self))])
         self.dfs = L(dfs) if dfs is not None else L([None] * len(self))
 
-    def get_image(self, page_no):
+    def get_image(self, page_no, dpi=None):
         page = self.doc.load_page(page_no)
-        pix = page.get_pixmap(dpi=150)
+        pix = page.get_pixmap(dpi=ifnone(dpi, self.dpi))
         mode = "RGBA" if pix.alpha else "RGB"
         img = Image.frombytes(mode, [pix.width, pix.height], pix.samples)
         return img
 
     def __len__(self):
         return len(self.doc)
```

### Comparing `torch_snippets-0.502/torch_snippets/registry.py` & `torch_snippets-0.503/torch_snippets/registry.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/sklegos.py` & `torch_snippets-0.503/torch_snippets/sklegos.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/text_utils.py` & `torch_snippets-0.503/torch_snippets/text_utils.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/thinc_parser/parser.py` & `torch_snippets-0.503/torch_snippets/thinc_parser/parser.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/torch_loader.py` & `torch_snippets-0.503/torch_snippets/torch_loader.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/trainer/capsule.py` & `torch_snippets-0.503/torch_snippets/trainer/capsule.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets/trainer/config.py` & `torch_snippets-0.503/torch_snippets/trainer/config.py`

 * *Files identical despite different names*

### Comparing `torch_snippets-0.502/torch_snippets.egg-info/PKG-INFO` & `torch_snippets-0.503/torch_snippets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-snippets
-Version: 0.502
+Version: 0.503
 Summary: One line functions for common tasks
 Home-page: https://github.com/sizhky/torch_snippets/tree/master/
 Author: Yeshwanth Reddy
 Author-email: 1992chinna@gmail.com
 License: Apache Software License 2.0
 Keywords: snippets,torch
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torch_snippets-0.502/torch_snippets.egg-info/SOURCES.txt` & `torch_snippets-0.503/torch_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

