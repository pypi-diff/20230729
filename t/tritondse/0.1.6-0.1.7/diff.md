# Comparing `tmp/tritondse-0.1.6.tar.gz` & `tmp/tritondse-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritondse-0.1.6.tar", last modified: Wed Jul 26 09:32:36 2023, max compression
+gzip compressed data, was "tritondse-0.1.7.tar", last modified: Sat Jul 29 12:32:53 2023, max compression
```

## Comparing `tritondse-0.1.6.tar` & `tritondse-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 09:32:34.000000 tritondse-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-26 09:32:36.062479 tritondse-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-26 09:32:34.000000 tritondse-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:32:36.062479 tritondse-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-26 09:32:34.000000 tritondse-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/heap_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/cle_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/quokkaprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse/probes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/probes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/probes/basic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    52218 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/process_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/qbdi_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/sanitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/seeds_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    36666 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/symbolic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/symbolic_explorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/thread_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 12:32:50.000000 tritondse-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 12:32:53.871581 tritondse-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-29 12:32:50.000000 tritondse-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:32:53.871581 tritondse-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 12:32:50.000000 tritondse-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.867581 tritondse-0.1.7/tritondse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/heap_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/tritondse/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/cle_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/loaders/quokkaprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/tritondse/probes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/probes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/probes/basic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52218 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/process_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/qbdi_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/sanitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/seeds_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36666 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/symbolic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/symbolic_explorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/thread_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-29 12:32:50.000000 tritondse-0.1.7/tritondse/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:32:53.871581 tritondse-0.1.7/tritondse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 12:32:53.000000 tritondse-0.1.7/tritondse.egg-info/top_level.txt
```

### Comparing `tritondse-0.1.6/LICENSE` & `tritondse-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/PKG-INFO` & `tritondse-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.6 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.7 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.6/README.md` & `tritondse-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/setup.py` & `tritondse-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md") as f:
     README = f.read()
 
 
 setup(
     name="tritondse",
-    version="0.1.6",
+    version="0.1.7",
     description="A library of Dynamic Symbolic Exploration based the Triton library",
     packages=find_packages(),
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/quarkslab/tritondse",
     project_urls={
         "Documentation": "https://quarkslab.github.io/tritondse/",
```

### Comparing `tritondse-0.1.6/tritondse/__init__.py` & `tritondse-0.1.7/tritondse/__init__.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/arch.py` & `tritondse-0.1.7/tritondse/arch.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/callbacks.py` & `tritondse-0.1.7/tritondse/callbacks.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/config.py` & `tritondse-0.1.7/tritondse/config.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/coverage.py` & `tritondse-0.1.7/tritondse/coverage.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/exception.py` & `tritondse-0.1.7/tritondse/exception.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/heap_allocator.py` & `tritondse-0.1.7/tritondse/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/loaders/cle_loader.py` & `tritondse-0.1.7/tritondse/loaders/cle_loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/loaders/loader.py` & `tritondse-0.1.7/tritondse/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/loaders/program.py` & `tritondse-0.1.7/tritondse/loaders/program.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/loaders/quokkaprogram.py` & `tritondse-0.1.7/tritondse/loaders/quokkaprogram.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/logging.py` & `tritondse-0.1.7/tritondse/logging.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/memory.py` & `tritondse-0.1.7/tritondse/memory.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/probes/basic_trace.py` & `tritondse-0.1.7/tritondse/probes/basic_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/process_state.py` & `tritondse-0.1.7/tritondse/process_state.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/qbdi_trace.py` & `tritondse-0.1.7/tritondse/qbdi_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/routines.py` & `tritondse-0.1.7/tritondse/routines.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/sanitizers.py` & `tritondse-0.1.7/tritondse/sanitizers.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/seed.py` & `tritondse-0.1.7/tritondse/seed.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/seeds_manager.py` & `tritondse-0.1.7/tritondse/seeds_manager.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/symbolic_executor.py` & `tritondse-0.1.7/tritondse/symbolic_executor.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/symbolic_explorator.py` & `tritondse-0.1.7/tritondse/symbolic_explorator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/thread_context.py` & `tritondse-0.1.7/tritondse/thread_context.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/trace.py` & `tritondse-0.1.7/tritondse/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # built-in imports
 import json
 import os
 import subprocess
 from pathlib import Path
+import time
 from typing import List, Optional, Union
 from collections import Counter
 
 
 # local imports
 import tritondse # NOTE We need this import so we can use it to determine the path of this file.
 from tritondse import Config, Program, SymbolicExecutor, CoverageStrategy, CoverageSingleRun
@@ -126,15 +127,16 @@
             raise FileNotFoundError()
 
         if stdin_file and not Path(stdin_file).exists():
             raise FileNotFoundError()
 
         args = [] if not args else args
 
-        cmdlne = f'python -m pyqbdipreload {QBDITrace.QBDI_SCRIPT_FILEPATH}'.split(' ') + [binary_path] + args
+        cmdlne = f'timeout {timeout} python -m pyqbdipreload {QBDITrace.QBDI_SCRIPT_FILEPATH}'.split(' ') + [binary_path] + args
+        cmdlne = " ".join(cmdlne)
 
         logger.debug(f'Command line: {" ".join(cmdlne)}')
 
         # Set environment variables.
         environ = {
             'PYQBDIPRELOAD_COVERAGE_STRATEGY': strategy.name,
             'PYQBDIPRELOAD_OUTPUT_FILEPATH': output_path,
@@ -143,24 +145,30 @@
         }
         environ.update(os.environ)
 
         # Open stdin file if it is present.
         stdin_fp = open(stdin_file, 'rb') if stdin_file else None
 
         # Run QBDI tool.
-        process = subprocess.Popen(cmdlne, stdin=stdin_fp, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=cwd, env=environ)
+        process = subprocess.Popen(cmdlne,
+                                   shell=True,
+                                   stdin=stdin_fp,
+                                   stdout=subprocess.DEVNULL,
+                                   stderr=subprocess.DEVNULL,
+                                   cwd=cwd,
+                                   env=environ)
         try:
             stdout, stderr = process.communicate(timeout=timeout)
-            for line in stdout.split(b"\n"):
-                logger.debug(f"stdout: {line}")
-            for line in stderr.split(b"\n"):
-                logger.debug(f"stdout: {line}")
+            # for line in stdout.split(b"\n"):
+            #     logger.debug(f"stdout: {line}")
+            # for line in stderr.split(b"\n"):
+            #     logger.debug(f"stdout: {line}")
         except subprocess.TimeoutExpired:
             process.wait()
-            logger.error('QBDI tracer timeout expired!')
+            # logger.warning('QBDI tracer timeout expired!')
             raise TraceException('QBDI tracer timeout expired')
 
         if stdin_fp:
             stdin_fp.close()
 
         return Path(output_path).exists()
```

### Comparing `tritondse-0.1.6/tritondse/types.py` & `tritondse-0.1.7/tritondse/types.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/worklist.py` & `tritondse-0.1.7/tritondse/worklist.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse/workspace.py` & `tritondse-0.1.7/tritondse/workspace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.6/tritondse.egg-info/PKG-INFO` & `tritondse-0.1.7/tritondse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.6 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.7 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.6/tritondse.egg-info/SOURCES.txt` & `tritondse-0.1.7/tritondse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

