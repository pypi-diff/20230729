# Comparing `tmp/tendril-utils-types-0.2.1.tar.gz` & `tmp/tendril-utils-types-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-utils-types-0.2.1.tar", last modified: Wed Jul 31 20:10:02 2019, max compression
+gzip compressed data, was "tendril-utils-types-0.2.2.tar", last modified: Sat Jul 29 09:43:06 2023, max compression
```

## Comparing `tendril-utils-types-0.2.1.tar` & `tendril-utils-types-0.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2019-07-31 19:40:20.000000 tendril-utils-types-0.2.1/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       46 2019-07-30 10:57:03.000000 tendril-utils-types-0.2.1/.coveralls.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3810 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2095 2019-07-30 10:54:24.000000 tendril-utils-types-0.2.1/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2019-07-30 10:56:54.000000 tendril-utils-types-0.2.1/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      831 2019-07-31 06:10:34.000000 tendril-utils-types-0.2.1/tox.ini
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2106 2018-09-11 04:42:38.000000 tendril-utils-types-0.2.1/.gitignore
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      851 2018-09-07 15:49:44.000000 tendril-utils-types-0.2.1/src/tendril/utils/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3502 2018-09-12 00:09:04.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/electromagnetic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8689 2018-09-12 00:09:04.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/signalbase.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1069 2018-09-27 10:26:41.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/mass.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2742 2018-09-11 23:53:32.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/lengths.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7725 2019-04-17 22:06:24.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/time.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2804 2018-09-11 23:53:32.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/cartesian.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5027 2019-07-31 06:31:07.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    19190 2019-07-31 07:50:18.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/unitbase.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    16522 2019-04-18 21:41:17.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/currency.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1524 2018-09-11 23:53:32.000000 tendril-utils-types-0.2.1/src/tendril/utils/types/thermodynamic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      851 2018-09-07 15:49:44.000000 tendril-utils-types-0.2.1/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1055 2019-07-31 17:21:14.000000 tendril-utils-types-0.2.1/src/tendril/config/types.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2019-04-01 11:34:55.000000 tendril-utils-types-0.2.1/src/tendril/config/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3810 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      559 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1692 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/SOURCES.txt
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3276 2019-07-31 18:03:05.000000 tendril-utils-types-0.2.1/setup.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2019-07-30 11:18:27.000000 tendril-utils-types-0.2.1/MANIFEST.in
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2019-07-31 19:18:18.000000 tendril-utils-types-0.2.1/docs/conf.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2019-07-31 18:51:10.000000 tendril-utils-types-0.2.1/docs/api/tendril.config.types.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      172 2015-09-24 00:45:21.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.lengths.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      196 2015-09-24 00:45:21.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.electromagnetic.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2019-07-31 18:50:25.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.currency.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      178 2015-09-24 00:45:21.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.cartesian.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      181 2015-09-24 00:45:21.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.signalbase.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2015-09-24 00:45:21.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.thermodynamic.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2015-08-11 20:26:37.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.unitbase.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      669 2019-07-31 18:51:10.000000 tendril-utils-types-0.2.1/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2015-09-24 00:45:21.000000 tendril-utils-types-0.2.1/docs/api/tendril.utils.types.time.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2015-08-23 17:49:15.000000 tendril-utils-types-0.2.1/docs/_static/logo_packed.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2019-07-31 07:34:28.000000 tendril-utils-types-0.2.1/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2019-07-31 06:52:53.000000 tendril-utils-types-0.2.1/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2015-08-23 17:49:15.000000 tendril-utils-types-0.2.1/docs/_static/logo.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2019-07-30 10:54:54.000000 tendril-utils-types-0.2.1/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2019-07-30 11:12:55.000000 tendril-utils-types-0.2.1/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2019-07-30 11:12:55.000000 tendril-utils-types-0.2.1/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1078 2019-07-31 06:33:10.000000 tendril-utils-types-0.2.1/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2019-07-30 10:54:54.000000 tendril-utils-types-0.2.1/docs/Makefile
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1849 2019-07-30 11:14:42.000000 tendril-utils-types-0.2.1/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2019-07-31 20:10:02.000000 tendril-utils-types-0.2.1/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2305 2015-10-02 03:18:37.000000 tendril-utils-types-0.2.1/tests/test_utils_types_thermodynamic.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4316 2019-07-31 06:19:04.000000 tendril-utils-types-0.2.1/tests/test_utils_types_currency.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4187 2015-11-07 16:26:53.000000 tendril-utils-types-0.2.1/tests/test_utils_types_time.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2019-07-30 10:55:00.000000 tendril-utils-types-0.2.1/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2562 2015-10-02 02:49:09.000000 tendril-utils-types-0.2.1/tests/test_utils_types_cartesian.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2019-07-30 10:55:00.000000 tendril-utils-types-0.2.1/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5797 2015-11-07 16:26:53.000000 tendril-utils-types-0.2.1/tests/test_utils_types_unitbase.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2017-05-03 06:19:27.000000 tendril-utils-types-0.2.1/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2019-07-30 10:47:23.000000 tendril-utils-types-0.2.1/CHANGELOG.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2120 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3555 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2256 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.291084 tendril-utils-types-0.2.2/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.291084 tendril-utils-types-0.2.2/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.291084 tendril-utils-types-0.2.2/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.291084 tendril-utils-types-0.2.2/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      669 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.config.types.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      178 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.cartesian.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.currency.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      196 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.electromagnetic.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      172 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.lengths.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      181 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.signalbase.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.thermodynamic.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.time.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      177 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/api/tendril.utils.types.unitbase.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1078 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1672 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.291084 tendril-utils-types-0.2.2/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3293 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.287084 tendril-utils-types-0.2.2/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.291084 tendril-utils-types-0.2.2/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:08:45.000000 tendril-utils-types-0.2.2/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1055 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/config/types.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:09:00.000000 tendril-utils-types-0.2.2/src/tendril/utils/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/src/tendril/utils/types/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5027 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2804 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/cartesian.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    16522 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/currency.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3502 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/electromagnetic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2742 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/lengths.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1069 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/mass.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      283 2023-07-29 07:46:30.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/memory.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8689 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/signalbase.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1524 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/thermodynamic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7725 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/time.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    19190 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/src/tendril/utils/types/unitbase.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3555 2023-07-29 09:43:06.000000 tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1711 2023-07-29 09:43:06.000000 tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-29 09:43:06.000000 tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      615 2023-07-29 09:43:06.000000 tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-29 09:43:06.000000 tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 09:43:06.295084 tendril-utils-types-0.2.2/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2562 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tests/test_utils_types_cartesian.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4316 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tests/test_utils_types_currency.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2305 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tests/test_utils_types_thermodynamic.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4187 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tests/test_utils_types_time.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5797 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tests/test_utils_types_unitbase.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      831 2020-08-18 06:57:09.000000 tendril-utils-types-0.2.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tendril-utils-types-0.2.1/.readthedocs.yml` & `tendril-utils-types-0.2.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/PKG-INFO` & `tendril-utils-types-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-utils-types
-Version: 0.2.1
+Version: 0.2.2
 Summary: Type classes for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-types
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
-Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-types
-Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-types/issues
 Project-URL: Documentation, https://tendril-utils-types.readthedocs.io/en/latest
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-utils-types.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-types
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-utils-types.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-types
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-types.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-utils-types
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-types.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-utils-types
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-types.svg
-            :target: https://requires.io/github/tendril-framework/tendril-utils-types/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-utils-types.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-utils-types.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-utils-types>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-utils-types`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-utils-types`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
+Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-types/issues
+Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-types
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -76,9 +23,65 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
-Provides-Extra: dev
 Provides-Extra: publish
+Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-utils-types.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-types
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-utils-types.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-types
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-types.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-utils-types
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-types.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-utils-types
+
+.. image:: https://img.shields.io/codacy/grade/eb5c1b09e6454c57910f370a6b4536c4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-utils-types
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-types.svg
+    :target: https://requires.io/github/tendril-framework/tendril-utils-types/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-utils-types.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-utils-types.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-utils-types>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-utils-types`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-utils-types`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-utils-types-0.2.1/README.rst` & `tendril-utils-types-0.2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 .. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-types.svg?logo=travis
     :target: https://travis-ci.org/tendril-framework/tendril-utils-types
 
 .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-types.svg?logo=coveralls
     :target: https://coveralls.io/github/tendril-framework/tendril-utils-types
 
+.. image:: https://img.shields.io/codacy/grade/eb5c1b09e6454c57910f370a6b4536c4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-utils-types
+
 .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-types.svg
     :target: https://requires.io/github/tendril-framework/tendril-utils-types/requirements
 
 .. image:: https://img.shields.io/pypi/l/tendril-utils-types.svg
     :target: https://www.gnu.org/licenses/agpl-3.0.en.html
```

### Comparing `tendril-utils-types-0.2.1/.travis.yml` & `tendril-utils-types-0.2.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/tox.ini` & `tendril-utils-types-0.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/.gitignore` & `tendril-utils-types-0.2.2/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -136,8 +136,8 @@
 atlassian-ide-plugin.xml
 
 # Crashlytics plugin (for Android Studio and IntelliJ)
 com_crashlytics_export_strings.xml
 crashlytics.properties
 crashlytics-build.properties
 fabric.properties
-
+.coveralls.yml
```

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/__init__.py` & `tendril-utils-types-0.2.2/src/tendril/config/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
-# Copyright (C) 2018 Chintalagiri Shashank
+# Copyright (C) 2019 Chintalagiri Shashank
 #
 # This file is part of tendril.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,7 +16,15 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
+
+from tendril.utils.config import ConfigManager
+_manager = ConfigManager(prefix='tendril.config',
+                         legacy='tendril.config.legacy',
+                         excluded=['tendril.config.legacy'])
+
+import sys
+sys.modules[__name__] = _manager
```

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/electromagnetic.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/electromagnetic.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/signalbase.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/signalbase.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/mass.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/mass.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/lengths.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/lengths.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/time.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/time.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/cartesian.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/cartesian.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/__init__.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/unitbase.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/unitbase.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/currency.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/currency.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/utils/types/thermodynamic.py` & `tendril-utils-types-0.2.2/src/tendril/utils/types/thermodynamic.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril/config/types.py` & `tendril-utils-types-0.2.2/src/tendril/config/types.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/PKG-INFO` & `tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-utils-types
-Version: 0.2.1
+Version: 0.2.2
 Summary: Type classes for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-types
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
-Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-types
-Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-types/issues
 Project-URL: Documentation, https://tendril-utils-types.readthedocs.io/en/latest
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-utils-types.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-types
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-utils-types.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-utils-types
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-types.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-utils-types
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-types.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-utils-types
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-types.svg
-            :target: https://requires.io/github/tendril-framework/tendril-utils-types/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-utils-types.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-utils-types.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-utils-types>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-utils-types`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-utils-types`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
+Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-types/issues
+Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-types
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -76,9 +23,65 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
-Provides-Extra: dev
 Provides-Extra: publish
+Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-utils-types.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-types
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-utils-types.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-utils-types
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-utils-types.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-utils-types
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-utils-types.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-utils-types
+
+.. image:: https://img.shields.io/codacy/grade/eb5c1b09e6454c57910f370a6b4536c4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-utils-types
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-utils-types.svg
+    :target: https://requires.io/github/tendril-framework/tendril-utils-types/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-utils-types.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-utils-types.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-utils-types>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-utils-types`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-utils-types`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/requires.txt` & `tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 [build]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
 pytest
+pytest-flake8
 pytest-cov
 coveralls[yaml]
 
 [dev]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
 pytest
+pytest-flake8
 pytest-cov
 coveralls[yaml]
 
 [docs]
 setuptools_scm
 sphinx
 sphinx-argparse
@@ -33,20 +35,22 @@
 
 [publish]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
 pytest
+pytest-flake8
 pytest-cov
 coveralls[yaml]
 twine
 pygithub
 
 [tests]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
 pytest
+pytest-flake8
 pytest-cov
 coveralls[yaml]
```

### Comparing `tendril-utils-types-0.2.1/src/tendril_utils_types.egg-info/SOURCES.txt` & `tendril-utils-types-0.2.2/src/tendril_utils_types.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.coveralls.yml
 .gitignore
 .readthedocs.yml
 .travis.yml
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
@@ -36,14 +35,15 @@
 src/tendril/utils/__init__.py
 src/tendril/utils/types/__init__.py
 src/tendril/utils/types/cartesian.py
 src/tendril/utils/types/currency.py
 src/tendril/utils/types/electromagnetic.py
 src/tendril/utils/types/lengths.py
 src/tendril/utils/types/mass.py
+src/tendril/utils/types/memory.py
 src/tendril/utils/types/signalbase.py
 src/tendril/utils/types/thermodynamic.py
 src/tendril/utils/types/time.py
 src/tendril/utils/types/unitbase.py
 src/tendril_utils_types.egg-info/PKG-INFO
 src/tendril_utils_types.egg-info/SOURCES.txt
 src/tendril_utils_types.egg-info/dependency_links.txt
```

### Comparing `tendril-utils-types-0.2.1/setup.py` & `tendril-utils-types-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
 
 doc_requires = setup_requires + ['sphinx', 'sphinx-argparse', 'alabaster']
 
-test_requires = doc_requires + ['pytest', 'pytest-cov', 'coveralls[yaml]']
+test_requires = doc_requires + ['pytest', 'pytest-flake8', 'pytest-cov', 'coveralls[yaml]']
 
 build_requires = test_requires  # + ['doit', 'pyinstaller']
 
 publish_requires = build_requires + ['twine', 'pygithub']
 
 setup(
     name='tendril-utils-types',
```

### Comparing `tendril-utils-types-0.2.1/docs/conf.py` & `tendril-utils-types-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/api/index.rst` & `tendril-utils-types-0.2.2/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/_static/logo_packed.png` & `tendril-utils-types-0.2.2/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/_static/custom.css` & `tendril-utils-types-0.2.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/_static/favicon.ico` & `tendril-utils-types-0.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/_static/logo.png` & `tendril-utils-types-0.2.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/_templates/about.html` & `tendril-utils-types-0.2.2/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/index.rst` & `tendril-utils-types-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/Makefile` & `tendril-utils-types-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/docs/installation.rst` & `tendril-utils-types-0.2.2/docs/installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ``tendril-utils-types`` can be installed normally from the Python Package Index.
 Note that you will need write access to your python packages folder. This
 means you will have to install as root or with sudo on most linux distributions,
 unless you are installing to a virtual environment you can write to.
 
 .. code-block:: console
 
-    $ sudo pip install tendril-utils-types
+    $ pip install tendril-utils-types
 
 
 Installation from Sources
 -------------------------
 
 The sources can be downloaded from the project's
 `github releases <https://github.com/tendril-framework/tendril-utils-types/releases>`_.
@@ -26,29 +26,24 @@
 You will have to ensure the following dependencies are installed and available
 in your python environment by whatever means you usually use.
 
     - six
     - cachecontrol[filecache]
     - arrow
     - num2words
-    - tendril-utils-core>=0.1.12
-    - tendril-config>=0.1.6
-    - tendril-utils-www>=0.1.5
+    - tendril-utils-core
+    - tendril-config
+    - tendril-utils-www
 
 ``sudo`` may be necessary if you are not installing into a virtual environment.
 
 
 .. code-block:: console
 
-    $ wget https://github.com/tendril-framework/tendril-utils-types/releases/v0.2.0.tar.gz
-    $ TODO untar
-    ...
-    $ TODO cd into folder
     $ python setup.py install
-    ...
 
 
 Installation for Development
 ----------------------------
 
 Installation from the repository is the most convenient installation method
 if you intend to modify the code, either for your own use or to contribute to
```

### Comparing `tendril-utils-types-0.2.1/tests/test_utils_types_thermodynamic.py` & `tendril-utils-types-0.2.2/tests/test_utils_types_thermodynamic.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/tests/test_utils_types_currency.py` & `tendril-utils-types-0.2.2/tests/test_utils_types_currency.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/tests/test_utils_types_time.py` & `tendril-utils-types-0.2.2/tests/test_utils_types_time.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/tests/test_utils_types_cartesian.py` & `tendril-utils-types-0.2.2/tests/test_utils_types_cartesian.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/tests/coveralls.py` & `tendril-utils-types-0.2.2/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/tests/test_utils_types_unitbase.py` & `tendril-utils-types-0.2.2/tests/test_utils_types_unitbase.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-types-0.2.1/LICENSE` & `tendril-utils-types-0.2.2/LICENSE`

 * *Files identical despite different names*

