# Comparing `tmp/amazon_scrape-1.0.5.tar.gz` & `tmp/amazon_scrape-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-1.0.5.tar", last modified: Fri Jul 28 11:12:20 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-1.0.6.tar", last modified: Sat Jul 29 09:21:52 2023, max compression
```

## Comparing `amazon_scrape-1.0.5.tar` & `amazon_scrape-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 11:12:20.221282 amazon_scrape-1.0.5/
--rw-r--r--   0 finn       (501) staff       (20)     5112 2023-07-28 11:12:20.221505 amazon_scrape-1.0.5/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2373 2023-07-28 11:12:07.000000 amazon_scrape-1.0.5/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 11:12:20.218734 amazon_scrape-1.0.5/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5112 2023-07-28 11:12:20.000000 amazon_scrape-1.0.5/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-28 11:12:20.000000 amazon_scrape-1.0.5/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 11:12:20.000000 amazon_scrape-1.0.5/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-28 11:12:20.000000 amazon_scrape-1.0.5/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:32:12.000000 amazon_scrape-1.0.5/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-28 11:12:20.000000 amazon_scrape-1.0.5/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-28 11:12:20.000000 amazon_scrape-1.0.5/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-28 11:12:20.220687 amazon_scrape-1.0.5/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:31:54.000000 amazon_scrape-1.0.5/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     8368 2023-07-28 09:06:51.000000 amazon_scrape-1.0.5/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-28 11:10:55.000000 amazon_scrape-1.0.5/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-28 11:12:20.222197 amazon_scrape-1.0.5/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-28 11:10:55.000000 amazon_scrape-1.0.5/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-29 09:21:52.800992 amazon_scrape-1.0.6/
+-rw-r--r--   0 finn       (501) staff       (20)     5112 2023-07-29 09:21:52.801289 amazon_scrape-1.0.6/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2373 2023-07-28 11:12:07.000000 amazon_scrape-1.0.6/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-29 09:21:52.797811 amazon_scrape-1.0.6/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5112 2023-07-29 09:21:52.000000 amazon_scrape-1.0.6/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-29 09:21:52.000000 amazon_scrape-1.0.6/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-29 09:21:52.000000 amazon_scrape-1.0.6/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-29 09:21:52.000000 amazon_scrape-1.0.6/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-28 06:32:12.000000 amazon_scrape-1.0.6/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-29 09:21:52.000000 amazon_scrape-1.0.6/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-29 09:21:52.000000 amazon_scrape-1.0.6/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-29 09:21:52.800159 amazon_scrape-1.0.6/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-28 06:31:54.000000 amazon_scrape-1.0.6/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     8041 2023-07-29 09:20:58.000000 amazon_scrape-1.0.6/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-29 08:00:09.000000 amazon_scrape-1.0.6/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-29 09:21:52.802158 amazon_scrape-1.0.6/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-29 08:00:09.000000 amazon_scrape-1.0.6/setup.py
```

### Comparing `amazon_scrape-1.0.5/PKG-INFO` & `amazon_scrape-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 1.0.5
+Version: 1.0.6
 Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_scrape-1.0.5/README.md` & `amazon_scrape-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `amazon_scrape-1.0.5/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-1.0.6/amazon_scrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 1.0.5
+Version: 1.0.6
 Summary: Scrape Amazon product data such as Product Name, Product Images, Number of Reviews, Price, Product URL, and ASIN.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_scrape-1.0.5/amazon_scraper/scraper.py` & `amazon_scrape-1.0.6/amazon_scraper/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 from bs4 import BeautifulSoup
 import csv
 import json
 import random
 import argparse
+from tqdm import tqdm
 
 class AmazonScraper:
     user_agents = [
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3",
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:61.0) Gecko/20100101 Firefox/61.0",
         "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.181 Safari/537.36",
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36",
@@ -48,87 +49,76 @@
         self.review_json_data = []
         self.locale = locale
 
     def start_scraping(self):
         self.product_writer.writerow(["product_name", "product_images", "number_of_reviews", "price", "product_url", "asin"])
         if self.review:
             self.review_writer.writerow(["product_name", "product_reviews", "product_url", "asin"])
-        for page in range(1, self.pages + 1):
+        for page in tqdm(range(1, self.pages + 1), desc="Scraping Pages"):
             url = self.url + "&page=" + str(page)
             headers = {"User-Agent": random.choice(self.user_agents)}
             response = requests.get(url, headers=headers)
             soup = BeautifulSoup(response.content, "html.parser")
             products = soup.find_all("div", {"class": "sg-col-inner"})
 
             for product in products:
-                # Product name
                 name = product.find("span", {"class": "a-size-medium a-color-base a-text-normal"})
                 if name is not None:
                     name = name.text
                 else:
-                    continue  # Skip if no product name
+                    continue
 
-                # Product images
                 images = product.find_all("img", {"class": "s-image"})
                 if images is not None:
                     images = [image['src'] for image in images]
                 else:
                     images = []
 
-                # Number of Reviews
                 number_of_reviews = product.find("span", {"class": "a-size-base"})
                 if number_of_reviews is not None:
                     number_of_reviews = number_of_reviews.text
                 else:
                     number_of_reviews = ''
 
-                # Price
                 price = product.find("span", {"class": "a-offscreen"})
                 if price is not None:
                     price = price.text
                 else:
                     price = ''
 
-                # Product URL
                 product_url = product.find("a", {"class": "a-link-normal"})
                 if product_url is not None:
                     product_url = f'https://www.amazon.{self.locale}' + product_url['href']
                 else:
                     product_url = ''
 
-                # ASIN
                 asin = product_url.split("/dp/")[1].split("/")[0] if "/dp/" in product_url else ''
 
-                # Write to CSV
                 self.product_writer.writerow([name, ", ".join(images), number_of_reviews, price, product_url, asin])
 
-                # Add to JSON data
                 self.product_json_data.append({
                     "product_name": name,
                     "product_images": images,
                     "number_of_reviews": number_of_reviews,
                     "price": price,
                     "product_url": product_url,
                     "asin": asin
                 })
 
-                # Product reviews
                 if self.review:
                     product_reviews = []
                     review_url = f'https://www.amazon.{self.locale}/product-reviews/{asin}'
                     review_response = requests.get(review_url, headers=headers)
                     review_soup = BeautifulSoup(review_response.content, "html.parser")
                     reviews = review_soup.find_all("span", {"data-hook": "review-body"})
                     for review in reviews:
                         product_reviews.append(review.text.strip())
 
-                    # Write to CSV
                     self.review_writer.writerow([name, ", ".join(product_reviews), product_url, asin])
 
-                    # Add to JSON data
                     self.review_json_data.append({
                         "product_name": name,
                         "product_reviews": product_reviews,
                         "product_url": product_url,
                         "asin": asin
                     })
```

### Comparing `amazon_scrape-1.0.5/setup.py` & `amazon_scrape-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

