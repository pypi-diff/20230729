# Comparing `tmp/aio_dt_protocol-1.2.0.tar.gz` & `tmp/aio_dt_protocol-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-1.2.0.tar", last modified: Fri Jul 28 18:21:24 2023, max compression
+gzip compressed data, was "aio_dt_protocol-1.2.1.tar", last modified: Sat Jul 29 13:50:59 2023, max compression
```

## Comparing `aio_dt_protocol-1.2.0.tar` & `aio_dt_protocol-1.2.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.945951 aio_dt_protocol-1.2.0/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     8069 2023-07-28 18:21:24.945951 aio_dt_protocol-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7302 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.894969 aio_dt_protocol-1.2.0/aio_dt_protocol/
--rw-rw-rw-   0        0        0      503 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/__init__.py
--rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/actions.py
--rw-rw-rw-   0        0        0    56344 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/browser.py
--rw-rw-rw-   0        0        0    17231 2023-07-28 18:01:34.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/connection.py
--rw-rw-rw-   0        0        0    25802 2023-07-28 10:14:12.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/data.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.900966 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.903965 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/
--rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/__init__.py
--rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/background_service.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.906964 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/__init__.py
--rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/browser.py
--rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.909963 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/__init__.py
--rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/css.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.911963 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/
--rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/__init__.py
--rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/device_orientation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.915961 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/
--rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/__init__.py
--rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom.py
--rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom_element.py
--rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.918960 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/
--rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/__init__.py
--rw-rw-rw-   0        0        0    24981 2023-07-04 09:40:58.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/emulation.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.921959 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/
--rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/__init__.py
--rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/fetch.py
--rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.924958 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/
--rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/__init__.py
--rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/input.py
--rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.927957 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/
--rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/log.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.930956 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/__init__.py
--rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/network.py
--rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.933955 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/overlay.py
--rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.936954 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/
--rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/__init__.py
--rw-rw-rw-   0        0        0    32632 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/page.py
--rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.939953 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/
--rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/__init__.py
--rw-rw-rw-   0        0        0    33744 2023-05-27 18:14:28.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/runtime.py
--rw-rw-rw-   0        0        0     8104 2023-05-26 16:33:22.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.942952 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/
--rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/system_info.py
--rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/types.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.945951 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/
--rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/__init__.py
--rw-rw-rw-   0        0        0    16832 2023-07-25 17:35:03.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/target.py
--rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/types.py
--rw-rw-rw-   0        0        0     4207 2023-07-28 15:07:56.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     9483 2023-07-03 05:36:05.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/extend_connection.py
--rw-rw-rw-   0        0        0    12324 2023-07-09 14:14:30.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/js.py
--rw-rw-rw-   0        0        0     7136 2023-07-28 15:10:54.000000 aio_dt_protocol-1.2.0/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:21:24.899967 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     8069 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2526 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 18:21:24.000000 aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 18:21:24.946950 aio_dt_protocol-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1565 2023-07-28 15:29:36.000000 aio_dt_protocol-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.337230 aio_dt_protocol-1.2.1/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     8069 2023-07-29 13:50:59.337230 aio_dt_protocol-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7302 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.236888 aio_dt_protocol-1.2.1/aio_dt_protocol/
+-rw-rw-rw-   0        0        0      503 2023-07-29 10:10:46.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/__init__.py
+-rw-rw-rw-   0        0        0    10780 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/actions.py
+-rw-rw-rw-   0        0        0    56632 2023-07-29 11:32:07.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/browser.py
+-rw-rw-rw-   0        0        0    17231 2023-07-28 18:01:34.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/connection.py
+-rw-rw-rw-   0        0        0    25910 2023-07-29 08:32:32.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/data.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.243957 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.246384 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/background_service/
+-rw-rw-rw-   0        0        0      107 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/background_service/__init__.py
+-rw-rw-rw-   0        0        0     3279 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/background_service/background_service.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/background_service/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.249879 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/browser/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/browser/__init__.py
+-rw-rw-rw-   0        0        0    13585 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/browser/browser.py
+-rw-rw-rw-   0        0        0     1346 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/browser/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.252375 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/css/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/css/__init__.py
+-rw-rw-rw-   0        0        0     6353 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/css/css.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/css/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.255370 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/device_orientation/
+-rw-rw-rw-   0        0        0       51 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/device_orientation/__init__.py
+-rw-rw-rw-   0        0        0     1455 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/device_orientation/device_orientation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/device_orientation/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.271318 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/
+-rw-rw-rw-   0        0        0       80 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/__init__.py
+-rw-rw-rw-   0        0        0    16508 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/dom.py
+-rw-rw-rw-   0        0        0    35568 2023-05-24 16:56:17.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/dom_element.py
+-rw-rw-rw-   0        0        0      798 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.274812 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/emulation/
+-rw-rw-rw-   0        0        0       73 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/emulation/__init__.py
+-rw-rw-rw-   0        0        0    24981 2023-07-04 09:40:58.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/emulation/emulation.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/emulation/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.277308 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/fetch/
+-rw-rw-rw-   0        0        0       57 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/fetch/__init__.py
+-rw-rw-rw-   0        0        0    17264 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/fetch/fetch.py
+-rw-rw-rw-   0        0        0     5210 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/fetch/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.280302 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/input/
+-rw-rw-rw-   0        0        0       26 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/input/__init__.py
+-rw-rw-rw-   0        0        0    23645 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/input/input.py
+-rw-rw-rw-   0        0        0     2778 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/input/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.283298 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/log/
+-rw-rw-rw-   0        0        0       49 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/log/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/log/log.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/log/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.320757 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/network/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/network/__init__.py
+-rw-rw-rw-   0        0        0    18941 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/network/network.py
+-rw-rw-rw-   0        0        0     3522 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/network/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.324251 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/overlay/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/overlay/__init__.py
+-rw-rw-rw-   0        0        0     1731 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/overlay/overlay.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/overlay/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.327246 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/page/
+-rw-rw-rw-   0        0        0       53 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/page/__init__.py
+-rw-rw-rw-   0        0        0    32632 2023-07-28 17:32:46.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/page/page.py
+-rw-rw-rw-   0        0        0     3104 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/page/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.330241 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/runtime/
+-rw-rw-rw-   0        0        0       65 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/runtime/__init__.py
+-rw-rw-rw-   0        0        0    33744 2023-05-27 18:14:28.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/runtime/runtime.py
+-rw-rw-rw-   0        0        0     8104 2023-05-26 16:33:22.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/runtime/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.333236 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/system_info/
+-rw-rw-rw-   0        0        0       37 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/system_info/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/system_info/system_info.py
+-rw-rw-rw-   0        0        0      784 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/system_info/types.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.336731 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/target/
+-rw-rw-rw-   0        0        0       61 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/target/__init__.py
+-rw-rw-rw-   0        0        0    16832 2023-07-25 17:35:03.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/target/target.py
+-rw-rw-rw-   0        0        0      408 2023-05-24 15:34:41.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/domains/target/types.py
+-rw-rw-rw-   0        0        0     4207 2023-07-28 15:07:56.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     9483 2023-07-03 05:36:05.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/extend_connection.py
+-rw-rw-rw-   0        0        0    12324 2023-07-09 14:14:30.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/js.py
+-rw-rw-rw-   0        0        0     7454 2023-07-29 12:25:48.000000 aio_dt_protocol-1.2.1/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 13:50:59.242379 aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     8069 2023-07-29 13:50:59.000000 aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2526 2023-07-29 13:50:59.000000 aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 13:50:59.000000 aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-29 13:50:59.000000 aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-29 13:50:59.000000 aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 13:50:59.338229 aio_dt_protocol-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-07-28 15:29:36.000000 aio_dt_protocol-1.2.1/setup.py
```

### Comparing `aio_dt_protocol-1.2.0/LICENSE` & `aio_dt_protocol-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/PKG-INFO` & `aio_dt_protocol-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio_dt_protocol
-Version: 1.2.0
+Version: 1.2.1
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-1.2.0/README.md` & `aio_dt_protocol-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/actions.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/actions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/browser.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/browser.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,24 @@
     import ujson as json
     HAS_UJSON = True
 except ModuleNotFoundError:
     HAS_UJSON = False
     import json
 import warnings
 import re, os, sys, signal, subprocess
-from urllib.parse import quote
 from os.path import expanduser
 from inspect import iscoroutinefunction
 from typing import List, Dict, Union, Optional, Tuple, Literal
 from collections.abc import Sequence
 from enum import Enum
 from .connection import Connection
-from .data import TargetConnectionInfo, TargetConnectionType, CommonCallback
+from .data import TargetConnectionInfo, TargetConnectionType, CommonCallback, BrowserInstanceInfo
 from .exceptions import FlagArgumentContainError, NoTargetWithGivenIdFound
 from .utils import (
-    get_request,
+    make_request,
     find_browser_executable_path,
     log,
     async_util_call,
     find_instances,
     prepare_url
 )
 
@@ -35,48 +34,42 @@
             cls,
             debug_port: int = 9222,
             browser_name: str = "chrome",
             callback: CommonCallback = None,
             **options
     ) -> Tuple["Browser", "Connection"]:
         if browser_instances := find_instances(debug_port, browser_name):
-            browser = Browser(debug_port=debug_port, browser_pid=browser_instances[debug_port])
-            running_state = "CONNECT TO EXISTING BROWSER"
+            browser = Browser(instance_info=browser_instances[debug_port])
         else:
             browser = Browser(
                 debug_port=debug_port,
                 browser_exe=browser_name,
                 **options
             )
-            running_state = "CREATE NEW BROWSER"
-
-        if options.get("verbose"):
-            log(running_state)
 
         return browser, await browser.waitFirstTab(callback=callback)
 
 
     def __init__(
-            self,
+            self, *,
             profile_path: str = "testProfile",
             dev_tool_profiles:  bool = False,
             url: Optional[Union[str, bytes]] = None,
             flags:  Optional["FlagBuilder"] = None,
             browser_path: str = "",
             debug_port:   Union[str, int] = 9222,
-            browser_pid:  int = 0,
             app:         bool = False,
             browser_exe:  str = "chrome",
             proxy_address:str = "http://127.0.0.1",
             proxy_port:   Union[str, int] = "",
             verbose:     bool = False,
             position: Optional[Tuple[int, int]] = None,
             sizes:    Optional[Tuple[int, int]] = None,
             prevent_restore: bool = False,
-
+            instance_info: Optional[BrowserInstanceInfo] = None
     ) -> None:
         """
         Все параметры — не обязательны.
         ==============================================================================================
 
         :param profile_path:    Путь до каталога, в который будет сохранена сессия профиля.
                                     Если не передан, или указано название папки, браузер
@@ -104,20 +97,14 @@
                                     https://peter.sh/experiments/chromium-command-line-switches/
 
         :param browser_path:    Путь до исполняемого файла браузера. Имеет приоритет над
                                     аргументом `browser_exe`.
 
         :param debug_port:      Используется порт по умолчанию 9222.
 
-        :param browser_pid:     ProcessID браузера. Используется методом kill(). Если
-                                    передано значение большее нуля, считается, что производится
-                                    подключение к уже существующему экземпляру браузера. Чтобы
-                                    найти запущенный браузер в режиме отладки, воспользуйтесь
-                                    `find_instances()`.
-
         :param app:             Запускает браузер в окне без пользовательского интерфейса,
                                     вроде адресной строки, кнопок навигации и прочих атрибутов.
                                     Распространяется только на первую страницу браузера. Прочие
                                     страницы будут открываться в обычном виде и в отдельном
                                     от первого окне.
 
         :param browser_exe:     Имя исполняемого файла браузера, который будет автоматизирован.
@@ -131,15 +118,19 @@
         :param verbose:         Печатать некие подробности процесса?
 
         :param position:        Кортеж с иксом и игреком, в которых откроется окно браузера.
 
         :param sizes:           Кортеж с длиной и шириной в которые будет установлено окно браузера.
 
         :param prevent_restore: Предотвращать восстановление предыдущей сессии после крашей.
+
+        :param instance_info:   Если передано, считается, что браузер уже был запущен и мы к
+                                    нему подключились.
         """
+
         if sys.platform not in ("win32", "linux"): raise OSError(f"Platform '{sys.platform}' — not supported")
         self.dev_tool_profiles = dev_tool_profiles if profile_path else False
 
         if verbose and not HAS_UJSON:
             log("Call 'python -m pip install ujson' for install", lvl="[- UJSON IS NOT INSTALLED -]")
 
         if self.dev_tool_profiles:
@@ -173,65 +164,81 @@
                 # ? Только для чтения
                 # os.chmod(preferences_path, READ_ONLY)
                 if verbose: log("Файл настроек — изменён и сохранён")
             else:
                 # os.chmod(preferences_path, READ_WRITE)
                 if verbose: log("Файл настроек — только для чтения")
 
-        if browser_exe == "chrome":
+        if "chrome" in browser_exe:
             self.browser_name = "chrome"
             browser_exe = "chrome" if sys.platform == "win32" else "google-chrome"
-        elif browser_exe == "brave":
+        elif "brave" in browser_exe:
             self.browser_name = "brave"
             browser_exe = "brave" if sys.platform == "win32" else "brave-browser"
-        elif browser_exe == "chromium":
+        elif "chromium" in browser_exe:
             self.browser_name = "chrome"
             browser_exe = "chromium" if sys.platform == "win32" else "chromium-browser"
         elif "edge" in browser_exe:
             self.browser_name = "edge"
             browser_exe = "msedge" if sys.platform == "win32" else "microsoft-edge"
+        else:
+            self.browser_name = browser_exe
 
         # ? Константы URL соответствующих вкладок
         self.NEW_TAB:       str = self.browser_name + "://newtab/"          # дефолтная вкладка
         self.SETTINGS:      str = self.browser_name + "://settings/"        # настройки
         self.BRAVE_REWARDS: str = self.browser_name + "://rewards/"         # вознаграждения (brave only)
         self.HISTORY:       str = self.browser_name + "://history/"         # история переходов
         self.BOOKMARKS:     str = self.browser_name + "://bookmarks/"       # закладки
         self.DOWNLOADS:     str = self.browser_name + "://downloads/"       # загрузки
         self.WALLET:        str = self.browser_name + "://wallet/"          # кошельки (brave only)
         self.EXTENSIONS:    str = self.browser_name + "://extensions/"      # расширения
         self.FLAGS:         str = self.browser_name + "://flags/"           # экспериментальные технологии
 
+        self.proxy_addres = proxy_address
+        self.proxy_port = str(proxy_port)
+        self.verbose = verbose
+
+        if instance_info:
+            self.is_headless_mode = instance_info.headless
+            self.browser_pid = instance_info.pid
+            self.debug_port = str(instance_info.port)
+            if verbose:
+                log(f"Connected to {self.debug_port} port | Headless mod: {self.is_headless_mode}")
+            return
+
         if sys.platform == "win32":
             browser_path = browser_path if browser_path else find_browser_executable_path(browser_exe)
         else:   #  ! sys.platform == "linux"
             browser_path = browser_path if browser_path else os.popen("which " + browser_exe).read().strip()
 
         if not os.path.exists(browser_path) or not os.path.isfile(browser_path):
             raise FileNotFoundError(f"Переданный 'browser_path' => '{browser_path}' — не существует, или содержит ошибку")
         self.browser_path = browser_path
 
         if int(debug_port) <= 0:
             raise ValueError(f"Значение 'debug_port' => '{debug_port}' — должно быть положительным целым числом!")
         self.debug_port = str(debug_port)
-        self.proxy_addres = proxy_address
-        self.proxy_port = str(proxy_port)
-        self.verbose = verbose
 
         # https://stackoverflow.com/questions/2381241/what-is-the-subprocess-popen-max-length-of-the-args-parameter
-        # data_url_len_is_high = len(url[0]) > 32_767
         data_url_len = len(url) if url else 0
-        # print("url =", url)
+
         if data_url_len > 30_000:
             warnings.warn(f"Length data url ({data_url_len}) is approaching to critical length = 32767 symbols!")
 
+        self.is_headless_mode = self.profile_path == ""
+        if self.is_headless_mode:
+            app = False
+            if url is None:
+                url = ""
         url = prepare_url(url, self.browser_name, app)
 
-        self.is_headless_mode = False
-        self.browser_pid = browser_pid if browser_pid > 0 else self._run_browser(url, flags, position, sizes)
+        self.browser_pid = self._run_browser(url, flags, position, sizes)
+        if verbose:
+            log(f"Running at {self.debug_port} port | Headless mod: {self.is_headless_mode}")
 
     def _run_browser(self, url: Optional[str] = None,
                      flags: Optional["FlagBuilder"] = None,
                      position: Optional[Tuple[int, int]] = None,
                      sizes: Optional[Tuple[int, int]] = None) -> int:
         """
         Запускает браузер с переданными флагами.
@@ -267,15 +274,14 @@
                 flag_box.add(CMDFlags.Screen.window_position, *position)
             if sizes is not None:
                 flag_box.add(CMDFlags.Screen.window_size, *sizes)
 
         # ! Headless mode
         else:
             flag_box.add(CMDFlags.Headless.headless)
-            self.is_headless_mode = True
 
         if self.proxy_port:
             flag_box.add(CMDFlags.Other.proxy_server, self.proxy_addres + ":" + self.proxy_port)
             if self.verbose:
                 log(f"Run browser {self.browser_name!r} on port: {self.debug_port} with proxy " +
                       f"on http://127.0.0.1:{self.proxy_port}")
         else:
@@ -324,31 +330,40 @@
                     "title": "Yahoo",
                     "type": "page",
                     "url": "https://www.yahoo.com/",
                     "webSocketDebuggerUrl": "ws://localhost:9222/devtools/page/DAB7FB6187B554E10B0BD18821265734"
                 }, { ... } ]
         """
         result = await async_util_call(
-            get_request, f"http://127.0.0.1:{self.debug_port}/json/list")
+            make_request, f"http://127.0.0.1:{self.debug_port}/json/list")
 
         if self.verbose: log("getPageList() => " + result)
         return json.loads(result)
 
+    async def queryNewTab(self, url: str = "about:blank") -> Connection:
+        result: str = await async_util_call(
+            make_request, f"http://127.0.0.1:{self.debug_port}/json/new?{url}", "PUT")
+
+        if self.verbose: log("queryNewTab() => " + result)
+        result: dict = json.loads(result)
+        return await self.getConnectionByID(result["id"])
+
+
     async def getConnectionBy(
             self, key: Union[str, int],
             value: Union[str, int],
             match_mode: Literal["exact", "contains", "startswith"] = "exact",
             index: int = 0,
             callback: CommonCallback = None) -> Optional[Connection]:
         """
         Организует выбор нужного соединения из процессов браузера по следующим критериям:
         :param key:                 По ключу из словаря. Список ключей смотри
                                         в возвращаемых значениях GetPageList()
         :param value:               Значение ключа, которому должен соответствовать выбор
-        :param match_mode:          Значение ключа:
+        :param match_mode:          Соответствие ключа:
                                         "exact"      - полностью совпадает с value,
                                         "contains"   - содержит value,
                                         "startswith" - начинается с value
         :param index:               Поскольку открытых страниц с одинаковым ключом может
                                         быть несколько, предоставляется возможность выбрать
                                         по индексу. По умолчанию = 0
         :param callback:            Корутина, которой будет передаваться контекст абсолютно
@@ -360,25 +375,25 @@
         """
 
         if callback is not None and not iscoroutinefunction(callback):
             raise TypeError("Argument 'callback' must be a coroutine")
 
         counter = 0; v = value.lower()
         for page_data in await self.getConnectionList():
-            data = page_data[key]
+            data: str = page_data[key].lower()
             if ((match_mode == "exact" and data == v)
                 or (match_mode == "contains" and data.find(v) > -1 )
-                    or (match_mode == "startswith" and data.find(v) == 0)):
+                    or (match_mode == "startswith" and data.startswith(v))):
                 if counter == index:
                     conn = Connection(
                         page_data["webSocketDebuggerUrl"],
                         page_data["id"],
                         page_data["devtoolsFrontendUrl"],
                         callback,
-                        self.profile_path == "",
+                        self.is_headless_mode,
                         self.verbose,
                         self.browser_name
                     )
 
                     await conn.activate()
                     return conn
                 counter += 1
@@ -529,15 +544,15 @@
                     target_info.targetId, callback=callback))
         return connections
 
     async def waitFirstTab(
             self, timeout: float = 20.0,
             callback: CommonCallback = None) -> Connection:
         """ Дожидается получения соединения или вызывает исключение
-        'asyncio.exceptions.TimeoutError' по истечении таймаута.
+        'TimeoutError' по истечении таймаута.
         """
         return await asyncio.wait_for(self.getFirstTab(callback), timeout)
 
     async def getFirstTab(self, callback: CommonCallback = None) -> Connection:
         """
         Безусловно дожидается соединения со страницей.
         """
```

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/connection.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/connection.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/data.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 from asyncio import Queue
 
 CommonCallback = Optional[Callable[[dict], Coroutine[None, None, None]]]
 T = TypeVar("T")
 
 
 @dataclass
+class BrowserInstanceInfo:
+    name: str
+    pid: int
+    port: int
+    headless: bool
+
+
+@dataclass
 class GeoInfo:
     ip: str
     timezone: str
     geo: dict[str, float]
     country: str
     languages: list[str]
     city: str
```

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/background_service/background_service.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/background_service/background_service.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/browser.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/browser/browser.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/browser/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/browser/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/css/css.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/css/css.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/device_orientation/device_orientation.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/device_orientation/device_orientation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/dom.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/dom_element.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/dom_element.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/dom/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/dom/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/emulation/emulation.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/emulation/emulation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/fetch.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/fetch/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/fetch/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/input.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/input/input.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/input/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/input/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/log/log.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/log/log.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/network.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/network/network.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/network/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/network/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/overlay/overlay.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/overlay/overlay.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/page.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/page/page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/page/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/page/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/runtime.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/runtime/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/runtime/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/system_info.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/system_info/system_info.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/system_info/types.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/system_info/types.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/domains/target/target.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/domains/target/target.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/extend_connection.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/extend_connection.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/js.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/js.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol/utils.py` & `aio_dt_protocol-1.2.1/aio_dt_protocol/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import subprocess
 import re
 import sys
 import urllib.request
 from pathlib import Path
 from typing import Optional, Dict, Callable, Union
 from urllib.parse import quote
+from .data import BrowserInstanceInfo
 
 
-def get_request(url: str) -> str:
-    with urllib.request.urlopen(url) as response:
-        return response.read().decode('utf-8')
+def make_request(url: str, method="GET") -> str:
+    req = urllib.request.Request(url, method=method)
+    with urllib.request.urlopen(req) as response:
+        return response.read().decode("utf-8")
 
 
 def find_browser_executable_path(exe="chrome") -> str:
     """ Возвращает путь до EXE. """
     if not sys.platform == "win32":
         raise OSError("find_browser_executable_path() is only available on Windows")
 
@@ -60,67 +62,80 @@
     )
     """
     return await asyncio.get_running_loop().run_in_executor(
         None, function, *args
     )
 
 
-def find_instances(for_port: Optional[int] = None, browser: str = "chrome") -> Dict[int, int]:
+def find_instances(for_port: Optional[int] = None, browser: str = "chrome") -> Dict[int, BrowserInstanceInfo]:
     """ !!! ВНИМАНИЕ !!! На Windows 11 может быть отключен компонент WMI("Windows Management
     Instrumentation"), его нужно либо включить в разделе “Программы и компоненты” панели
     управления, либо установить из официальных источников.
 
     Используется для обнаружения уже запущенных браузеров в режиме отладки.
     Например:
             if browser_instances := find_instances():
-                port, pid = [(k, v) for k, v in browser_instances.items()][0]
-                browser_instance = Browser(debug_port=port, chrome_pid=pid)
+                port, instance_info = [(k, v) for k, v in browser_instances.items()][0]
+                browser_instance = Browser(instance_info=instance_info)
             else:
                 browser_instance = Browser()
 
             # Или для конкретного, известного порта:
             if browser_instances := find_instances(port):
-                pid = browser_instances[port]
-                browser_instance = Browser(debug_port=port, chrome_pid=pid)
+                instance_info = browser_instances[port]
+                browser_instance = Browser(instance_info=instance_info)
             else:
                 browser_instance = Browser()
     :param for_port:    - порт, для которого осуществляется поиск.
     :param browser:     - браузер, для которого запрашивается поиск.
-    :return:            - словарь, ключами которого являются используемые порты запущенных
-                            браузеров, а значениями, их ProcessID, или пустой словарь,
-                            если ничего не найдено.
-                            { 9222: 16017, 9223: 2001, ... }
+    :return:
     """
+    win_exp = re.compile(r"^\"[^\"]+(?<=\\)(\w+\.\w+)\".*?--remote-debugging-port=(\d+).*?(\d+)\s*$")
+    linux_exp = re.compile(r"^[/\w]+/(\w+).*?--remote-debugging-port=(\d+)")
+
     result = {}
     if sys.platform == "win32":
         if "chrom" in browser: browser = "chrome.exe"
         elif "brave" in browser: browser = "brave.exe"
         elif "edge" in browser: browser = "msedge.exe"
         # else: ValueError("Not support browser: " + browser)
         cmd = f"WMIC PROCESS WHERE NAME='{browser}' GET Commandline,Processid"
         for line in subprocess.Popen(cmd, stdout=subprocess.PIPE).stdout:
             if b"--type=renderer" not in line and b"--remote-debugging-port=" in line:
-                port, pid = re.findall(r"--remote-debugging-port=(\d+).*?(\d+)\s*$", line.decode())[0]
-                port, pid = int(port), int(pid)
-                if for_port == port: return {port: pid}
-                result[port] = pid
+                name, port, pid = win_exp.findall(line.decode())[0]
+                inst = BrowserInstanceInfo(
+                    name=name,
+                    port=(port := int(port)),
+                    pid=int(pid),
+                    headless=b"--headless" in line
+                )
+                if for_port == port:
+                    return {port: inst}
+                result[port] = inst
 
     elif sys.platform == "linux":
         if "chrom" in browser: browser = "chrome"
         elif "brave" in browser: browser = "brave"
         elif "edge" in browser: browser = "msedge"
         # else: ValueError("Not support browser: " + browser)
         try: itr = map(int, subprocess.check_output(["pidof", browser]).split())
         except subprocess.CalledProcessError: itr = []
         for pid in itr:
             with open("/proc/" + str(pid) + "/cmdline") as f: cmd_line =  f.read()[:-1]
             if "--type=renderer" not in cmd_line and "--remote-debugging-port=" in cmd_line:
-                port = int(re.findall(r"--remote-debugging-port=(\d+)", cmd_line)[0])
-                if for_port == port: return {port: pid}
-                result[port] = pid
+                name, port = linux_exp.findall(cmd_line)[0]
+                inst = BrowserInstanceInfo(
+                    name=name,
+                    port=(port := int(port)),
+                    pid=pid,
+                    headless="--headless" in cmd_line
+                )
+                if for_port == port:
+                    return {port: inst}
+                result[port] = inst
     else:
         raise OSError(f"Platform '{sys.platform}' — not supported")
     return {} if for_port else result
 
 
 def prepare_url(url: Union[str, bytes, None], browser_name: str, app: bool = False) -> Optional[str]:
     """ Подготавливает строку для передачи в navigate(), или в конструкторе Browser."""
```

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-dt-protocol
-Version: 1.2.0
+Version: 1.2.1
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-1.2.0/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-1.2.1/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-1.2.0/setup.py` & `aio_dt_protocol-1.2.1/setup.py`

 * *Files identical despite different names*

