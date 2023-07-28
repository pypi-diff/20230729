# Comparing `tmp/trading-backend-1.2.5.tar.gz` & `tmp/trading-backend-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading-backend-1.2.5.tar", last modified: Tue Jul  4 18:45:18 2023, max compression
+gzip compressed data, was "trading-backend-1.2.6.tar", last modified: Fri Jul 28 23:33:14 2023, max compression
```

## Comparing `trading-backend-1.2.5.tar` & `trading-backend-1.2.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.885764 trading-backend-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-04 18:44:49.000000 trading-backend-1.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-04 18:44:49.000000 trading-backend-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-04 18:44:49.000000 trading-backend-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-04 18:45:18.885764 trading-backend-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-04 18:44:49.000000 trading-backend-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 18:44:49.000000 trading-backend-1.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-04 18:45:18.885764 trading-backend-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-04 18:44:49.000000 trading-backend-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_kucoin_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_mexc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/exchanges/test_phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-04 18:44:49.000000 trading-backend-1.2.5/tests/util/create_order_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.881764 trading-backend-1.2.5/trading_backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchange_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.885764 trading-backend-1.2.5/trading_backend/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/kucoinfutures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/mexc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-04 18:44:49.000000 trading-backend-1.2.5/trading_backend/exchanges/phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:18.885764 trading-backend-1.2.5/trading_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 18:45:18.000000 trading-backend-1.2.5/trading_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:33:14.835923 trading-backend-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-28 23:32:32.000000 trading-backend-1.2.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-28 23:32:32.000000 trading-backend-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 23:32:32.000000 trading-backend-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-28 23:33:14.835923 trading-backend-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-28 23:32:32.000000 trading-backend-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 23:32:32.000000 trading-backend-1.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-28 23:33:14.835923 trading-backend-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-28 23:32:32.000000 trading-backend-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:33:14.827923 trading-backend-1.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:33:14.831923 trading-backend-1.2.6/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/exchanges/test_phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:33:14.831923 trading-backend-1.2.6/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-28 23:32:32.000000 trading-backend-1.2.6/tests/util/create_order_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:33:14.831923 trading-backend-1.2.6/trading_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchange_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:33:14.835923 trading-backend-1.2.6/trading_backend/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/kucoinfutures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-28 23:32:32.000000 trading-backend-1.2.6/trading_backend/exchanges/phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:33:14.831923 trading-backend-1.2.6/trading_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-28 23:33:14.000000 trading-backend-1.2.6/trading_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-28 23:33:14.000000 trading-backend-1.2.6/trading_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:33:14.000000 trading-backend-1.2.6/trading_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:33:14.000000 trading-backend-1.2.6/trading_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 23:33:14.000000 trading-backend-1.2.6/trading_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 23:33:14.000000 trading-backend-1.2.6/trading_backend.egg-info/top_level.txt
```

### Comparing `trading-backend-1.2.5/CHANGELOG.md` & `trading-backend-1.2.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.6] - 2023-07-29
+### Fixed
+- Binance support check
+
 ## [1.2.5] - 2023-06-29
 ### Added
 - Crypto.com
 - MEXC
 
 ## [1.2.4] - 2023-06-24
 ### Added
```

### Comparing `trading-backend-1.2.5/LICENSE` & `trading-backend-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/PKG-INFO` & `trading-backend-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.5
+Version: 1.2.6
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.5](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.6](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.5/README.md` & `trading-backend-1.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# trading-backend [1.2.5](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.6](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.5/setup.py` & `trading-backend-1.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 # from distutils.extension import Extension
 from setuptools import find_packages
 from setuptools import setup
 
-VERSION = "1.2.5"
+VERSION = "1.2.6"
 PROJECT_NAME = "trading-backend"
 
 PACKAGES = find_packages(exclude=["tests"])
 
 
 # long description from README file
 with open('README.md', encoding='utf-8') as f:
```

### Comparing `trading-backend-1.2.5/tests/exchanges/test_ascendex.py` & `trading-backend-1.2.6/tests/exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_binance.py` & `trading-backend-1.2.6/tests/exchanges/test_binance.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_bitget.py` & `trading-backend-1.2.6/tests/exchanges/test_bitget.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_bybit.py` & `trading-backend-1.2.6/tests/exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_cryptocom.py` & `trading-backend-1.2.6/tests/exchanges/test_cryptocom.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_exchange.py` & `trading-backend-1.2.6/tests/exchanges/test_exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_gateio.py` & `trading-backend-1.2.6/tests/exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_huobi.py` & `trading-backend-1.2.6/tests/exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_huobipro.py` & `trading-backend-1.2.6/tests/exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_kucoin.py` & `trading-backend-1.2.6/tests/exchanges/test_kucoin.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_kucoin_futures.py` & `trading-backend-1.2.6/tests/exchanges/test_kucoin_futures.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_mexc.py` & `trading-backend-1.2.6/tests/exchanges/test_mexc.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_okx.py` & `trading-backend-1.2.6/tests/exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/exchanges/test_phemex.py` & `trading-backend-1.2.6/tests/exchanges/test_phemex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/util/__init__.py` & `trading-backend-1.2.6/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/tests/util/create_order_tests.py` & `trading-backend-1.2.6/tests/util/create_order_tests.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/__init__.py` & `trading-backend-1.2.6/trading_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/errors.py` & `trading-backend-1.2.6/trading_backend/errors.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchange_factory.py` & `trading-backend-1.2.6/trading_backend/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/__init__.py` & `trading-backend-1.2.6/trading_backend/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/ascendex.py` & `trading-backend-1.2.6/trading_backend/exchanges/ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/binance.py` & `trading-backend-1.2.6/trading_backend/exchanges/binance.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,17 +66,17 @@
                 return f"Broker rebate not working: {details}"
             return f"Broker rebate is enabled."
         except Exception as err:
             return f"Broker rebate check error: {err}"
 
     async def _get_account_referral_details(self) -> dict:
         return await self._exchange.connector.client.sapi_get_apireferral_ifnewuser(
-            params=self._exchange._get_params({
+            params={
                 "apiAgentCode": self._get_id()
-            })
+            }
         )
 
     async def _inner_is_valid_account(self) -> (bool, str):
         details = None
         try:
             details = await self._get_account_referral_details()
             if not details.get("rebateWorking", False):
```

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/bitget.py` & `trading-backend-1.2.6/trading_backend/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/bybit.py` & `trading-backend-1.2.6/trading_backend/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/cryptocom.py` & `trading-backend-1.2.6/trading_backend/exchanges/cryptocom.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/exchange.py` & `trading-backend-1.2.6/trading_backend/exchanges/exchange.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/gateio.py` & `trading-backend-1.2.6/trading_backend/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/huobi.py` & `trading-backend-1.2.6/trading_backend/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/huobipro.py` & `trading-backend-1.2.6/trading_backend/exchanges/huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/kucoin.py` & `trading-backend-1.2.6/trading_backend/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/kucoinfutures.py` & `trading-backend-1.2.6/trading_backend/exchanges/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/mexc.py` & `trading-backend-1.2.6/trading_backend/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/okx.py` & `trading-backend-1.2.6/trading_backend/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend/exchanges/phemex.py` & `trading-backend-1.2.6/trading_backend/exchanges/phemex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.5/trading_backend.egg-info/PKG-INFO` & `trading-backend-1.2.6/trading_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.5
+Version: 1.2.6
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.5](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.6](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.5/trading_backend.egg-info/SOURCES.txt` & `trading-backend-1.2.6/trading_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

