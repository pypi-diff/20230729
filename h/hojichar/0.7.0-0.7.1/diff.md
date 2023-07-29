# Comparing `tmp/hojichar-0.7.0.tar.gz` & `tmp/hojichar-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.7.0.tar", max compression
+gzip compressed data, was "hojichar-0.7.1.tar", max compression
```

## Comparing `hojichar-0.7.0.tar` & `hojichar-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-07-28 04:01:09.966417 hojichar-0.7.0/LICENSE
--rw-r--r--   0        0        0    13612 2023-07-28 04:01:09.966417 hojichar-0.7.0/README.md
--rw-r--r--   0        0        0      547 2023-07-28 04:01:32.878969 hojichar-0.7.0/hojichar/__init__.py
--rw-r--r--   0        0        0     4269 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/cli.py
--rw-r--r--   0        0        0       42 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/__init__.py
--rw-r--r--   0        0        0     4448 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/composition.py
--rw-r--r--   0        0        0     5641 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     6221 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/inspection.py
--rw-r--r--   0        0        0     1087 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    12104 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    23939 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1606 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2530 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0        0 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/py.typed
--rw-r--r--   0        0        0      595 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3380 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1920 2023-07-28 04:01:09.966417 hojichar-0.7.0/hojichar/utils/process.py
--rw-r--r--   0        0        0     1746 2023-07-28 04:01:32.874969 hojichar-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    14345 1970-01-01 00:00:00.000000 hojichar-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-29 05:26:46.953899 hojichar-0.7.1/LICENSE
+-rw-r--r--   0        0        0    14086 2023-07-29 05:26:46.953899 hojichar-0.7.1/README.md
+-rw-r--r--   0        0        0      547 2023-07-29 05:27:06.330181 hojichar-0.7.1/hojichar/__init__.py
+-rw-r--r--   0        0        0     4264 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/cli.py
+-rw-r--r--   0        0        0       42 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     5039 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/composition.py
+-rw-r--r--   0        0        0     5638 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     6221 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/inspection.py
+-rw-r--r--   0        0        0     1087 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    12104 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    23939 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1606 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2530 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0        0 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/py.typed
+-rw-r--r--   0        0        0      595 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3380 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1920 2023-07-29 05:26:46.953899 hojichar-0.7.1/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1746 2023-07-29 05:27:06.330181 hojichar-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    14819 1970-01-01 00:00:00.000000 hojichar-0.7.1/PKG-INFO
```

### Comparing `hojichar-0.7.0/LICENSE` & `hojichar-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/README.md` & `hojichar-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/hojichar.svg)](https://pypi.org/project/hojichar/)
 [![CI wowkflow](https://github.com/HojiChar/HojiChar/actions/workflows/ci.yaml/badge.svg)](https://github.com/HojiChar/HojiChar/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/HojiChar/HojiChar/branch/main/graph/badge.svg?token=16928I9U9Y)](https://codecov.io/gh/HojiChar/HojiChar)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/hojichar)
 
 Official docs: <https://hojichar.github.io/HojiChar/hojichar.html>
 
+## Features
+
+- HojiChar provides a way to combine multiple arbitrary text processing tasks into a streamlined pipeline.
+- The sequence of operations can be described declaratively, ensuring portability.
+- HojiChar allows users to gather detailed statistical information from large amounts of text during processing.
+- It enables management of any Python text processing tasks, providing a Command Line Interface (CLI) capable of parallel processing.
+
 ## Background and what is for HojiChar
 
 Text preprocessing is far from a one-size-fits-all process. Depending on the data source and the specific task at hand, various steps including normalization, noise removal, and filtering may be necessary. Not all texts require the same level of preprocessing. For instance, relatively clean texts may only need minimal filtering, while "dirtier" sources like Common Crawl data often require more thorough processing. As a result, the preprocessing profile has to be tailored to each specific domain.
 
 Many preprocessing operations can be viewed as filters, taking string as input, applying a transformation, and outputting the processed string. Even though these operations might seem straightforward individually, managing them in a multi-layered, efficient manner can be challenging.
 
 Inspired by [`torchvision.transforms`](https://pytorch.org/vision/stable/transforms.html) and [iver56/audiomentations](https://github.com/iver56/audiomentations), HojiChar addresses these challenges. It enables users to define each text processing step as a class inheriting from `hojichar.Filter` and use `hojichar.Compose` to chain them together into a single filter. By writing out the `Compose` recipe as a profile, the preprocessing process for a specific domain's text can be made portable. Moreover, `Compose` automatically logs various metrics for each filter, such as byte changes, processing time, and number of rejected texts. This allows users to assess the validity of each operation and consider trade-offs between computation time and performance.
@@ -331,8 +338,9 @@
 poetry publish
 ```
 
 The actual task for the manager is to apply the appropriate tag to the commit to be released and to create the release from GitHub:
 
 ```
 git tag -a v0.1.2 -m "Version 0.1.2"
+git push origin v0.1.2
 ```
```

### Comparing `hojichar-0.7.0/hojichar/__init__.py` & `hojichar-0.7.1/hojichar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.7.0"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.7.1"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "utils",
     "Compose",
     "Filter",
```

### Comparing `hojichar-0.7.0/hojichar/cli.py` & `hojichar-0.7.1/hojichar/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from hojichar.core.inspection import StatsContainer
 from hojichar.utils.io_iter import fileout_from_iter, stdin_iter, stdout_from_iter
 from hojichar.utils.load_compose import load_compose
 
 MAIN_FILTER: hojichar.Compose
 CLI_ARGS: argparse.Namespace
 
-logger = logging.getLogger("hojichar.__main__")
+logger = logging.getLogger("hojichar.cli")
 
 
 def argparser() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--profile",
         "-p",
```

### Comparing `hojichar-0.7.0/hojichar/core/composition.py` & `hojichar-0.7.1/hojichar/core/composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         random_state : Union[None, int, np.random.Generator], optional
             Default = None
             Seed for applying filters randomly.
             `random_state` must be int or np.random.Generator instance.
         """
         super().__init__(*args, **kwargs)
-        self.filters = filters
+        self.set_filters(filters)
         self.logger = logging.getLogger("hojichar.Compose")
         self.before_process_inspector = Inspector(
             target_filter=BeforeProcessFilter(), filter_idx=-1
         )
         self.inspectors = [
             Inspector(target_filter=filter, filter_idx=idx)
             for idx, filter in enumerate(self.filters)
@@ -56,14 +56,29 @@
         elif isinstance(random_state, int):
             self.rng = np.random.default_rng(random_state)
         elif isinstance(random_state, np.random.Generator):
             self.rng = random_state
         else:
             raise ValueError(f"{random_state} cannot be used to seed.")
 
+    def set_filters(self, filters: List[Union[Filter, TokenFilter]]) -> None:
+        """
+        Set the filter to a Compose object. The filter is expanded if the
+        list of filters in the argument contains a filter bound by Compose.
+
+        Args:
+            filters (List[Union[Filter, TokenFilter]]): Target filters
+        """
+        self.filters: List[Union[Filter, TokenFilter]] = []
+        for filter in filters:
+            if isinstance(filter, Compose):
+                self.filters.extend(filter.filters)
+            else:
+                self.filters.append(filter)
+
     def __call__(self, text: str) -> str:
         document = Document(text)
         document = self.apply(document)
         if document.is_rejected:
             return ""
         else:
             return document.text
```

### Comparing `hojichar-0.7.0/hojichar/core/filter_interface.py` & `hojichar-0.7.1/hojichar/core/filter_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def __init__(
         self, p: float = 1, skip_rejected: bool = True, *args: Any, **kwargs: Any
     ) -> None:
         """
         Parameters
         ----------
-        p : float, opt∏ional
+        p : float, optional
             Probability that this filter will be applied. Default=1
         """
         self.name = self.__class__.__name__
         self.logger = logging.getLogger("hojichar.document_filters." + self.name)
         assert 0 <= p <= 1
         self.p = p
         self.skip_rejected = skip_rejected
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hojichar-0.7.0/hojichar/core/inspection.py` & `hojichar-0.7.1/hojichar/core/inspection.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/core/models.py` & `hojichar-0.7.1/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.7.1/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.7.1/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.7.1/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.7.1/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.7.1/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/filters/__init__.py` & `hojichar-0.7.1/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/filters/deduplication.py` & `hojichar-0.7.1/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/filters/document_filters.py` & `hojichar-0.7.1/hojichar/filters/document_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/filters/token_filters.py` & `hojichar-0.7.1/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/filters/tokenization.py` & `hojichar-0.7.1/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/utils/__init__.py` & `hojichar-0.7.1/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/utils/io_iter.py` & `hojichar-0.7.1/hojichar/utils/io_iter.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/utils/load_compose.py` & `hojichar-0.7.1/hojichar/utils/load_compose.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/hojichar/utils/process.py` & `hojichar-0.7.1/hojichar/utils/process.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.7.0/pyproject.toml` & `hojichar-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.7.0"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.7.1"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
```

### Comparing `hojichar-0.7.0/PKG-INFO` & `hojichar-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.7.0
+Version: 0.7.1
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,14 +24,21 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/hojichar.svg)](https://pypi.org/project/hojichar/)
 [![CI wowkflow](https://github.com/HojiChar/HojiChar/actions/workflows/ci.yaml/badge.svg)](https://github.com/HojiChar/HojiChar/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/gh/HojiChar/HojiChar/branch/main/graph/badge.svg?token=16928I9U9Y)](https://codecov.io/gh/HojiChar/HojiChar)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/hojichar)
 
 Official docs: <https://hojichar.github.io/HojiChar/hojichar.html>
 
+## Features
+
+- HojiChar provides a way to combine multiple arbitrary text processing tasks into a streamlined pipeline.
+- The sequence of operations can be described declaratively, ensuring portability.
+- HojiChar allows users to gather detailed statistical information from large amounts of text during processing.
+- It enables management of any Python text processing tasks, providing a Command Line Interface (CLI) capable of parallel processing.
+
 ## Background and what is for HojiChar
 
 Text preprocessing is far from a one-size-fits-all process. Depending on the data source and the specific task at hand, various steps including normalization, noise removal, and filtering may be necessary. Not all texts require the same level of preprocessing. For instance, relatively clean texts may only need minimal filtering, while "dirtier" sources like Common Crawl data often require more thorough processing. As a result, the preprocessing profile has to be tailored to each specific domain.
 
 Many preprocessing operations can be viewed as filters, taking string as input, applying a transformation, and outputting the processed string. Even though these operations might seem straightforward individually, managing them in a multi-layered, efficient manner can be challenging.
 
 Inspired by [`torchvision.transforms`](https://pytorch.org/vision/stable/transforms.html) and [iver56/audiomentations](https://github.com/iver56/audiomentations), HojiChar addresses these challenges. It enables users to define each text processing step as a class inheriting from `hojichar.Filter` and use `hojichar.Compose` to chain them together into a single filter. By writing out the `Compose` recipe as a profile, the preprocessing process for a specific domain's text can be made portable. Moreover, `Compose` automatically logs various metrics for each filter, such as byte changes, processing time, and number of rejected texts. This allows users to assess the validity of each operation and consider trade-offs between computation time and performance.
@@ -351,9 +358,10 @@
 poetry publish
 ```
 
 The actual task for the manager is to apply the appropriate tag to the commit to be released and to create the release from GitHub:
 
 ```
 git tag -a v0.1.2 -m "Version 0.1.2"
+git push origin v0.1.2
 ```
```

