# Comparing `tmp/yet_another_wizz_cli-1.2.4.tar.gz` & `tmp/yet_another_wizz_cli-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz_cli-1.2.4.tar", last modified: Thu Jul 20 13:12:10 2023, max compression
+gzip compressed data, was "yet_another_wizz_cli-1.2.5.tar", last modified: Fri Jul 28 22:42:32 2023, max compression
```

## Comparing `yet_another_wizz_cli-1.2.4.tar` & `yet_another_wizz_cli-1.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.764617 yet_another_wizz_cli-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.764617 yet_another_wizz_cli-1.2.4/src/yaw_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.764617 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17491 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/default_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-07-20 13:11:56.000000 yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:12:10.768617 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 13:12:10.000000 yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.322504 yet_another_wizz_cli-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-07-28 22:42:20.000000 yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:42:32.326504 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 22:42:32.000000 yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/top_level.txt
```

### Comparing `yet_another_wizz_cli-1.2.4/LICENSE` & `yet_another_wizz_cli-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/PKG-INFO` & `yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yet_another_wizz_cli
-Version: 1.2.4
+Name: yet-another-wizz-cli
+Version: 1.2.5
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -113,15 +113,16 @@
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz_cli/issues
 
 
-**Maintainers:**
+Maintainers
+-----------
 
 - Jan Luca van den Busch
   (*author*, Ruhr-Universität Bochum, Astronomisches Institut)
 
 
 Acknowledgements
 ----------------
```

### Comparing `yet_another_wizz_cli-1.2.4/README.rst` & `yet_another_wizz_cli-1.2.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,16 @@
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz_cli/issues
 
 
-**Maintainers:**
+Maintainers
+-----------
 
 - Jan Luca van den Busch
   (*author*, Ruhr-Universität Bochum, Astronomisches Institut)
 
 
 Acknowledgements
 ----------------
```

### Comparing `yet_another_wizz_cli-1.2.4/pyproject.toml` & `yet_another_wizz_cli-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 requires-python = ">=3.8"
 dependencies = [
     "numpy",
     "pandas",
     "pyyaml",
     "matplotlib",
-    "yet-another-wizz>=2.5.2",
+    "yet-another-wizz>=2.5.5",
 ]
 
 [project.scripts]
 yaw_cli = "yaw_cli:Commandline.main"
 
 [project.optional-dependencies]
 plot = ["matplotlib"]
```

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/main.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/main.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/subcommands.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/subcommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,15 @@
         )
         populate_parser(yaw_config.ScalesConfig, group_scales)
 
         group_bins = parser.add_argument_group(
             title="redshift binning",
             description="sets the redshift binning for the clustering redshifts",
         )
-        populate_parser(yaw_config.AutoBinningConfig, group_bins)
-        populate_parser(yaw_config.ManualBinningConfig, group_bins)
+        populate_parser(yaw_config.BinningConfig, group_bins)
 
         group_backend = parser.add_argument_group(
             title="backend specific",
             description="parameters that are specific to pair counting backends",
         )
         populate_parser(yaw_config.BackendConfig, group_backend)
```

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/commandline/utils.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/commandline/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/__init__.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/data.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/data.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/default_setup.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/default_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,15 @@
 
     setup_default += format_line(
         "binning:",
         "specify the redshift binning for the clustering redshifts",
         indents=1,
         width=width,
     )
-    setup_default += make_doc(config.AutoBinningConfig, indent=2, width=width)
-    setup_default += make_doc(config.ManualBinningConfig, indent=2, width=width)
+    setup_default += make_doc(config.BinningConfig, indent=2, width=width)
 
     setup_default += format_line(
         "scales:", "specify the correlation measurement scales", indents=1, width=width
     )
     setup_default += make_doc(config.ScalesConfig, indent=2, width=width)
 
     setup_default += make_doc(config.Configuration, indent=1, width=width)
```

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/directories.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/directories.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/logger.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/logger.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/merge.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import Iterable, Sequence
 from itertools import groupby
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
-from yaw.config import OPTIONS, Configuration, ManualBinningConfig, ScalesConfig
+from yaw.config import OPTIONS, BinningConfig, Configuration, ScalesConfig
 from yaw.config import default as DEFAULT
 from yaw.core.utils import TypePathStr
 from yaw.correlation import CorrFunc
 from yaw.redshifts import HistData
 
 from yaw_cli.pipeline.project import (
     ProjectDirectory,
@@ -75,15 +75,15 @@
     extra = set.union(*scale_sets) - common
     if len(extra) > 0:
         logger.warning("ignoring unmatched scales: %s", ", ".join(extra))
 
     # merge binning
     if merge_binning:
         bins = np.unique(np.concatenate(bins))
-        bin_config = ManualBinningConfig(bins)
+        bin_config = BinningConfig.create(zbins=bins)
         if bin_config.zbin_num != n_bins:
             raise MergeError("cannot concatenate bins contiguously")
     else:
         bin_config = config.binning  # all identical
 
     config = Configuration(
         scales=ScalesConfig(
```

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/plot.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/plot.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/processing.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/processing.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/project.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/project.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yaw_cli/pipeline/tasks.py` & `yet_another_wizz_cli-1.2.5/src/yaw_cli/pipeline/tasks.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/PKG-INFO` & `yet_another_wizz_cli-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yet-another-wizz-cli
-Version: 1.2.4
+Name: yet_another_wizz_cli
+Version: 1.2.5
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -113,15 +113,16 @@
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz_cli/issues
 
 
-**Maintainers:**
+Maintainers
+-----------
 
 - Jan Luca van den Busch
   (*author*, Ruhr-Universität Bochum, Astronomisches Institut)
 
 
 Acknowledgements
 ----------------
```

### Comparing `yet_another_wizz_cli-1.2.4/src/yet_another_wizz_cli.egg-info/SOURCES.txt` & `yet_another_wizz_cli-1.2.5/src/yet_another_wizz_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

