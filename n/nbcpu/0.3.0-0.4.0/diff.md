# Comparing `tmp/nbcpu-0.3.0.tar.gz` & `tmp/nbcpu-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbcpu-0.3.0.tar", max compression
+gzip compressed data, was "nbcpu-0.4.0.tar", max compression
```

## Comparing `nbcpu-0.3.0.tar` & `nbcpu-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1071 2023-07-28 23:48:55.082976 nbcpu-0.3.0/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-28 23:48:55.082976 nbcpu-0.3.0/README.md
--rw-r--r--   0        0        0     2985 2023-07-28 23:49:21.783127 nbcpu-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      180 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/__init__.py
--rw-r--r--   0        0        0       22 2023-07-28 23:49:21.743127 nbcpu-0.3.0/src/nbcpu/_version.py
--rw-r--r--   0        0        0        0 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/conf/__init__.py
--rw-r--r--   0        0        0      275 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/conf/about/nbcpu.yaml
--rw-r--r--   0        0        0      609 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/conf/fetcher/khmer.yaml
--rw-r--r--   0        0        0        0 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/fetcher/__init__.py
--rw-r--r--   0        0        0    14530 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/fetcher/khmer.py
--rw-r--r--   0        0        0        0 2023-07-28 23:48:55.086976 nbcpu-0.3.0/src/nbcpu/py.typed
--rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 nbcpu-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-29 05:29:34.130010 nbcpu-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-29 05:29:34.130010 nbcpu-0.4.0/README.md
+-rw-r--r--   0        0        0     2985 2023-07-29 05:29:58.798376 nbcpu-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-07-29 05:29:34.130010 nbcpu-0.4.0/src/nbcpu/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-29 05:29:58.754375 nbcpu-0.4.0/src/nbcpu/_version.py
+-rw-r--r--   0        0        0        0 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/conf/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/conf/about/nbcpu.yaml
+-rw-r--r--   0        0        0      609 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/conf/fetcher/khmer.yaml
+-rw-r--r--   0        0        0        0 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/fetcher/__init__.py
+-rw-r--r--   0        0        0    13499 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/fetcher/khmer.py
+-rw-r--r--   0        0        0        0 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/py.typed
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 nbcpu-0.4.0/PKG-INFO
```

### Comparing `nbcpu-0.3.0/LICENSE` & `nbcpu-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbcpu-0.3.0/README.md` & `nbcpu-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nbcpu-0.3.0/pyproject.toml` & `nbcpu-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nbcpu"
-version = "0.3.0"
+version = "0.4.0"
 description = "Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/nbcpu"
 repository = "https://github.com/entelecheia/nbcpu"
 readme = "README.md"
 packages = [{ include = "nbcpu", from = "src" }]
 
 [tool.poetry.scripts]
 nbcpu = 'nbcpu.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.12.2"
+hyfi = "^1.12.5"
 # hyfi = { path = "../hyfi", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
```

### Comparing `nbcpu-0.3.0/src/nbcpu/conf/fetcher/khmer.yaml` & `nbcpu-0.4.0/src/nbcpu/conf/fetcher/khmer.yaml`

 * *Files identical despite different names*

### Comparing `nbcpu-0.3.0/src/nbcpu/fetcher/khmer.py` & `nbcpu-0.4.0/src/nbcpu/fetcher/khmer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import multiprocessing as mp
 from datetime import datetime
 from functools import partial
 from pathlib import Path
 from typing import List, Optional
 
 import requests
@@ -92,20 +91,20 @@
     def article_filepath_tmp(self) -> str:
         _path = Path(self.output_dir) / f"{self.article_filename}.tmp"
         _path.parent.mkdir(parents=True, exist_ok=True)
         return str(_path)
 
     def _load_links(self):
         if Path(self.link_filepath).exists():
-            self._links = load_jsonl(self.link_filepath)
+            self._links = HyFI.load_jsonl(self.link_filepath)
         return self._links
 
     def _load_articles(self):
         if Path(self.article_filepath).exists():
-            self._articles = load_jsonl(self.article_filepath)
+            self._articles = HyFI.load_jsonl(self.article_filepath)
         return self._articles
 
     def fetch_links(self):
         num_workers = min(self.num_workers, len(self.search_keywords))
         self._load_links()
         links = self._links
         if num_workers > 1:
@@ -118,21 +117,21 @@
                     links=links,
                     max_num_pages=self.max_num_pages,
                     link_filepath=self.link_filepath_tmp,
                     print_every=self.print_every,
                     verbose=self.verbose,
                 )
         original_len = len(self._links)
-        self._links = remove_duplicates(self._links, key="url")
+        self._links = HyFI.remove_duplicates_from_list_of_dicts(self._links, key="url")
         logger.info(
             "Removed %s duplicate links from %s links",
             original_len - len(self._links),
             original_len,
         )
-        save_jsonl(self._links, self.link_filepath)
+        HyFI.save_jsonl(self._links, self.link_filepath)
         logger.info("Saved %s links to %s", len(self._links), self.link_filepath)
 
     def _fetch_links_mp(self, num_workers, links):
         process_batch_partial = partial(
             crawl_khmer_times,
             search_url=self.search_url,
             links=links,
@@ -161,21 +160,23 @@
                 overwrite_existing=self.overwrite_existing,
                 max_num_articles=self.max_num_articles,
                 article_filepath=self.article_filepath_tmp,
                 print_every=self.print_every,
                 verbose=self.verbose,
             )
         original_len = len(self._articles)
-        self._articles = remove_duplicates(self._articles, key="url")
+        self._articles = HyFI.remove_duplicates_from_list_of_dicts(
+            self._articles, key="url"
+        )
         logger.info(
             "Removed %s duplicate articles from %s articles",
             original_len - len(self._articles),
             original_len,
         )
-        save_jsonl(self._articles, self.article_filepath)
+        HyFI.save_jsonl(self._articles, self.article_filepath)
         logger.info(
             "Saved %s articles to %s", len(self._articles), self.article_filepath
         )
 
     def _fetch_articles_mp(self, num_workers, articles):
         batch_size = len(self.links) // num_workers
         batches = [
@@ -261,15 +262,15 @@
                         "title": title,
                         "url": url,
                         "keyword": keyword,
                     }
                     links.append(link)
                     link_urls.append(url)
                     if link_filepath:
-                        append_to_jsonl(link, link_filepath)
+                        HyFI.append_to_jsonl(link, link_filepath)
                 else:
                     logger.info("Link %s already exists, skipping...", url)
         except Exception as e:
             logger.error("Error while fetching the page url: %s", page_url)
             logger.error(e)
 
         page += 1
@@ -333,15 +334,15 @@
                     url=url,
                     keyword=keyword,
                     title=title,
                 )
                 articles.append(article)
                 article_urls.append(url)
                 if article_filepath:
-                    append_to_jsonl(article, article_filepath)
+                    HyFI.append_to_jsonl(article, article_filepath)
                 if verbose and (i + 1) % print_every == 0:
                     logger.info("Article [%s](%s) scraped", title, url)
             else:
                 logger.info("Article [%s](%s) does not exist, skipping...", title, url)
         except Exception as e:
             logger.error("Error while scraping the article url: %s", url)
             logger.error(e)
@@ -374,44 +375,7 @@
         "url": url,
         "keyword": keyword,
         "title": title,
         "categories": entry_categories,
         "time": entry_time.isoformat(),  # Convert datetime to string
         "text": article_text,
     }
-
-
-def append_to_jsonl(data, filename: str, encoding: str = "utf-8") -> None:
-    """Append a json payload to the end of a jsonl file."""
-    json_string = json.dumps(data, ensure_ascii=False)
-    with open(filename, "a", encoding=encoding) as f:
-        f.write(json_string + "\n")
-
-
-def load_jsonl(filename: str, encoding: str = "utf-8") -> List[dict]:
-    """Load a jsonl file into a list of json objects."""
-    with open(filename, "r", encoding=encoding) as f:
-        return [json.loads(line) for line in f]
-
-
-def save_jsonl(
-    data: List[dict],
-    filename: str,
-    encoding: str = "utf-8",
-) -> None:
-    """
-    Save a list of json objects to a jsonl file.
-    """
-    with open(filename, "w", encoding=encoding) as f:
-        for line in data:
-            f.write(json.dumps(line, ensure_ascii=False) + "\n")
-
-
-def remove_duplicates(data: List[dict], key: str) -> List[dict]:
-    """Remove duplicates from a list of dicts based on a key."""
-    seen = set()
-    new_data = []
-    for d in data:
-        if d[key] not in seen:
-            new_data.append(d)
-            seen.add(d[key])
-    return new_data
```

### Comparing `nbcpu-0.3.0/PKG-INFO` & `nbcpu-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nbcpu
-Version: 0.3.0
+Version: 0.4.0
 Summary: Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach
 Home-page: https://entelecheia.github.io/nbcpu
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=1.12.2,<2.0.0)
+Requires-Dist: hyfi (>=1.12.5,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/nbcpu
 Description-Content-Type: text/markdown
 
 # Measuring Central Bank Policy Uncertainty
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

