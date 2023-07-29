# Comparing `tmp/nbcpu-0.4.0.tar.gz` & `tmp/nbcpu-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbcpu-0.4.0.tar", max compression
+gzip compressed data, was "nbcpu-0.5.0.tar", max compression
```

## Comparing `nbcpu-0.4.0.tar` & `nbcpu-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-07-29 05:29:34.130010 nbcpu-0.4.0/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-29 05:29:34.130010 nbcpu-0.4.0/README.md
--rw-r--r--   0        0        0     2985 2023-07-29 05:29:58.798376 nbcpu-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      180 2023-07-29 05:29:34.130010 nbcpu-0.4.0/src/nbcpu/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/__init__.py
--rw-r--r--   0        0        0       22 2023-07-29 05:29:58.754375 nbcpu-0.4.0/src/nbcpu/_version.py
--rw-r--r--   0        0        0        0 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/conf/__init__.py
--rw-r--r--   0        0        0      275 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/conf/about/nbcpu.yaml
--rw-r--r--   0        0        0      609 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/conf/fetcher/khmer.yaml
--rw-r--r--   0        0        0        0 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/fetcher/__init__.py
--rw-r--r--   0        0        0    13499 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/fetcher/khmer.py
--rw-r--r--   0        0        0        0 2023-07-29 05:29:34.134010 nbcpu-0.4.0/src/nbcpu/py.typed
--rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 nbcpu-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-29 20:34:59.258586 nbcpu-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-29 20:34:59.258586 nbcpu-0.5.0/README.md
+-rw-r--r--   0        0        0     2985 2023-07-29 20:35:26.435073 nbcpu-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-29 20:35:26.391072 nbcpu-0.5.0/src/nbcpu/_version.py
+-rw-r--r--   0        0        0        0 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/about/nbcpu.yaml
+-rw-r--r--   0        0        0      674 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/fetcher/khmer.yaml
+-rw-r--r--   0        0        0      697 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/fetcher/phnompenh.yaml
+-rw-r--r--   0        0        0        0 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/__init__.py
+-rw-r--r--   0        0        0    12088 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/base.py
+-rw-r--r--   0        0        0     4049 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/khmer.py
+-rw-r--r--   0        0        0     4704 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/phnompenh.py
+-rw-r--r--   0        0        0        0 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/py.typed
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 nbcpu-0.5.0/PKG-INFO
```

### Comparing `nbcpu-0.4.0/LICENSE` & `nbcpu-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbcpu-0.4.0/README.md` & `nbcpu-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nbcpu-0.4.0/pyproject.toml` & `nbcpu-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nbcpu"
-version = "0.4.0"
+version = "0.5.0"
 description = "Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/nbcpu"
 repository = "https://github.com/entelecheia/nbcpu"
 readme = "README.md"
 packages = [{ include = "nbcpu", from = "src" }]
```

### Comparing `nbcpu-0.4.0/src/nbcpu/fetcher/khmer.py` & `nbcpu-0.5.0/src/nbcpu/fetcher/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,64 @@
+"""Base Fetcher"""
 import multiprocessing as mp
-from datetime import datetime
+import time
 from functools import partial
 from pathlib import Path
-from typing import List, Optional
+from typing import Callable, List, Optional
 
-import requests
-from bs4 import BeautifulSoup
 from hyfi.composer import BaseModel
 from hyfi.main import HyFI
 
 logger = HyFI.getLogger(__name__)
 
 
-class KhmerFetcher(BaseModel):
+class BaseFetcher(BaseModel):
     """
-    Fetcher for Khmer Times.
+    Base Fetcher
     """
 
-    _config_name_: str = "khmer"
+    _config_name_: str = "base"
     _config_group_: str = "fetcher"
 
-    search_url: str = "https://www.khmertimeskh.com/page/{page}/?s={keyword}"
-    search_keywords: List[str] = [
-        "NBC",
-        "Exchange Rate",
-        "De-dollarization",
-        "Inflation",
-        "GDP",
-        "Monetary Policy",
-        "Finance",
-        "Banking",
-        "Stock Exchange",
-        "Uncertain",
-        "Economic",
-        "Policy",
-        "Financial",
-        "Riel",
-        "Bank",
-        "Economy",
-        "Securities Exchange",
-        "National Bank of Cambodia",
-    ]
+    search_url: str = ""
+    search_keywords: List[str] = []
+    start_page: int = 1
     max_num_pages: Optional[int] = 2
     max_num_articles: Optional[int] = 10
-    output_dir: str = "workspace/datasets/khmer"
+    output_dir: str = f"workspace/datasets/{_config_group_}/{_config_name_}"
     link_filename: str = "links.jsonl"
     article_filename: str = "articles.jsonl"
     overwrite_existing: bool = False
+    key_field: str = "url"
+    delay_between_requests: float = 0.0
     num_workers: int = 1
     print_every: int = 10
     verbose: bool = True
 
     _links: List[dict] = []
     _articles: List[dict] = []
+    _headers = {
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3"
+    }
 
     def __call__(self):
         self.fetch()
 
     def fetch(self):
         self.fetch_links()
         self.fetch_articles()
 
     @property
+    def search_keywords_encoded(self):
+        return [self.encode_keyword(keyword) for keyword in self.search_keywords]
+
+    def encode_keyword(self, keyword: str):
+        return keyword.replace(" ", "+")
+
+    @property
     def links(self):
         return self._links or self._load_links()
 
     @property
     def articles(self):
         return self._articles or self._load_articles()
 
@@ -89,207 +82,225 @@
 
     @property
     def article_filepath_tmp(self) -> str:
         _path = Path(self.output_dir) / f"{self.article_filename}.tmp"
         _path.parent.mkdir(parents=True, exist_ok=True)
         return str(_path)
 
-    def _load_links(self):
+    def _load_links(self) -> List[dict]:
         if Path(self.link_filepath).exists():
             self._links = HyFI.load_jsonl(self.link_filepath)
         return self._links
 
-    def _load_articles(self):
+    def _load_articles(self) -> List[dict]:
         if Path(self.article_filepath).exists():
             self._articles = HyFI.load_jsonl(self.article_filepath)
         return self._articles
 
     def fetch_links(self):
+        def parse_page_func(url: str) -> List[dict]:
+            return []
+
+        self._fetch_links(parse_page_func)
+
+    def fetch_articles(self):
+        def _parse_article_text(url: str) -> dict:
+            return {}
+
+        self._fetch_articles(_parse_article_text)
+
+    def _fetch_links(self, parse_page_func: Callable):
         num_workers = min(self.num_workers, len(self.search_keywords))
-        self._load_links()
-        links = self._links
+        link_urls = [link["url"] for link in self.links]
+        fetch_links_func = partial(
+            crawl_links,
+            search_url=self.search_url,
+            parse_page_func=parse_page_func,
+            link_urls=link_urls,
+            start_page=self.start_page,
+            max_num_pages=self.max_num_pages,
+            link_filepath=self.link_filepath_tmp,
+            delay_between_requests=self.delay_between_requests,
+        )
         if num_workers > 1:
-            self._fetch_links_mp(num_workers, links)
+            links = self._fetch_links_mp(
+                num_workers,
+                fetch_links_func,
+            )
         else:
-            for keyword in self.search_keywords:
-                self._links = crawl_khmer_times(
-                    keyword,
-                    search_url=self.search_url,
-                    links=links,
-                    max_num_pages=self.max_num_pages,
-                    link_filepath=self.link_filepath_tmp,
-                    print_every=self.print_every,
-                    verbose=self.verbose,
-                )
+            for keyword in self.search_keywords_encoded:
+                links = fetch_links_func(keyword)
+        if links:
+            self.save_links(links)
+        else:
+            logger.info("No more links found")
+
+    def save_links(self, links: List[dict]):
+        self._links.extend(links)
         original_len = len(self._links)
-        self._links = HyFI.remove_duplicates_from_list_of_dicts(self._links, key="url")
+        self._links = HyFI.remove_duplicates_from_list_of_dicts(
+            self._links, key=self.key_field
+        )
         logger.info(
             "Removed %s duplicate links from %s links",
             original_len - len(self._links),
             original_len,
         )
         HyFI.save_jsonl(self._links, self.link_filepath)
         logger.info("Saved %s links to %s", len(self._links), self.link_filepath)
 
-    def _fetch_links_mp(self, num_workers, links):
-        process_batch_partial = partial(
-            crawl_khmer_times,
-            search_url=self.search_url,
-            links=links,
-            max_num_pages=self.max_num_pages,
-            link_filepath=self.link_filepath_tmp,
-            print_every=self.print_every,
-            verbose=self.verbose,
-        )
+    def _fetch_links_mp(
+        self,
+        num_workers: int,
+        batch_func: Callable,
+    ) -> List[dict]:
         with mp.Pool(num_workers) as pool:
-            results = pool.map(process_batch_partial, self.search_keywords)
+            results = pool.map(batch_func, self.search_keywords_encoded)
         links = []
         for result in results:
             links.extend(result)
-        self._links = links
+        return links
 
-    def fetch_articles(self):
-        num_workers = self.num_workers
-        self._load_articles()
-        articles = self._articles
+    def _fetch_articles(self, parse_article_func: Callable):
+        num_workers = min(self.num_workers, len(self.links))
+        article_urls = [article["url"] for article in self.articles]
+        fetch_articles_func = partial(
+            scrape_article_text,
+            parse_article_func=parse_article_func,
+            article_urls=article_urls,
+            overwrite_existing=self.overwrite_existing,
+            article_filepath=self.article_filepath_tmp,
+            max_num_articles=self.max_num_articles,
+            delay_between_requests=self.delay_between_requests,
+            print_every=self.print_every,
+            verbose=self.verbose,
+        )
         if num_workers > 1:
-            self._fetch_articles_mp(num_workers, articles)
+            articles = self._fetch_articles_mp(num_workers, fetch_articles_func)
         else:
-            self._articles = scrape_article_text(
-                self.links,
-                articles=articles,
-                overwrite_existing=self.overwrite_existing,
-                max_num_articles=self.max_num_articles,
-                article_filepath=self.article_filepath_tmp,
-                print_every=self.print_every,
-                verbose=self.verbose,
-            )
+            articles = fetch_articles_func(self.links)
+        if articles:
+            self.save_articles(articles)
+        else:
+            logger.info("No more articles found")
+
+    def save_articles(self, articles: List[dict]):
+        self._articles.extend(articles)
         original_len = len(self._articles)
         self._articles = HyFI.remove_duplicates_from_list_of_dicts(
-            self._articles, key="url"
+            self._articles, key=self.key_field
         )
         logger.info(
             "Removed %s duplicate articles from %s articles",
             original_len - len(self._articles),
             original_len,
         )
         HyFI.save_jsonl(self._articles, self.article_filepath)
         logger.info(
-            "Saved %s articles to %s", len(self._articles), self.article_filepath
+            "Saved %s articles to %s",
+            len(self._articles),
+            self.article_filepath,
         )
 
-    def _fetch_articles_mp(self, num_workers, articles):
+    def _fetch_articles_mp(
+        self,
+        num_workers: int,
+        batch_func: Callable,
+    ) -> List[dict]:
         batch_size = len(self.links) // num_workers
         batches = [
             self.links[i : i + batch_size]
             for i in range(0, len(self.links), batch_size)
         ]
-        process_batch_partial = partial(
-            scrape_article_text,
-            articles=articles,
-            overwrite_existing=self.overwrite_existing,
-            article_filepath=self.article_filepath_tmp,
-            max_num_articles=self.max_num_articles,
-            print_every=self.print_every,
-            verbose=self.verbose,
-        )
         with mp.Pool(num_workers) as pool:
-            results = pool.map(process_batch_partial, batches)
+            results = pool.map(batch_func, batches)
         articles = []
         for result in results:
             articles.extend(result)
-        self._articles = articles
+        return articles
 
 
-def crawl_khmer_times(
+def crawl_links(
     keyword: str,
-    search_url: str = "https://www.khmertimeskh.com/page/{page}/?s={keyword}",
-    links: Optional[List[dict]] = None,
+    search_url: str,
+    parse_page_func: Callable,
+    link_urls: Optional[List[str]] = None,
+    start_page: int = 1,
     max_num_pages: Optional[int] = 2,
     link_filepath: Optional[str] = None,
-    print_every: int = 10,
-    verbose: bool = False,
+    delay_between_requests: float = 0.0,
 ) -> List[dict]:
-    """Crawl Khmer Times for article links with the given keyword.
+    """Crawl links for article links with the given keyword.
 
     Args:
         keyword (str): Keyword to search for.
         search_url (str, optional): URL to search for the keyword. Defaults to "https://www.khmertimeskh.com/page/{page}/?s={keyword}".
         links (List[dict], optional): List of links to append to. Defaults to None.
         max_num_pages (Optional[int], optional): Maximum number of pages to crawl. Defaults to 2.
         link_filepath (Optional[str], optional): Filepath to save the links to. Defaults to None.
         print_every (int, optional): Print progress every n pages. Defaults to 10.
         verbose (bool, optional): Print progress. Defaults to False.
 
     Returns:
         List[dict]: List of links.
     """
 
-    page = 1
-    article_no = 0  # Number of articles found
-    links = links or []
-    link_urls = [link["url"] for link in links]
+    page = start_page
+    links = []
+    link_urls = link_urls or []
     logger.info("Fetching links for keyword: %s", keyword)
-    while max_num_pages is None or page <= max_num_pages:
-        keyword = keyword.replace(" ", "+")
+    while True:
         page_url = search_url.format(page=page, keyword=keyword)
 
-        response = requests.get(page_url)
-        # Check if page exists (status code 200) or not (status code 404)
-        if response.status_code == 404:
-            logger.info("Page %s does not exist, stopping...", page)
-            break
+        logger.info("[Keyword: %s] Page: %s", keyword, page)
 
-        try:
-            soup = BeautifulSoup(response.text, "html.parser")
+        # Parse page
+        page_links = parse_page_func(page_url)
 
-            # Find the section with class 'section-category'
-            section = soup.find("section", class_="section-category")
-
-            # Find all articles within the section
-            articles = section.find_all("article")
+        # Check if page_links is None
+        if page_links is None:
+            logger.info("No more links found, stopping...")
+            break
 
-            for article in articles:
-                article_no += 1
-                # Extract and print article information
-                title = article.find("h2", class_="item-title").text
-                url = article.find("a")["href"]
-                if verbose and article_no % print_every == 0:
-                    logger.info("[Keyword: %s] Page: %s", keyword, page)
-                    logger.info("Title: %s", title)
-                    logger.info("URL: %s", url)
-                if url not in link_urls:
-                    link = {
-                        "title": title,
-                        "url": url,
-                        "keyword": keyword,
-                    }
-                    links.append(link)
-                    link_urls.append(url)
-                    if link_filepath:
-                        HyFI.append_to_jsonl(link, link_filepath)
-                else:
-                    logger.info("Link %s already exists, skipping...", url)
-        except Exception as e:
-            logger.error("Error while fetching the page url: %s", page_url)
-            logger.error(e)
+        for link in page_links:
+            if link["url"] not in link_urls:
+                link["keyword"] = keyword
+                links.append(link)
+                link_urls.append(link["url"])
+                if link_filepath:
+                    HyFI.append_to_jsonl(link, link_filepath)
+            else:
+                logger.info(
+                    "Link %s already exists, skipping...",
+                    link["url"],
+                )
 
         page += 1
 
+        if max_num_pages and page > max_num_pages:
+            logger.info("Reached max number of pages, stopping...")
+            break
+        # Delay between requests
+        if delay_between_requests > 0:
+            logger.info("Sleeping for %s seconds...", delay_between_requests)
+            time.sleep(delay_between_requests)
+
     logger.info("Finished fetching links for keyword: %s", keyword)
     logger.info("Total links fetched: %s", len(links))
     return links
 
 
 def scrape_article_text(
     links: List[dict],
-    articles: Optional[List[dict]] = None,
+    parse_article_func: Callable,
+    article_urls: Optional[List[dict]] = None,
     overwrite_existing: bool = False,
     max_num_articles: Optional[int] = 10,
     article_filepath: Optional[str] = None,
+    delay_between_requests: float = 0.0,
     print_every: int = 10,
     verbose: bool = False,
 ) -> List[dict]:
     """Scrape the article text from the given links.
 
     Args:
         links (List[dict]): List of links to scrape.
@@ -299,83 +310,46 @@
         article_filepath (Optional[str], optional): Filepath to save the articles to. Defaults to None.
         print_every (int, optional): Print progress every n articles. Defaults to 10.
         verbose (bool, optional): Print progress. Defaults to False.
 
     Returns:
         List[dict]: List of articles.
     """
-    articles = articles or []
-    article_urls = [article["url"] for article in articles]
+    articles = []
+    article_urls = article_urls or []
     for i, link in enumerate(links):
         if max_num_articles is not None and i >= max_num_articles:
             logger.info("Reached max number of articles, stopping...")
             break
 
         url = link["url"]
         title = link["title"]
-        keyword = link["keyword"]
         if url in article_urls and not overwrite_existing:
             logger.info("Article [%s](%s) already exists, skipping...", title, url)
             continue
 
-        try:
-            response = requests.get(url)
-            soup = BeautifulSoup(response.text, "html.parser")
-
-            # Find the div with class 'entry-content'
-            entry_content_div = soup.find("div", class_="entry-content")
-
-            # Find the div with class 'entry-meta'
-            entry_meta_div = soup.find("div", class_="entry-meta")
-
-            if entry_content_div and entry_meta_div:
-                article = parse_article_text(
-                    entry_content_div,
-                    entry_meta_div,
-                    url=url,
-                    keyword=keyword,
-                    title=title,
-                )
-                articles.append(article)
-                article_urls.append(url)
-                if article_filepath:
-                    HyFI.append_to_jsonl(article, article_filepath)
-                if verbose and (i + 1) % print_every == 0:
-                    logger.info("Article [%s](%s) scraped", title, url)
-            else:
-                logger.info("Article [%s](%s) does not exist, skipping...", title, url)
-        except Exception as e:
-            logger.error("Error while scraping the article url: %s", url)
-            logger.error(e)
+        # Parse article
+        _article = parse_article_func(url)
+        if _article is None:
+            logger.info(
+                "Article [%s](%s) does not exist, skipping...",
+                title,
+                url,
+            )
+            continue
+        article = link.copy()
+        article.update(_article)
+        articles.append(article)
+        article_urls.append(url)
+        if article_filepath:
+            HyFI.append_to_jsonl(article, article_filepath)
+        if (verbose and (i + 1) % print_every == 0) or delay_between_requests > 0:
+            logger.info("Article [%s](%s) scraped", title, url)
+
+        # Delay between requests
+        if delay_between_requests > 0 and i < len(links) - 1:
+            logger.info("Sleeping for %s seconds...", delay_between_requests)
+            time.sleep(delay_between_requests)
 
     logger.info("Finished scraping articles")
     logger.info("Total articles scraped: %s", len(articles))
     return articles
-
-
-def parse_article_text(
-    entry_content_div,
-    entry_meta_div,
-    url: str,
-    keyword: str,
-    title: str,
-) -> dict:
-    """Parse the article text from the given divs."""
-    # Find all p tags within the div and extract the text
-    p_tags = entry_content_div.find_all("p")
-    article_text = "\n".join(p_tag.text for p_tag in p_tags)
-
-    # Extract the entry categories
-    entry_categories = [a_tag.text for a_tag in entry_meta_div.find_all("a", rel="tag")]
-
-    # Extract the entry time and convert it to a datetime object
-    entry_time_str = entry_meta_div.find("time", class_="entry-time")["datetime"]
-    entry_time = datetime.fromisoformat(entry_time_str)
-
-    return {
-        "url": url,
-        "keyword": keyword,
-        "title": title,
-        "categories": entry_categories,
-        "time": entry_time.isoformat(),  # Convert datetime to string
-        "text": article_text,
-    }
```

### Comparing `nbcpu-0.4.0/PKG-INFO` & `nbcpu-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbcpu
-Version: 0.4.0
+Version: 0.5.0
 Summary: Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach
 Home-page: https://entelecheia.github.io/nbcpu
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

