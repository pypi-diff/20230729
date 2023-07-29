# Comparing `tmp/Bokit-0.2.2.tar.gz` & `tmp/Bokit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bokit-0.2.2.tar", last modified: Sat Jul 29 11:25:42 2023, max compression
+gzip compressed data, was "Bokit-0.2.3.tar", last modified: Sat Jul 29 11:43:20 2023, max compression
```

## Comparing `Bokit-0.2.2.tar` & `Bokit-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:25:42.715031 Bokit-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:25:42.711031 Bokit-0.2.2/Bokit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 11:25:42.000000 Bokit-0.2.2/Bokit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-29 11:25:42.000000 Bokit-0.2.2/Bokit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 11:25:42.000000 Bokit-0.2.2/Bokit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 11:25:42.000000 Bokit-0.2.2/Bokit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 11:25:42.715031 Bokit-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-29 11:25:34.000000 Bokit-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:25:42.715031 Bokit-0.2.2/bokit/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:25:42.715031 Bokit-0.2.2/bokit/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/ChatGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/CreateFlashcards.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/DictionaryLookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/OCR.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/Phonetize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/TokenStatistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/Tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/Transifex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/Translate.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:25:42.715031 Bokit-0.2.2/bokit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/clean_tibetan_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/create_particles_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/create_punctuation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/create_special_char_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/create_stopword_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/is_all_latin.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/is_all_tibetan.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/is_partly_tibetan.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/pdf_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/read_text_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/remove_non_tibetan.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/tibetan_to_wylie.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/utils/wylie_to_tibetan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:25:42.715031 Bokit-0.2.2/bokit/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/workflows/build_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/workflows/image_to_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 11:25:34.000000 Bokit-0.2.2/bokit/workflows/pdf_to_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 11:25:42.715031 Bokit-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-29 11:25:34.000000 Bokit-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:43:20.480368 Bokit-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:43:20.480368 Bokit-0.2.3/Bokit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 11:43:20.000000 Bokit-0.2.3/Bokit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-29 11:43:20.000000 Bokit-0.2.3/Bokit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 11:43:20.000000 Bokit-0.2.3/Bokit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 11:43:20.000000 Bokit-0.2.3/Bokit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 11:43:20.480368 Bokit-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-29 11:43:12.000000 Bokit-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:43:20.480368 Bokit-0.2.3/bokit/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:43:20.480368 Bokit-0.2.3/bokit/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/ChatGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/CreateFlashcards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/DictionaryLookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/OCR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/Phonetize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/TokenStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/Tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/Transifex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:43:20.480368 Bokit-0.2.3/bokit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/clean_tibetan_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/create_particles_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/create_punctuation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/create_special_char_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/create_stopword_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/is_all_latin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/is_all_tibetan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/is_partly_tibetan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/pdf_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/read_text_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/remove_non_tibetan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/tibetan_to_wylie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/utils/wylie_to_tibetan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:43:20.480368 Bokit-0.2.3/bokit/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/workflows/build_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/workflows/image_to_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 11:43:12.000000 Bokit-0.2.3/bokit/workflows/pdf_to_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 11:43:20.480368 Bokit-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-29 11:43:12.000000 Bokit-0.2.3/setup.py
```

### Comparing `Bokit-0.2.2/Bokit.egg-info/PKG-INFO` & `Bokit-0.2.3/Bokit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bokit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bokit is a Python API that exposes commonly used tools for various Tibetan language workflows.
 Home-page: https://github.com/lopenling/bokit
 Author: Mikko Kotila
 Author-email: mailme@mikkokotila.com
 License: MIT
 Keywords: tibetan etl tools
 Classifier: Intended Audience :: Developers
```

### Comparing `Bokit-0.2.2/Bokit.egg-info/SOURCES.txt` & `Bokit-0.2.3/Bokit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/PKG-INFO` & `Bokit-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bokit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bokit is a Python API that exposes commonly used tools for various Tibetan language workflows.
 Home-page: https://github.com/lopenling/bokit
 Author: Mikko Kotila
 Author-email: mailme@mikkokotila.com
 License: MIT
 Keywords: tibetan etl tools
 Classifier: Intended Audience :: Developers
```

### Comparing `Bokit-0.2.2/README.md` & `Bokit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/__init__.py` & `Bokit-0.2.3/bokit/__init__.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/ChatGPT.py` & `Bokit-0.2.3/bokit/commands/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/CreateFlashcards.py` & `Bokit-0.2.3/bokit/commands/CreateFlashcards.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/DictionaryLookup.py` & `Bokit-0.2.3/bokit/commands/DictionaryLookup.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/OCR.py` & `Bokit-0.2.3/bokit/commands/OCR.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/Phonetize.py` & `Bokit-0.2.3/bokit/commands/Phonetize.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/TokenStatistics.py` & `Bokit-0.2.3/bokit/commands/TokenStatistics.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/Tokenize.py` & `Bokit-0.2.3/bokit/commands/Tokenize.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,33 @@
         from botok.config import Config
         from pathlib import Path
         
         # initialize the tokenizer
         config = Config(dialect_name="general", base_path=Path.home())
         self._wt = WordTokenizer(config=config)
 
-    def query(self, text):
+    def query(self, text, split_affixes=False, tokenizer_object=False):
 
         '''Takes in Tibetan string and returns list of tokens.
         
-        text | str | Tibetan string
-        
+        text | str | Tibetan string to tokenize
+        split_affixes | bool | if True, returns list of tokens with affixes
+        tokenizer_object | bool | if True, returns tokenizer object with more data
         '''
 
         # initialize the list of tokens to be returned
         tokens = []
 
         # tokenize the input text
-        tokenizer_output = self._wt.tokenize(text, split_affixes=False)
+        tokenizer_output = self._wt.tokenize(text, split_affixes=split_affixes)
+        
+        if tokenizer_object is True:
+            return tokenizer_output
         
-        # iterate through the tokens and add them to the list
         for token in tokenizer_output:
-            tokens.append(token['text_unaffixed'])
+            
+            if split_affixes is True:
+                tokens.append(token['text'])
+            elif split_affixes is False:
+                tokens.append(token['text_unaffixed'])
 
-        return tokens
-   
+        return tokens
```

### Comparing `Bokit-0.2.2/bokit/commands/Transifex.py` & `Bokit-0.2.3/bokit/commands/Transifex.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/commands/Translate.py` & `Bokit-0.2.3/bokit/commands/Translate.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/utils/clean_tibetan_string.py` & `Bokit-0.2.3/bokit/utils/clean_tibetan_string.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/utils/create_particles_list.py` & `Bokit-0.2.3/bokit/utils/create_particles_list.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/utils/create_punctuation_list.py` & `Bokit-0.2.3/bokit/utils/create_punctuation_list.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/utils/create_special_char_list.py` & `Bokit-0.2.3/bokit/utils/create_special_char_list.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/workflows/build_text.py` & `Bokit-0.2.3/bokit/workflows/build_text.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/bokit/workflows/image_to_translation.py` & `Bokit-0.2.3/bokit/workflows/image_to_translation.py`

 * *Files identical despite different names*

### Comparing `Bokit-0.2.2/setup.py` & `Bokit-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 setup(
     name='Bokit',
-    version='v0.2.2',
+    version='v0.2.3',
     description='Bokit is a Python API that exposes commonly used tools for various Tibetan language workflows.',
     long_description='Bokit is a Python API that exposes commonly used tools for various Tibetan language workflows.',
     url='https://github.com/lopenling/bokit',
     author='Mikko Kotila',
     author_email='mailme@mikkokotila.com',
     license='MIT',
     classifiers=[
```

