# Comparing `tmp/dxlib-0.2.3.tar.gz` & `tmp/dxlib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.2.3.tar", last modified: Sat Jul 15 09:58:55 2023, max compression
+gzip compressed data, was "dxlib-0.2.4.tar", last modified: Sat Jul 29 07:37:53 2023, max compression
```

## Comparing `dxlib-0.2.3.tar` & `dxlib-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.435587 dxlib-0.2.3/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 09:58:55.432585 dxlib-0.2.3/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      981 2023-07-15 07:58:15.000000 dxlib-0.2.3/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:54.746892 dxlib-0.2.3/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:54.944587 dxlib-0.2.3/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       73 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.3/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.3/dxlib/api/terminal.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.018837 dxlib-0.2.3/dxlib/core/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.3/dxlib/core/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/core/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/core/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.068677 dxlib-0.2.3/dxlib/data/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/data/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.2.3/dxlib/data/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.118496 dxlib-0.2.3/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.3/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.211680 dxlib-0.2.3/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.3/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.3/dxlib/db/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.312093 dxlib-0.2.3/dxlib/models/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.3/dxlib/models/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2338 2023-07-15 08:38:49.000000 dxlib-0.2.3/dxlib/models/options.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-28 17:50:38.000000 dxlib-0.2.3/dxlib/models/pricing.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:26:00.000000 dxlib-0.2.3/dxlib/models/systematic_trading.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.336120 dxlib-0.2.3/dxlib/research/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.3/dxlib/research/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.384850 dxlib-0.2.3/dxlib/simulation/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.3/dxlib/simulation/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.3/dxlib/simulation/backtesting.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.410540 dxlib-0.2.3/dxlib/visualization/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.3/dxlib/visualization/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:54.842620 dxlib-0.2.3/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      735 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       96 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 09:58:55.436589 dxlib-0.2.3/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.3/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.863823 dxlib-0.2.4/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)    10948 2023-07-16 21:40:36.000000 dxlib-0.2.4/LICENSE
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:37:53.859819 dxlib-0.2.4/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2487 2023-07-16 21:40:36.000000 dxlib-0.2.4/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:52.823392 dxlib-0.2.4/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.158405 dxlib-0.2.4/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      114 2023-07-29 07:33:31.000000 dxlib-0.2.4/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      541 2023-07-29 07:28:35.000000 dxlib-0.2.4/dxlib/api/alpaca_markets.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3117 2023-07-29 07:33:09.000000 dxlib-0.2.4/dxlib/api/core.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.4/dxlib/api/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.4/dxlib/api/terminal.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.309404 dxlib-0.2.4/dxlib/core/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.4/dxlib/core/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/core/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/core/finite_differences.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     9503 2023-07-25 00:10:53.000000 dxlib-0.2.4/dxlib/core/options.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.385403 dxlib-0.2.4/dxlib/data/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/data/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.2.4/dxlib/data/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.459404 dxlib-0.2.4/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      603 2023-07-17 19:47:05.000000 dxlib-0.2.4/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.597123 dxlib-0.2.4/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.4/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.4/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.4/dxlib/db/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.676124 dxlib-0.2.4/dxlib/models/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.4/dxlib/models/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:26:00.000000 dxlib-0.2.4/dxlib/models/systematic_trading.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     5388 2023-07-29 07:35:54.000000 dxlib-0.2.4/dxlib/portfolio_theory_module.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.713127 dxlib-0.2.4/dxlib/research/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.4/dxlib/research/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.787999 dxlib-0.2.4/dxlib/simulation/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.4/dxlib/simulation/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.4/dxlib/simulation/backtesting.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      311 2023-07-29 07:36:07.000000 dxlib-0.2.4/dxlib/test.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:53.825822 dxlib-0.2.4/dxlib/visualization/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.4/dxlib/visualization/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:37:52.953407 dxlib-0.2.4/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      810 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       96 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-29 07:37:52.000000 dxlib-0.2.4/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-29 07:37:53.864823 dxlib-0.2.4/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.4/setup.py
```

### Comparing `dxlib-0.2.3/dxlib/api/alphavantage.py` & `dxlib-0.2.4/dxlib/api/alphavantage.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.3/dxlib/data/utils.py` & `dxlib-0.2.4/dxlib/data/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.3/dxlib/db/sql/queries.py` & `dxlib-0.2.4/dxlib/db/sql/queries.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.3/dxlib/db/utils.py` & `dxlib-0.2.4/dxlib/db/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.3/dxlib/simulation/backtesting.py` & `dxlib-0.2.4/dxlib/simulation/backtesting.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.3/dxlib.egg-info/SOURCES.txt` & `dxlib-0.2.4/dxlib.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
+LICENSE
 README.md
 setup.py
 dxlib/__init__.py
+dxlib/portfolio_theory_module.py
+dxlib/test.py
 dxlib.egg-info/PKG-INFO
 dxlib.egg-info/SOURCES.txt
 dxlib.egg-info/dependency_links.txt
 dxlib.egg-info/requires.txt
 dxlib.egg-info/top_level.txt
 dxlib/api/__init__.py
+dxlib/api/alpaca_markets.py
 dxlib/api/alphavantage.py
+dxlib/api/core.py
 dxlib/api/logger.py
 dxlib/api/terminal.py
 dxlib/core/__init__.py
 dxlib/core/euler_method.py
 dxlib/core/finite_differences.py
+dxlib/core/options.py
 dxlib/data/__init__.py
 dxlib/data/utils.py
 dxlib/db/__init__.py
 dxlib/db/utils.py
 dxlib/db/sql/__init__.py
 dxlib/db/sql/create.py
 dxlib/db/sql/queries.py
 dxlib/models/__init__.py
-dxlib/models/options.py
-dxlib/models/pricing.py
 dxlib/models/systematic_trading.py
 dxlib/research/__init__.py
 dxlib/simulation/__init__.py
 dxlib/simulation/backtesting.py
 dxlib/visualization/__init__.py
```

### Comparing `dxlib-0.2.3/setup.py` & `dxlib-0.2.4/setup.py`

 * *Files identical despite different names*

