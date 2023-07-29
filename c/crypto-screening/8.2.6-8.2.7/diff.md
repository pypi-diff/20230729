# Comparing `tmp/crypto-screening-8.2.6.tar.gz` & `tmp/crypto-screening-8.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.2.6.tar", last modified: Sat Jul 29 10:35:15 2023, max compression
+gzip compressed data, was "crypto-screening-8.2.7.tar", last modified: Sat Jul 29 10:57:34 2023, max compression
```

## Comparing `crypto-screening-8.2.6.tar` & `crypto-screening-8.2.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.790093 crypto-screening-8.2.6/
--rw-rw-rw-   0        0        0      196 2023-07-29 10:35:13.000000 crypto-screening-8.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-29 10:35:15.790093 crypto-screening-8.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.6/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.6/build.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.560717 crypto-screening-8.2.6/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.598681 crypto-screening-8.2.6/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.6/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4940 2023-07-27 15:04:17.000000 crypto-screening-8.2.6/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.627711 crypto-screening-8.2.6/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.6/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.6/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.650710 crypto-screening-8.2.6/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.6/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    20755 2023-07-27 15:10:03.000000 crypto-screening-8.2.6/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19564 2023-07-27 15:04:24.000000 crypto-screening-8.2.6/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-29 10:34:53.000000 crypto-screening-8.2.6/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.6/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.2.6/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.715047 crypto-screening-8.2.6/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.6/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    23843 2023-07-27 14:49:56.000000 crypto-screening-8.2.6/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.738228 crypto-screening-8.2.6/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.6/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.6/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.761226 crypto-screening-8.2.6/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.6/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.6/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.6/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.6/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.2.6/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.779120 crypto-screening-8.2.6/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.2.6/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.6/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.6/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.6/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.6/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.2.6/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.2.6/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.2.6/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.6/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.2.6/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.6/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.541709 crypto-screening-8.2.6/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.780092 crypto-screening-8.2.6/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.6/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10390 2023-07-29 10:33:38.000000 crypto-screening-8.2.6/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.789109 crypto-screening-8.2.6/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.6/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.6/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.6/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:35:15.576134 crypto-screening-8.2.6/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-29 10:35:15.000000 crypto-screening-8.2.6/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-29 10:35:15.000000 crypto-screening-8.2.6/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:35:15.000000 crypto-screening-8.2.6/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-29 10:35:15.000000 crypto-screening-8.2.6/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-29 10:35:15.000000 crypto-screening-8.2.6/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-29 10:35:13.000000 crypto-screening-8.2.6/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 10:35:15.790093 crypto-screening-8.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-29 10:35:07.000000 crypto-screening-8.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.285184 crypto-screening-8.2.7/
+-rw-rw-rw-   0        0        0      196 2023-07-29 10:57:33.000000 crypto-screening-8.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-29 10:57:34.285184 crypto-screening-8.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.7/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.7/build.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.232668 crypto-screening-8.2.7/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.255670 crypto-screening-8.2.7/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.7/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4940 2023-07-27 15:04:17.000000 crypto-screening-8.2.7/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.260673 crypto-screening-8.2.7/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.7/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.7/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.263679 crypto-screening-8.2.7/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.7/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    20755 2023-07-27 15:10:03.000000 crypto-screening-8.2.7/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19564 2023-07-27 15:04:24.000000 crypto-screening-8.2.7/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-29 10:34:53.000000 crypto-screening-8.2.7/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.7/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.2.7/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.273674 crypto-screening-8.2.7/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.7/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23844 2023-07-29 10:57:24.000000 crypto-screening-8.2.7/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.276186 crypto-screening-8.2.7/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.7/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.7/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.279185 crypto-screening-8.2.7/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.7/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.7/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.7/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.7/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.2.7/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.282184 crypto-screening-8.2.7/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.2.7/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.7/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.7/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.7/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.7/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.2.7/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.2.7/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.2.7/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.7/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.2.7/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.7/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.224342 crypto-screening-8.2.7/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.282184 crypto-screening-8.2.7/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.7/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10390 2023-07-29 10:33:38.000000 crypto-screening-8.2.7/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.284185 crypto-screening-8.2.7/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.7/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.7/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.7/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:57:34.251668 crypto-screening-8.2.7/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-29 10:57:34.000000 crypto-screening-8.2.7/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-29 10:57:34.000000 crypto-screening-8.2.7/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:57:34.000000 crypto-screening-8.2.7/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-29 10:57:34.000000 crypto-screening-8.2.7/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-29 10:57:34.000000 crypto-screening-8.2.7/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-29 10:57:33.000000 crypto-screening-8.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.7/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 10:57:34.285184 crypto-screening-8.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-29 10:57:31.000000 crypto-screening-8.2.7/setup.py
```

### Comparing `crypto-screening-8.2.6/PKG-INFO` & `crypto-screening-8.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.6
+Version: 8.2.7
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.6/README.md` & `crypto-screening-8.2.7/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/build.py` & `crypto-screening-8.2.7/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/assets.py` & `crypto-screening-8.2.7/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/exchanges.py` & `crypto-screening-8.2.7/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.2.7/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.2.7/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/market/orders.py` & `crypto-screening-8.2.7/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.2.7/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.2.7/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.2.7/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/market/trades.py` & `crypto-screening-8.2.7/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/screeners.py` & `crypto-screening-8.2.7/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/collect/symbols.py` & `crypto-screening-8.2.7/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/dataset.py` & `crypto-screening-8.2.7/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/exchanges.py` & `crypto-screening-8.2.7/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/interval.py` & `crypto-screening-8.2.7/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/base.py` & `crypto-screening-8.2.7/crypto_screening/screeners/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
 
     def find_screeners(
             self,
             exchange: Optional[str] = None,
             symbol: Optional[str] = None,
             base: Optional[Type[_S]] = None,
             interval: Optional[str] = None,
-            adjust: Optional[bool] = True
+            adjust: Optional[bool] = False
     ) -> List[_S]:
         """
         Returns the data by according to the parameters.
 
         :param base: The base type of the screener.
         :param exchange: The exchange name.
         :param symbol: The symbol name.
```

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.2.7/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.2.7/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.2.7/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.2.7/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.2.7/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.2.7/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/combined.py` & `crypto-screening-8.2.7/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/container.py` & `crypto-screening-8.2.7/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/database.py` & `crypto-screening-8.2.7/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.2.7/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.2.7/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.2.7/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.2.7/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/market.py` & `crypto-screening-8.2.7/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.2.7/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.2.7/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/orders.py` & `crypto-screening-8.2.7/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/recorder.py` & `crypto-screening-8.2.7/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/trades.py` & `crypto-screening-8.2.7/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/screeners/waiting.py` & `crypto-screening-8.2.7/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.2.7/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/symbols.py` & `crypto-screening-8.2.7/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/utils/base.py` & `crypto-screening-8.2.7/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/utils/process.py` & `crypto-screening-8.2.7/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening/validate.py` & `crypto-screening-8.2.7/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.2.7/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.6
+Version: 8.2.7
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.6/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.2.7/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.6/pyproject.toml` & `crypto-screening-8.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.2.6'
+version = '8.2.7'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.2.6/setup.py` & `crypto-screening-8.2.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.2.6',
+        version='8.2.7',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

