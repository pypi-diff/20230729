# Comparing `tmp/smartloop-1.0.2.tar.gz` & `tmp/smartloop-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartloop-1.0.2.tar", last modified: Fri Jul 28 23:35:03 2023, max compression
+gzip compressed data, was "smartloop-1.0.3.tar", last modified: Fri Jul 28 23:43:37 2023, max compression
```

## Comparing `smartloop-1.0.2.tar` & `smartloop-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.890018 smartloop-1.0.2/
--rw-r--r--   0 mehfuz     (501) staff       (20)     1065 2023-06-20 05:48:15.000000 smartloop-1.0.2/LICENSE.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)       24 2022-06-27 05:07:42.000000 smartloop-1.0.2/MANIFEST.in
--rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-28 23:35:03.890070 smartloop-1.0.2/PKG-INFO
--rw-r--r--   0 mehfuz     (501) staff       (20)     4704 2023-07-28 18:42:15.000000 smartloop-1.0.2/README.md
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.887288 smartloop-1.0.2/data/
--rw-r--r--   0 mehfuz     (501) staff       (20)    19738 2023-07-20 21:20:54.000000 smartloop-1.0.2/data/sample.json
--rw-r--r--   0 mehfuz     (501) staff       (20)      106 2023-07-28 23:35:03.890257 smartloop-1.0.2/setup.cfg
--rw-r--r--   0 mehfuz     (501) staff       (20)     1437 2023-07-28 23:33:18.000000 smartloop-1.0.2/setup.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.888615 smartloop-1.0.2/sl_core/
--rw-r--r--   0 mehfuz     (501) staff       (20)      344 2023-01-06 20:04:52.000000 smartloop-1.0.2/sl_core/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      171 2022-06-27 05:07:42.000000 smartloop-1.0.2/sl_core/classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      387 2023-01-06 20:04:52.000000 smartloop-1.0.2/sl_core/config.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      109 2022-06-01 06:34:59.000000 smartloop-1.0.2/sl_core/default_config.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.888806 smartloop-1.0.2/sl_core/errors/
--rw-r--r--   0 mehfuz     (501) staff       (20)       41 2022-08-05 16:36:45.000000 smartloop-1.0.2/sl_core/errors/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)       69 2022-08-05 16:36:45.000000 smartloop-1.0.2/sl_core/errors/mode_not_found.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      229 2022-06-01 06:34:59.000000 smartloop-1.0.2/sl_core/file_config.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      904 2022-08-25 21:26:36.000000 smartloop-1.0.2/sl_core/label_parser.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1428 2023-05-03 01:19:44.000000 smartloop-1.0.2/sl_core/model_loader.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.888904 smartloop-1.0.2/sl_core/nlu/
--rw-r--r--   0 mehfuz     (501) staff       (20)       47 2022-06-01 06:34:59.000000 smartloop-1.0.2/sl_core/nlu/__init__.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.889110 smartloop-1.0.2/sl_core/nlu/callbacks/
--rw-r--r--   0 mehfuz     (501) staff       (20)       51 2022-06-27 05:07:42.000000 smartloop-1.0.2/sl_core/nlu/callbacks/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1217 2022-06-27 05:07:42.000000 smartloop-1.0.2/sl_core/nlu/callbacks/train_status_report.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.889316 smartloop-1.0.2/sl_core/nlu/classifiers/
--rw-r--r--   0 mehfuz     (501) staff       (20)       67 2022-06-27 05:07:42.000000 smartloop-1.0.2/sl_core/nlu/classifiers/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     6786 2023-07-28 23:34:11.000000 smartloop-1.0.2/sl_core/nlu/classifiers/embedding_intent_classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1819 2023-07-28 23:34:05.000000 smartloop-1.0.2/sl_core/project.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      723 2023-07-28 23:34:11.000000 smartloop-1.0.2/sl_core/sanitizer.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1593 2023-07-28 23:34:05.000000 smartloop-1.0.2/sl_core/text_classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      627 2023-07-28 23:34:05.000000 smartloop-1.0.2/sl_core/tokenizer.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:35:03.889921 smartloop-1.0.2/smartloop.egg-info/
--rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-28 23:35:03.000000 smartloop-1.0.2/smartloop.egg-info/PKG-INFO
--rw-r--r--   0 mehfuz     (501) staff       (20)      732 2023-07-28 23:35:03.000000 smartloop-1.0.2/smartloop.egg-info/SOURCES.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)        1 2023-07-28 23:35:03.000000 smartloop-1.0.2/smartloop.egg-info/dependency_links.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)       56 2023-07-28 23:35:03.000000 smartloop-1.0.2/smartloop.egg-info/requires.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)        8 2023-07-28 23:35:03.000000 smartloop-1.0.2/smartloop.egg-info/top_level.txt
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.023837 smartloop-1.0.3/
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1065 2023-06-20 05:48:15.000000 smartloop-1.0.3/LICENSE.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       24 2022-06-27 05:07:42.000000 smartloop-1.0.3/MANIFEST.in
+-rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-28 23:43:37.023890 smartloop-1.0.3/PKG-INFO
+-rw-r--r--   0 mehfuz     (501) staff       (20)     4704 2023-07-28 18:42:15.000000 smartloop-1.0.3/README.md
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.021162 smartloop-1.0.3/data/
+-rw-r--r--   0 mehfuz     (501) staff       (20)    19738 2023-07-20 21:20:54.000000 smartloop-1.0.3/data/sample.json
+-rw-r--r--   0 mehfuz     (501) staff       (20)      106 2023-07-28 23:43:37.024061 smartloop-1.0.3/setup.cfg
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1437 2023-07-28 23:43:31.000000 smartloop-1.0.3/setup.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.022532 smartloop-1.0.3/smartloop/
+-rw-r--r--   0 mehfuz     (501) staff       (20)      344 2023-01-06 20:04:52.000000 smartloop-1.0.3/smartloop/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      171 2022-06-27 05:07:42.000000 smartloop-1.0.3/smartloop/classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      387 2023-01-06 20:04:52.000000 smartloop-1.0.3/smartloop/config.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      109 2022-06-01 06:34:59.000000 smartloop-1.0.3/smartloop/default_config.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.023279 smartloop-1.0.3/smartloop/errors/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       41 2022-08-05 16:36:45.000000 smartloop-1.0.3/smartloop/errors/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)       69 2022-08-05 16:36:45.000000 smartloop-1.0.3/smartloop/errors/mode_not_found.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      229 2022-06-01 06:34:59.000000 smartloop-1.0.3/smartloop/file_config.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      904 2022-08-25 21:26:36.000000 smartloop-1.0.3/smartloop/label_parser.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1428 2023-05-03 01:19:44.000000 smartloop-1.0.3/smartloop/model_loader.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.023379 smartloop-1.0.3/smartloop/nlu/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       47 2022-06-01 06:34:59.000000 smartloop-1.0.3/smartloop/nlu/__init__.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.023551 smartloop-1.0.3/smartloop/nlu/callbacks/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       51 2022-06-27 05:07:42.000000 smartloop-1.0.3/smartloop/nlu/callbacks/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1217 2022-06-27 05:07:42.000000 smartloop-1.0.3/smartloop/nlu/callbacks/train_status_report.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.023740 smartloop-1.0.3/smartloop/nlu/classifiers/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       67 2022-06-27 05:07:42.000000 smartloop-1.0.3/smartloop/nlu/classifiers/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     6802 2023-07-28 23:43:31.000000 smartloop-1.0.3/smartloop/nlu/classifiers/embedding_intent_classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1821 2023-07-28 23:43:31.000000 smartloop-1.0.3/smartloop/project.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      725 2023-07-28 23:43:31.000000 smartloop-1.0.3/smartloop/sanitizer.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1601 2023-07-28 23:43:31.000000 smartloop-1.0.3/smartloop/text_classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      629 2023-07-28 23:43:31.000000 smartloop-1.0.3/smartloop/tokenizer.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-28 23:43:37.023066 smartloop-1.0.3/smartloop.egg-info/
+-rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-28 23:43:36.000000 smartloop-1.0.3/smartloop.egg-info/PKG-INFO
+-rw-r--r--   0 mehfuz     (501) staff       (20)      768 2023-07-28 23:43:37.000000 smartloop-1.0.3/smartloop.egg-info/SOURCES.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)        1 2023-07-28 23:43:36.000000 smartloop-1.0.3/smartloop.egg-info/dependency_links.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       56 2023-07-28 23:43:36.000000 smartloop-1.0.3/smartloop.egg-info/requires.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       10 2023-07-28 23:43:36.000000 smartloop-1.0.3/smartloop.egg-info/top_level.txt
```

### Comparing `smartloop-1.0.2/LICENSE.txt` & `smartloop-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.2/PKG-INFO` & `smartloop-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartloop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Natural language processing framework for text processing
 Home-page: https://github.com/SmartloopAI/sl-core
 Download-URL: https://github.com/SmartloopAI/sl-core/archive/refs/tags/1.0.1.tar.gz
 Author: Smartloop Inc.
 Author-email: mehfuz@smartloop.ai
 License: LICENSE.txt
 Keywords: NLP,framework,tensorflow,smartloop
```

### Comparing `smartloop-1.0.2/README.md` & `smartloop-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.2/data/sample.json` & `smartloop-1.0.3/data/sample.json`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.2/setup.py` & `smartloop-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'PyYAML==6.0',
     'scikit-learn~=1.2.2',
 ]
 
 setup(
     name='smartloop',
     description='Natural language processing framework for text processing',
-    version='1.0.2',
+    version='1.0.3',
     author_email='mehfuz@smartloop.ai',
     author='Smartloop Inc.',
     url='https://github.com/SmartloopAI/sl-core',
     download_url='https://github.com/SmartloopAI/sl-core/archive/refs/tags/1.0.1.tar.gz',
     keywords=['NLP', 'framework', 'tensorflow', 'smartloop'],
     packages=find_packages(exclude=['tests*']),
     license='LICENSE.txt',
```

### Comparing `smartloop-1.0.2/sl_core/label_parser.py` & `smartloop-1.0.3/smartloop/label_parser.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.2/sl_core/model_loader.py` & `smartloop-1.0.3/smartloop/model_loader.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.2/sl_core/nlu/callbacks/train_status_report.py` & `smartloop-1.0.3/smartloop/nlu/callbacks/train_status_report.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.2/sl_core/nlu/classifiers/embedding_intent_classifier.py` & `smartloop-1.0.3/smartloop/nlu/classifiers/embedding_intent_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from sklearn.preprocessing import LabelEncoder
 
 from keras.preprocessing.text import Tokenizer
 from keras.preprocessing.text import tokenizer_from_json
 from keras.callbacks import TensorBoard
 from keras.callbacks import EarlyStopping
 
-from sl_core import Config, DefaultConfig
+from smartloop import Config, DefaultConfig
 
-from sl_core.classifier import Classifier
-from sl_core.label_parser import LabelParser
-from sl_core.tokenizer import SentenceTokenizer
-from sl_core.nlu import OOV_TOKEN
-from sl_core.nlu.callbacks import TrainStatusReport
-from sl_core.model_loader import ModelLoader
+from smartloop.classifier import Classifier
+from smartloop.label_parser import LabelParser
+from smartloop.tokenizer import SentenceTokenizer
+from smartloop.nlu import OOV_TOKEN
+from smartloop.nlu.callbacks import TrainStatusReport
+from smartloop.model_loader import ModelLoader
 
-from sl_core.sanitizer import Sanitizer
+from smartloop.sanitizer import Sanitizer
 
 logger = logging.getLogger(__name__)
 
 
 class EmbeddingIntentClassifier(Classifier):
     """
         Intent classifier using LSTM model
```

### Comparing `smartloop-1.0.2/sl_core/project.py` & `smartloop-1.0.3/smartloop/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from sl_core.errors import ModelNotFound
+from smartloop.errors import ModelNotFound
 
 
 class Project(object):
     """
        Creates a new project or use an existing one
     """
```

### Comparing `smartloop-1.0.2/sl_core/sanitizer.py` & `smartloop-1.0.3/smartloop/sanitizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nltk.corpus import stopwords
 from nltk.tokenize import RegexpTokenizer
 
 from nltk import PorterStemmer
 
-from sl_core import LANG_MAPS
+from smartloop import LANG_MAPS
 
 
 class Sanitizer:
     """
         Remove punctuations and stop words
     """
```

### Comparing `smartloop-1.0.2/sl_core/text_classifier.py` & `smartloop-1.0.3/smartloop/text_classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
 
 import numpy as np
 
-from sl_core import Config
-from sl_core import Project
+from smartloop import Config
+from smartloop import Project
 
-from sl_core.nlu.classifiers import EmbeddingIntentClassifier
-from sl_core.sanitizer import Sanitizer
+from smartloop.nlu.classifiers import EmbeddingIntentClassifier
+from smartloop.sanitizer import Sanitizer
 
 
 class TextClassifier(object):
     """
         Trains and parses input data to resolve an intent for a given project_id
     """
```

### Comparing `smartloop-1.0.2/sl_core/tokenizer.py` & `smartloop-1.0.3/smartloop/tokenizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from keras.preprocessing.text import Tokenizer
 from keras.utils.data_utils import pad_sequences
-from sl_core import Config, DefaultConfig
+from smartloop import Config, DefaultConfig
 
 
 class SentenceTokenizer:
     """
         Tokenize sentences to sequences
     """
```

### Comparing `smartloop-1.0.2/smartloop.egg-info/PKG-INFO` & `smartloop-1.0.3/smartloop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartloop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Natural language processing framework for text processing
 Home-page: https://github.com/SmartloopAI/sl-core
 Download-URL: https://github.com/SmartloopAI/sl-core/archive/refs/tags/1.0.1.tar.gz
 Author: Smartloop Inc.
 Author-email: mehfuz@smartloop.ai
 License: LICENSE.txt
 Keywords: NLP,framework,tensorflow,smartloop
```

