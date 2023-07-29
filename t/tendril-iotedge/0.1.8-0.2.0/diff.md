# Comparing `tmp/tendril-iotedge-0.1.8.tar.gz` & `tmp/tendril-iotedge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-iotedge-0.1.8.tar", last modified: Tue Jul 25 11:05:49 2023, max compression
+gzip compressed data, was "tendril-iotedge-0.2.0.tar", last modified: Sat Jul 29 13:09:33 2023, max compression
```

## Comparing `tendril-iotedge-0.1.8.tar` & `tendril-iotedge-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.716405 tendril-iotedge-0.1.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-07-25 11:05:49.716405 tendril-iotedge-0.1.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.708405 tendril-iotedge-0.1.8/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.708405 tendril-iotedge-0.1.8/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-25 11:05:49.716405 tendril-iotedge-0.1.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-03-16 07:26:30.000000 tendril-iotedge-0.1.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.704405 tendril-iotedge-0.1.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1879 2023-07-25 05:05:32.000000 tendril-iotedge-0.1.8/src/tendril/apiserver/routers/iotcore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2267 2023-07-23 18:59:09.000000 tendril-iotedge-0.1.8/src/tendril/apiserver/routers/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/common/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril-iotedge-0.1.8/src/tendril/common/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril-iotedge-0.1.8/src/tendril/common/iotcore/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril-iotedge-0.1.8/src/tendril/common/iotcore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/common/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/common/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/common/iotedge/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      733 2023-04-12 18:16:23.000000 tendril-iotedge-0.1.8/src/tendril/common/iotedge/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril-iotedge-0.1.8/src/tendril/config/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4980 2023-07-25 09:15:17.000000 tendril-iotedge-0.1.8/src/tendril/db/models/deviceconfig.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril-iotedge-0.1.8/src/tendril/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril-iotedge-0.1.8/src/tendril/iotcore/settings.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2664 2023-04-12 18:53:32.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      422 2023-04-05 04:43:55.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/heartbeat.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril/iotedge/profiles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/profiles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      963 2023-04-05 18:20:26.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/profiles/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-04-08 07:11:19.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/profiles/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.8/src/tendril/iotedge/registration.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-07-25 11:05:49.000000 tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1575 2023-07-25 11:05:49.000000 tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-25 11:05:49.000000 tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-07-25 11:05:49.000000 tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-25 11:05:49.000000 tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 11:05:49.712406 tendril-iotedge-0.1.8/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.041798 tendril-iotedge-0.2.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-07-29 13:09:33.041798 tendril-iotedge-0.2.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.033798 tendril-iotedge-0.2.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-29 13:09:33.041798 tendril-iotedge-0.2.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-03-16 07:26:30.000000 tendril-iotedge-0.2.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.033798 tendril-iotedge-0.2.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1879 2023-07-25 05:05:32.000000 tendril-iotedge-0.2.0/src/tendril/apiserver/routers/iotcore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2267 2023-07-23 18:59:09.000000 tendril-iotedge-0.2.0/src/tendril/apiserver/routers/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/common/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-25 05:48:52.000000 tendril-iotedge-0.2.0/src/tendril/common/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      125 2023-07-25 05:51:28.000000 tendril-iotedge-0.2.0/src/tendril/common/iotcore/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril-iotedge-0.2.0/src/tendril/common/iotcore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/common/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/common/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/common/iotedge/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      733 2023-04-12 18:16:23.000000 tendril-iotedge-0.2.0/src/tendril/common/iotedge/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril-iotedge-0.2.0/src/tendril/config/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4980 2023-07-25 09:15:17.000000 tendril-iotedge-0.2.0/src/tendril/db/models/deviceconfig.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril-iotedge-0.2.0/src/tendril/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril-iotedge-0.2.0/src/tendril/iotcore/settings.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2664 2023-04-12 18:53:32.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      422 2023-04-05 04:43:55.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      627 2023-07-29 10:49:03.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/heartbeat.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.037798 tendril-iotedge-0.2.0/src/tendril/iotedge/profiles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/profiles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1166 2023-07-29 10:10:25.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/profiles/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-07-28 16:44:25.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/profiles/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-04-03 17:40:48.000000 tendril-iotedge-0.2.0/src/tendril/iotedge/registration.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.041798 tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-07-29 13:09:32.000000 tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1575 2023-07-29 13:09:33.000000 tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-29 13:09:32.000000 tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-07-29 13:09:32.000000 tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-29 13:09:32.000000 tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-29 13:09:33.041798 tendril-iotedge-0.2.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril-iotedge-0.2.0/tox.ini
```

### Comparing `tendril-iotedge-0.1.8/.gitignore` & `tendril-iotedge-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/.readthedocs.yml` & `tendril-iotedge-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/.travis.yml` & `tendril-iotedge-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/LICENSE` & `tendril-iotedge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/PKG-INFO` & `tendril-iotedge-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.1.8
+Version: 0.2.0
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril-iotedge-0.1.8/README.rst` & `tendril-iotedge-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/Makefile` & `tendril-iotedge-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/_static/custom.css` & `tendril-iotedge-0.2.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/_static/favicon.ico` & `tendril-iotedge-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/_static/logo.png` & `tendril-iotedge-0.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/_static/logo_packed.png` & `tendril-iotedge-0.2.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/_templates/about.html` & `tendril-iotedge-0.2.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/conf.py` & `tendril-iotedge-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/index.rst` & `tendril-iotedge-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/docs/installation.rst` & `tendril-iotedge-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/setup.py` & `tendril-iotedge-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/apiserver/routers/iotcore.py` & `tendril-iotedge-0.2.0/src/tendril/apiserver/routers/iotcore.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/apiserver/routers/iotedge.py` & `tendril-iotedge-0.2.0/src/tendril/apiserver/routers/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/common/iotedge/exceptions.py` & `tendril-iotedge-0.2.0/src/tendril/common/iotedge/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/common/iotedge/formats.py` & `tendril-iotedge-0.2.0/src/tendril/common/iotedge/formats.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/config/__init__.py` & `tendril-iotedge-0.2.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/config/iotedge.py` & `tendril-iotedge-0.2.0/src/tendril/config/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/db/models/deviceconfig.py` & `tendril-iotedge-0.2.0/src/tendril/db/models/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/iotcore/settings.py` & `tendril-iotedge-0.2.0/src/tendril/iotcore/settings.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/iotedge/announce.py` & `tendril-iotedge-0.2.0/src/tendril/iotedge/announce.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/iotedge/heartbeat.py` & `tendril-iotedge-0.2.0/src/tendril/iotedge/heartbeat.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 def mark_seen(func):
     @wraps(func)
     def inner(device=None, session=None, **kwargs):
         logger.debug(f"Mark device {device} as seen")
+        device.report_seen()
         return func(device=device, session=session, **kwargs)
     return inner
 
 
 @with_db
 @registered_device()
 @mark_seen
 def ping(device=None, appname=None, status=None, session=None):
     logger.info(f"Got ping from {device}")
+    device.report_status(status)
```

### Comparing `tendril-iotedge-0.1.8/src/tendril/iotedge/profiles/manager.py` & `tendril-iotedge-0.2.0/src/tendril/iotedge/profiles/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril/iotedge/registration.py` & `tendril-iotedge-0.2.0/src/tendril/iotedge/registration.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/PKG-INFO` & `tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.1.8
+Version: 0.2.0
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/SOURCES.txt` & `tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/src/tendril_iotedge.egg-info/requires.txt` & `tendril-iotedge-0.2.0/src/tendril_iotedge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/tests/coveralls.py` & `tendril-iotedge-0.2.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.8/tox.ini` & `tendril-iotedge-0.2.0/tox.ini`

 * *Files identical despite different names*

