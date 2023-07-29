# Comparing `tmp/pyPhasesML-0.6.2.tar.gz` & `tmp/pyPhasesML-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.6.2.tar", last modified: Thu Jun  1 14:28:47 2023, max compression
+gzip compressed data, was "pyPhasesML-0.7.0.tar", last modified: Sat Jul 29 16:54:39 2023, max compression
```

## Comparing `pyPhasesML-0.6.2.tar` & `pyPhasesML-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.873707 pyPhasesML-0.6.2/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-06-01 14:28:47.872707 pyPhasesML-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.869707 pyPhasesML-0.6.2/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4491 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.870707 pyPhasesML-0.6.2/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    18506 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.871707 pyPhasesML-0.6.2/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.872707 pyPhasesML-0.6.2/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.872707 pyPhasesML-0.6.2/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    18685 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 14:28:47.870707 pyPhasesML-0.6.2/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-01 14:28:47.000000 pyPhasesML-0.6.2/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-06-01 14:28:30.000000 pyPhasesML-0.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 14:28:47.873707 pyPhasesML-0.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-01 14:28:31.000000 pyPhasesML-0.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.606605 pyPhasesML-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-29 16:54:39.606605 pyPhasesML-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.600605 pyPhasesML-0.7.0/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4077 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.602605 pyPhasesML-0.7.0/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.603605 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3654 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2582 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.604605 pyPhasesML-0.7.0/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.605605 pyPhasesML-0.7.0/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.605605 pyPhasesML-0.7.0/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.601605 pyPhasesML-0.7.0/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 16:54:39.606605 pyPhasesML-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-29 16:54:24.000000 pyPhasesML-0.7.0/setup.py
```

### Comparing `pyPhasesML-0.6.2/LICENSE` & `pyPhasesML-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/PKG-INFO` & `pyPhasesML-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 This Extension adds:
 - an Exporter for `PyTorch` and `TensorFlow` Models.
 - an Modelmanager that can handle `PyTorch` and `TensorFlow` Models
 
 
 ## Setup
 
-- add pyPhasesML to your dependencies or run `pipp install -U pyPhasesML`
+- add pyPhasesML to your dependencies or run `pip install -U pyPhasesML`
 - add `pyPhasesML` to your plugins in the main project config f.e: in your `project.yaml`
 ```yaml
 name: bumpDetector
 namespace: ibmt.tud
 
 # load machine learning plugin
 plugins:
```

### Comparing `pyPhasesML-0.6.2/README.md` & `pyPhasesML-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This Extension adds:
 - an Exporter for `PyTorch` and `TensorFlow` Models.
 - an Modelmanager that can handle `PyTorch` and `TensorFlow` Models
 
 
 ## Setup
 
-- add pyPhasesML to your dependencies or run `pipp install -U pyPhasesML`
+- add pyPhasesML to your dependencies or run `pip install -U pyPhasesML`
 - add `pyPhasesML` to your plugins in the main project config f.e: in your `project.yaml`
 ```yaml
 name: bumpDetector
 namespace: ibmt.tud
 
 # load machine learning plugin
 plugins:
```

### Comparing `pyPhasesML-0.6.2/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.7.0/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/DataSet.py` & `pyPhasesML-0.7.0/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.7.0/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.7.0/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/Model.py` & `pyPhasesML-0.7.0/pyPhasesML/Model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import csv
 from abc import ABC, abstractmethod
 from pathlib import Path
+import signal
 
 from pyPhases.util.Optionizable import Optionizable
 from pyPhases.util.EventBus import EventBus
 
 from .DataSet import DataSet
 
 
 class MetricsDoesNotExist(Exception):
     pass
 
 class AdapterNotImplemented(Exception):
     pass
 
+class ModelConfig:
+    def __init__(self):
+        self.optimizerId = "adams"
+        self.learningRate = 0.001
+        self.learningRateDecay = None
+        self.stopAfterNotImproving = None
+        
+        # cyclic lr
+        self.cycleLRDivisor = 4  # minLR = lr / cycleLRFactor
+        
+        # logging
+        self.logPath = "logs"
+        self.csvLogFile = "log.csv"
 
 class Model(ABC, Optionizable, EventBus):
     metrics = {
         "acc": {"name": "acc", "type": "max"},
         "binary_accuracy": {"name": "binary_accuracy", "type": "max"},
         "accuracy": {"name": "accuracy", "type": "max"},
         "kappa": {"name": "kappa", "type": "max"},
@@ -25,30 +39,26 @@
     }
     optimizers = ["adams"]
     useGPU = True
 
     def __init__(self, options=None) -> None:
         options = options or {}
         super().__init__(options)
-        self.logPath = "logs"
-        self.csvLogFile = "log.csv"
+        
         # segmentlength, channelSize
         self.inputShape = None
         self.numClasses = None
         self.classWeights = None
 
         self.batchSize = None
         self.maxEpochs = 100
         self.stopAfterNotImproving = None
-        self.learningRate = 0.001
-        self.learningRateDecay = None
 
         self.classNames = []
         self.monitorMetrics = ["accuracy"]
-        self.optimizer = "adams"
         self.validationMetrics = ["kappa", "accuracy"]
 
         self.model = None
         self.modelEval = None
         self.modelDebug = None
         self.parameter = None
         self.bestMetric = 0
@@ -59,17 +69,18 @@
         self.startFigures = []
         self.showProgress = True
         self.startEpoch = 0
         self.useEventScorer = False
         self.predictionType = "classification"
 
         self.oneHotDecoded = False
+        self.config = ModelConfig()
 
     def getCsvPath(self):
-        return f"{self.logPath}/{self.csvLogFile}"
+        return f"{self.config.logPath}/{self.config.csvLogFile}"
 
     def getMetric(self, name):
         if name not in Model.metrics:
             raise MetricsDoesNotExist(f"The metrics with the name {name} is not defined")
         return Model.metrics[name]
 
     def init(self):
@@ -133,7 +144,8 @@
     @abstractmethod
     def train(self, dataset: DataSet, validationDataset: DataSet = None):
         raise AdapterNotImplemented("required train method is not implemented in the model adapter!")
 
     @abstractmethod
     def predict(self, input, get_likelihood=False, returnNumpy=True):
         raise AdapterNotImplemented("required predict method is not implemented in the model adapter!")
+
```

### Comparing `pyPhasesML-0.6.2/pyPhasesML/ModelManager.py` & `pyPhasesML-0.7.0/pyPhasesML/ModelManager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 
 from pyPhases import ConfigNotFoundException
 from pyPhases.util.EventBusStatic import EventBusStatic
 
-from .Model import Model
+from .Model import Model, ModelConfig
 
 
 class ModelManager(EventBusStatic):
     model: Model = None
     modelOptions = None
     beforeBuild = None
     modelPath = None
@@ -22,20 +22,25 @@
         return ModelManager.model
 
     def loadModelFromOptions() -> None:
         options = ModelManager.modelOptions
         modelClass = ModelManager.loadModelByModule(options["modelName"])
         model = modelClass(options["modelConfig"])
 
-        for field in options["general"]:
-            setattr(model, field, options["general"][field])
+        for field, value in options["general"].items():
+            setattr(model, field, value)
+            
+        model.config = ModelConfig()
+        for field, value in options["config"].items():
+            setattr(model.config, field, value)
 
         if ModelManager.beforeBuild is not None:
             ModelManager.beforeBuild(model)
-
+    
+        model.initAdapter()
         model.init()
         model.define()
         model.build()
         ModelManager.model = model
         ModelManager.trigger("modelLoaded", model)
 
     def validate(config):
@@ -71,25 +76,30 @@
             "general": {
                 "inputShape": project.config["inputShape"],
                 "numClasses": classCount,
                 "maxEpochs": project.getConfig("trainingParameter.maxEpochs", None, False),
                 "batchSize": trainingParameter["batchSize"],
                 "classWeights": project.getConfig("trainingParameter.classWeights", None, False),
                 "classNames": classNames,
-                "learningRate": project.getConfig("trainingParameter.learningRate", 0.001),
-                "learningRateDecay": project.getConfig("trainingParameter.learningRateDecay", None, False),
-                "stopAfterNotImproving": project.getConfig("trainingParameter.stopAfterNotImproving", 10),
                 "validationEvery": project.getConfig("trainingParameter.validationEvery", None, False),
-                "optimizer": project.getConfig("trainingParameter.optimizer", "Adams"),
                 "ignoreClassIndex": project.getConfig("ignoreClassIndex", None, False),
                 "validationMetrics": project.getConfig("trainingParameter.validationMetrics", ["loss"]),
                 "useEventScorer": project.getConfig("trainingParameter.useEventScorer", False),
                 "predictionType": project.getConfig("classification.type", "classification"),
                 "oneHotDecoded": project.getConfig("oneHotDecoded", False),
+                "cycleLR": project.getConfig("trainingParameter.cyclicLearningRate", False),
             },
+            "config": {
+                # training
+                "optimizerId": project.getConfig("trainingParameter.optimizer", "Adams"),
+                "learningRate": project.getConfig("trainingParameter.learningRate", 0.001),
+                "learningRateDecay": project.getConfig("trainingParameter.learningRateDecay", None, False),
+                "stopAfterNotImproving": project.getConfig("trainingParameter.stopAfterNotImproving", 10),
+                "cycleLRDivisor": project.getConfig("trainingParameter.cycleLRDivisor", 4),                
+            }
         }
 
     @staticmethod
     def loadModelByModule(name):
         path = ModelManager.modelPath.replace("/", ".")
         packageSplit = path.split(".")
         package = packageSplit[0]
```

### Comparing `pyPhasesML-0.6.2/pyPhasesML/Plugin.py` & `pyPhasesML-0.7.0/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.7.0/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.7.0/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pyPhasesML import ModelAdapter
 from ..scorer.ScorerTF import ScorerTF
 
 import shutil
 import tensorflow as tf
 import tensorflow.keras as K
 import matplotlib.pyplot as plt
 import numpy as np
@@ -24,15 +25,15 @@
     # Convert PNG buffer to TF image
     image = tf.image.decode_png(buf.getvalue(), channels=4)
     # Add the batch dimension
     image = tf.expand_dims(image, 0)
     return image
 
 
-class ModelKerasAdapter(Model):
+class ModelKerasAdapter(ModelAdapter):
     model: K.Model = None
 
     def _metrics(self, metric, validation=False):
         prepend = "val_" if validation else ""
         return prepend + metric["name"]
 
     def getMetrics(self):
```

### Comparing `pyPhasesML-0.6.2/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.7.0/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from numpy.core.records import record
+from pyPhasesML import ModelAdapter
 import tensorflow as tf
 import keras as K
 import numpy as np
 
 from ..DataSet import TrainingSet
 from ..Model import Model
 
 
 # K.set_image_data_format("channels_last")
 
 
-class ModelTf1Adapter(Model):
+class ModelTf1Adapter(ModelAdapter):
     model = None
 
     def _metrics(self, metric, validation=False):
         prepend = "val_" if validation else ""
         return prepend + metric["name"]
 
     def beforeTrain(self, dataset):
```

### Comparing `pyPhasesML-0.6.2/pyPhasesML/config.yaml` & `pyPhasesML-0.7.0/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.7.0/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.7.0/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.7.0/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.7.0/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.2/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.7.0/pyPhasesML/scorer/Scorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         self.recordResult = {}
         self.recordIndex = 0
         self.trace = trace
         self.possibleValues = None
         self.addEvents = False
         self.mapping = None
         self.threshold = threshold
+        
+    def reset(self):
+        self.recordResult = {}
+        self.recordIndex = 0
 
     def getMetricDefinition(self, name):
         metricDefinition = {
             # init value, useAsBest, biggerIsBetter
             "AUC": [0.5, False, True],
             "AP": [0.0, True, True],
             "accuracy": [0.0, False, True],
@@ -239,14 +243,17 @@
         max = np.max(prediction, axis=1, keepdims=True)
         if self.isHotEncoded(prediction):
             e_x = np.exp(prediction - max)
             sum = np.sum(e_x, axis=1, keepdims=True)  # returns sum of each row and keeps same dims
             predictionSoftMax = e_x / sum
             classLikelyhood = predictionSoftMax[:, 1]
         else:
+            if any(max > 1) or any(max < 0):
+                # transform to probability
+                max = 1 / (1 + np.exp(-max))
             classLikelyhood = max.reshape(-1)
         return classLikelyhood
 
     def getClassPrediction(self, prediction):
         likelyhood = self.getClassLikelyhood(prediction)
         binPrediction = np.full(prediction.shape[0], 0)
         binPrediction[likelyhood > self.threshold] = 1
@@ -270,16 +277,18 @@
                 binPrediction[binPrediction == self.numClasses] = self.numClasses - 1
                 return np.floor(binPrediction)
             else:
                 binPrediction[binPrediction >= threshhold] = 1
                 binPrediction[binPrediction < threshhold] = 0
         return binPrediction
 
-    def getMetricScorer(self, metricName):
+    def getMetricScorer(self, metricName, predictionFirst=False):
         def score(truth, prediction):
+            if predictionFirst:
+                truth, prediction = prediction, truth
             prediction = self.prepareInput(prediction)
             truth = self.prepareInput(truth)
             prediction = self.preparePrediction(prediction)
             truth = self.prepareTruth(truth)
             self.results = {}
             return self.scoreMetric(metricName, truth, prediction)
```

### Comparing `pyPhasesML-0.6.2/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.7.0/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 This Extension adds:
 - an Exporter for `PyTorch` and `TensorFlow` Models.
 - an Modelmanager that can handle `PyTorch` and `TensorFlow` Models
 
 
 ## Setup
 
-- add pyPhasesML to your dependencies or run `pipp install -U pyPhasesML`
+- add pyPhasesML to your dependencies or run `pip install -U pyPhasesML`
 - add `pyPhasesML` to your plugins in the main project config f.e: in your `project.yaml`
 ```yaml
 name: bumpDetector
 namespace: ibmt.tud
 
 # load machine learning plugin
 plugins:
```

### Comparing `pyPhasesML-0.6.2/setup.py` & `pyPhasesML-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.6.2"[1:],
+    version="v0.7.0"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

