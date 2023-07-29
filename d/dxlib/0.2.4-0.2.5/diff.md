# Comparing `tmp/dxlib-0.2.4.tar.gz` & `tmp/dxlib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.2.4.tar", last modified: Sat Jul 29 07:37:53 2023, max compression
+gzip compressed data, was "dxlib-0.2.5.tar", last modified: Sat Jul 29 07:42:04 2023, max compression
```

## Comparing `dxlib-0.2.4.tar` & `dxlib-0.2.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.863823 dxlib-0.2.4/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)    10948 2023-07-16 21:40:36.000000 dxlib-0.2.4/LICENSE
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:37:53.859819 dxlib-0.2.4/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2487 2023-07-16 21:40:36.000000 dxlib-0.2.4/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:52.823392 dxlib-0.2.4/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.158405 dxlib-0.2.4/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      114 2023-07-29 07:33:31.000000 dxlib-0.2.4/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      541 2023-07-29 07:28:35.000000 dxlib-0.2.4/dxlib/api/alpaca_markets.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3117 2023-07-29 07:33:09.000000 dxlib-0.2.4/dxlib/api/core.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.4/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.4/dxlib/api/terminal.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.309404 dxlib-0.2.4/dxlib/core/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.4/dxlib/core/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/core/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/core/finite_differences.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     9503 2023-07-25 00:10:53.000000 dxlib-0.2.4/dxlib/core/options.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.385403 dxlib-0.2.4/dxlib/data/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/data/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.2.4/dxlib/data/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.459404 dxlib-0.2.4/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      603 2023-07-17 19:47:05.000000 dxlib-0.2.4/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.597123 dxlib-0.2.4/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.4/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.4/dxlib/db/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.676124 dxlib-0.2.4/dxlib/models/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.4/dxlib/models/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:26:00.000000 dxlib-0.2.4/dxlib/models/systematic_trading.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     5388 2023-07-29 07:35:54.000000 dxlib-0.2.4/dxlib/portfolio_theory_module.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.713127 dxlib-0.2.4/dxlib/research/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.4/dxlib/research/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.787999 dxlib-0.2.4/dxlib/simulation/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.4/dxlib/simulation/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.4/dxlib/simulation/backtesting.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      311 2023-07-29 07:36:07.000000 dxlib-0.2.4/dxlib/test.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.825822 dxlib-0.2.4/dxlib/visualization/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.4/dxlib/visualization/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:52.953407 dxlib-0.2.4/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      810 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       96 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-29 07:37:53.864823 dxlib-0.2.4/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.4/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:04.338542 dxlib-0.2.5/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)    10948 2023-07-16 21:40:36.000000 dxlib-0.2.5/LICENSE
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:42:04.334541 dxlib-0.2.5/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2487 2023-07-16 21:40:36.000000 dxlib-0.2.5/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:03.292771 dxlib-0.2.5/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.5/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:03.653378 dxlib-0.2.5/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      117 2023-07-29 07:41:11.000000 dxlib-0.2.5/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      544 2023-07-29 07:41:00.000000 dxlib-0.2.5/dxlib/api/alpaca_markets.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.5/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3117 2023-07-29 07:33:09.000000 dxlib-0.2.5/dxlib/api/core.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.5/dxlib/api/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.5/dxlib/api/terminal.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:03.798542 dxlib-0.2.5/dxlib/core/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.5/dxlib/core/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.5/dxlib/core/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.5/dxlib/core/finite_differences.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     9503 2023-07-25 00:10:53.000000 dxlib-0.2.5/dxlib/core/options.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:03.871543 dxlib-0.2.5/dxlib/data/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.5/dxlib/data/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.2.5/dxlib/data/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:03.945542 dxlib-0.2.5/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      603 2023-07-17 19:47:05.000000 dxlib-0.2.5/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:04.078542 dxlib-0.2.5/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.5/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.5/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.5/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.5/dxlib/db/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:04.155542 dxlib-0.2.5/dxlib/models/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.5/dxlib/models/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:26:00.000000 dxlib-0.2.5/dxlib/models/systematic_trading.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     5388 2023-07-29 07:35:54.000000 dxlib-0.2.5/dxlib/portfolio_theory_module.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:04.191542 dxlib-0.2.5/dxlib/research/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.5/dxlib/research/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:04.264541 dxlib-0.2.5/dxlib/simulation/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.5/dxlib/simulation/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.5/dxlib/simulation/backtesting.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      218 2023-07-29 07:41:51.000000 dxlib-0.2.5/dxlib/test.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:04.301541 dxlib-0.2.5/dxlib/visualization/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.5/dxlib/visualization/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:42:03.430772 dxlib-0.2.5/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:42:02.000000 dxlib-0.2.5/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      810 2023-07-29 07:42:03.000000 dxlib-0.2.5/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-29 07:42:02.000000 dxlib-0.2.5/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       96 2023-07-29 07:42:02.000000 dxlib-0.2.5/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-29 07:42:02.000000 dxlib-0.2.5/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-29 07:42:04.339543 dxlib-0.2.5/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.5/setup.py
```

### Comparing `dxlib-0.2.4/LICENSE` & `dxlib-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/PKG-INFO` & `dxlib-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.4/README.md` & `dxlib-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/api/alpaca_markets.py` & `dxlib-0.2.5/dxlib/api/alpaca_markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 
 from .core import Api
 
 
-class AlpacaMarkets(Api):
+class AlpacaMarketsAPI(Api):
     def __init__(self, api_key, api_secret):
         super().__init__(api_key, api_secret, 'https://data.alpaca.markets', 'v2')
 
     class Endpoints(Enum):
         stocks = 'stocks'
         exchanges = 'exchanges'
         symbols = 'symbols'
```

### Comparing `dxlib-0.2.4/dxlib/api/alphavantage.py` & `dxlib-0.2.5/dxlib/api/alphavantage.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/api/core.py` & `dxlib-0.2.5/dxlib/api/core.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/core/options.py` & `dxlib-0.2.5/dxlib/core/options.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/data/utils.py` & `dxlib-0.2.5/dxlib/data/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/db/__init__.py` & `dxlib-0.2.5/dxlib/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/db/sql/queries.py` & `dxlib-0.2.5/dxlib/db/sql/queries.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/db/utils.py` & `dxlib-0.2.5/dxlib/db/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/portfolio_theory_module.py` & `dxlib-0.2.5/dxlib/portfolio_theory_module.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib/simulation/backtesting.py` & `dxlib-0.2.5/dxlib/simulation/backtesting.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/dxlib.egg-info/PKG-INFO` & `dxlib-0.2.5/dxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.4/dxlib.egg-info/SOURCES.txt` & `dxlib-0.2.5/dxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.4/setup.py` & `dxlib-0.2.5/setup.py`

 * *Files identical despite different names*

