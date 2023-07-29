# Comparing `tmp/textarium-0.1.3.tar.gz` & `tmp/textarium-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textarium-0.1.3.tar", max compression
+gzip compressed data, was "textarium-0.1.5.tar", max compression
```

## Comparing `textarium-0.1.3.tar` & `textarium-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1063 2023-06-06 20:22:21.061879 textarium-0.1.3/LICENSE
--rw-r--r--   0        0        0     1486 2023-06-06 20:22:21.065879 textarium-0.1.3/README.md
--rw-r--r--   0        0        0      602 2023-06-06 20:22:21.065879 textarium-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/.DS_Store
--rw-r--r--   0        0        0     1870 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/__init__.py
--rw-r--r--   0        0        0       65 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/__init__.py
--rw-r--r--   0        0        0     5229 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/en_stopwords.txt
--rw-r--r--   0        0        0     4536 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/ru_stopwords.txt
--rw-r--r--   0        0        0      305 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/collections/stopwords.py
--rw-r--r--   0        0        0      786 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/corpus.py
--rw-r--r--   0        0        0     1509 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/extraction.py
--rw-r--r--   0        0        0      216 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/models.py
--rw-r--r--   0        0        0     4655 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/preprocessing.py
--rw-r--r--   0        0        0        0 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/__init__.py
--rw-r--r--   0        0        0      283 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test__all__.py
--rw-r--r--   0        0        0      415 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_collections.py
--rw-r--r--   0        0        0      809 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_corpus.py
--rw-r--r--   0        0        0     2243 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_extraction.py
--rw-r--r--   0        0        0     2935 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_preprocessing.py
--rw-r--r--   0        0        0     1638 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/tests/test_text.py
--rw-r--r--   0        0        0     1092 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/text.py
--rw-r--r--   0        0        0      567 2023-06-06 20:22:21.065879 textarium-0.1.3/textarium/utils.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 textarium-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-29 07:48:01.890529 textarium-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1484 2023-07-29 07:48:01.890529 textarium-0.1.5/README.md
+-rw-r--r--   0        0        0      602 2023-07-29 07:48:01.890529 textarium-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/.DS_Store
+-rw-r--r--   0        0        0     1870 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/collections/__init__.py
+-rw-r--r--   0        0        0     5229 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/collections/en_stopwords.txt
+-rw-r--r--   0        0        0     4536 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/collections/ru_stopwords.txt
+-rw-r--r--   0        0        0      305 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/collections/stopwords.py
+-rw-r--r--   0        0        0      800 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/corpus.py
+-rw-r--r--   0        0        0     1509 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/extraction.py
+-rw-r--r--   0        0        0      216 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/models.py
+-rw-r--r--   0        0        0     4655 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/stats/__init__.py
+-rw-r--r--   0        0        0     2316 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/stats/text_stats.py
+-rw-r--r--   0        0        0        0 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/test__all__.py
+-rw-r--r--   0        0        0      415 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/test_collections.py
+-rw-r--r--   0        0        0      809 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/test_corpus.py
+-rw-r--r--   0        0        0     2243 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/test_extraction.py
+-rw-r--r--   0        0        0     2935 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     1638 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/test_text.py
+-rw-r--r--   0        0        0     2272 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/tests/test_text_stats.py
+-rw-r--r--   0        0        0     1093 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/text.py
+-rw-r--r--   0        0        0      567 2023-07-29 07:48:01.890529 textarium-0.1.5/textarium/utils.py
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 textarium-0.1.5/PKG-INFO
```

### Comparing `textarium-0.1.3/LICENSE` & `textarium-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/README.md` & `textarium-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# textarium: easy-to-use Python package for text processing.
+# textarium: easy-to-use Python package for text analysis.
 [![PyPI Latest Release](https://img.shields.io/pypi/v/textarium)](https://pypi.org/project/textarium/)
 [![License](https://img.shields.io/pypi/l/textarium)](https://github.com/6b656b/textarium/blob/main/LICENSE)
 [![Activity](https://img.shields.io/github/commit-activity/m/6b656b/textarium)](https://github.com/6b656b/textarium/pulse)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## What is it?
```

### Comparing `textarium-0.1.3/pyproject.toml` & `textarium-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textarium"
-version = "0.1.3"
+version = "0.1.5"
 description = "Textarium is a Python package for text analysis"
 authors = ["6b656b"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `textarium-0.1.3/textarium/.DS_Store` & `textarium-0.1.5/textarium/.DS_Store`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/__init__.py` & `textarium-0.1.5/textarium/__init__.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/collections/en_stopwords.txt` & `textarium-0.1.5/textarium/collections/en_stopwords.txt`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/collections/ru_stopwords.txt` & `textarium-0.1.5/textarium/collections/ru_stopwords.txt`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/corpus.py` & `textarium-0.1.5/textarium/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from .text import Text
 
 class Corpus:
     def __init__(self, texts: List[str], lang='en'):
         self.lang = lang
         self.corpus = [Text(t, lang=self.lang) for t in texts]
 
-    def __str__(self):
+    def __str__(self) -> str:
         first_five_texts = "\n\n".join([t.raw_text for t in self.corpus[:5]])
         last_five_texts = "\n\n".join([t.raw_text for t in self.corpus[-5:]])
         return first_five_texts + "\n\n...\n\n" + last_five_texts
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"textarium.Corpus object containing {len(self.corpus)} textarium.Text objects"
 
     def prepare(self, lemmatize: bool = True, stopwords: List[str] = None):
         for t in self.corpus:
             t.prepare(lemmatize=lemmatize, stopwords=stopwords)
```

### Comparing `textarium-0.1.3/textarium/extraction.py` & `textarium-0.1.5/textarium/extraction.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/preprocessing.py` & `textarium-0.1.5/textarium/preprocessing.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/tests/test_corpus.py` & `textarium-0.1.5/textarium/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/tests/test_extraction.py` & `textarium-0.1.5/textarium/tests/test_extraction.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/tests/test_preprocessing.py` & `textarium-0.1.5/textarium/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/tests/test_text.py` & `textarium-0.1.5/textarium/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/textarium/text.py` & `textarium-0.1.5/textarium/text.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         text = pipeline(self.raw_text, 
             [
                 tp.remove_html,
                 tp.remove_urls,
                 tp.remove_digits,
                 tp.make_lowercase,
-                tp.remove_punctuation
+                tp.remove_punctuation,
             ]
         )
         if lemmatize:
             text = tp.lemmatize(text, lang=self.lang)
         if stopwords:
             text = tp.remove_words(text, words_to_exclude=stopwords)
         self.prepared_text = text
```

### Comparing `textarium-0.1.3/textarium/utils.py` & `textarium-0.1.5/textarium/utils.py`

 * *Files identical despite different names*

### Comparing `textarium-0.1.3/PKG-INFO` & `textarium-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textarium
-Version: 0.1.3
+Version: 0.1.5
 Summary: Textarium is a Python package for text analysis
 License: MIT
 Author: 6b656b
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,15 @@
 Requires-Dist: pymorphy2-dicts (>=2.4.393442.3710985,<3.0.0.0)
 Requires-Dist: pytest (>=7.1.3,<8.0.0)
 Requires-Dist: razdel (>=0.5.0,<0.6.0)
 Requires-Dist: setuptools (>=65.6.3,<66.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
-# textarium: easy-to-use Python package for text processing.
+# textarium: easy-to-use Python package for text analysis.
 [![PyPI Latest Release](https://img.shields.io/pypi/v/textarium)](https://pypi.org/project/textarium/)
 [![License](https://img.shields.io/pypi/l/textarium)](https://github.com/6b656b/textarium/blob/main/LICENSE)
 [![Activity](https://img.shields.io/github/commit-activity/m/6b656b/textarium)](https://github.com/6b656b/textarium/pulse)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## What is it?
```

