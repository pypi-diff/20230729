# Comparing `tmp/pycodestyle-2.9.0.tar.gz` & `tmp/pycodestyle-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodestyle-2.9.0.tar", last modified: Sat Jul 30 19:32:55 2022, max compression
+gzip compressed data, was "pycodestyle-2.9.1.tar", last modified: Wed Aug  3 23:13:14 2022, max compression
```

## Comparing `pycodestyle-2.9.0.tar` & `pycodestyle-2.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-07-30 19:32:55.215552 pycodestyle-2.9.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)    26571 2022-07-30 19:31:57.000000 pycodestyle-2.9.0/CHANGES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3109 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/CONTRIBUTING.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)      243 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/MANIFEST.in
--rw-r--r--   0 asottile  (1000) asottile  (1000)    31414 2022-07-30 19:32:55.215552 pycodestyle-2.9.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3684 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/README.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)        4 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/dev-requirements.txt
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-07-30 19:32:55.207552 pycodestyle-2.9.0/docs/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5584 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/docs/Makefile
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2721 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/docs/advanced.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2582 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/docs/api.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8339 2022-07-30 18:16:16.000000 pycodestyle-2.9.0/docs/conf.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4207 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/docs/developer.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1906 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/docs/index.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)    27283 2022-07-30 18:35:01.000000 pycodestyle-2.9.0/docs/intro.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5106 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/docs/make.bat
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-07-30 19:32:55.207552 pycodestyle-2.9.0/pycodestyle.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)    31414 2022-07-30 19:32:54.000000 pycodestyle-2.9.0/pycodestyle.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1277 2022-07-30 19:32:55.000000 pycodestyle-2.9.0/pycodestyle.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-07-30 19:32:54.000000 pycodestyle-2.9.0/pycodestyle.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       50 2022-07-30 19:32:54.000000 pycodestyle-2.9.0/pycodestyle.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-07-30 19:32:54.000000 pycodestyle-2.9.0/pycodestyle.egg-info/not-zip-safe
--rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2022-07-30 19:32:55.000000 pycodestyle-2.9.0/pycodestyle.egg-info/top_level.txt
--rwxr-xr-x   0 asottile  (1000) asottile  (1000)   103429 2022-07-30 19:31:57.000000 pycodestyle-2.9.0/pycodestyle.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      191 2022-07-30 19:32:55.215552 pycodestyle-2.9.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1858 2022-07-30 18:16:16.000000 pycodestyle-2.9.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-07-30 19:32:55.211552 pycodestyle-2.9.0/testsuite/
--rw-r--r--   0 asottile  (1000) asottile  (1000)      740 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E10.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      737 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E11.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7394 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E12.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13378 2022-07-30 18:35:01.000000 pycodestyle-2.9.0/testsuite/E12not.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1157 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E20.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      226 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E21.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2100 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E22.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      163 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E23.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      216 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E24.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1214 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E25.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1370 2022-07-30 18:16:16.000000 pycodestyle-2.9.0/testsuite/E26.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      681 2022-07-30 18:35:01.000000 pycodestyle-2.9.0/testsuite/E27.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1996 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E30.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2752 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E30not.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      776 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E40.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3129 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E50.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      502 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E70.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1245 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E71.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1284 2022-07-30 19:17:48.000000 pycodestyle-2.9.0/testsuite/E72.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      262 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E73.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      436 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/E90.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2693 2022-07-30 18:35:01.000000 pycodestyle-2.9.0/testsuite/W19.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      460 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/W29.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      269 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/W39.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1348 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/W60.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/crlf.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      152 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/latin-1.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      408 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/noqa.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      925 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/python3.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      372 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/python310.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      266 2022-07-30 18:35:01.000000 pycodestyle-2.9.0/testsuite/python311.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/python35.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      681 2022-07-30 18:16:16.000000 pycodestyle-2.9.0/testsuite/python38.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8176 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/support.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1553 2022-07-30 18:35:01.000000 pycodestyle-2.9.0/testsuite/test_all.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    16581 2022-07-30 18:35:01.000000 pycodestyle-2.9.0/testsuite/test_api.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11155 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/test_blank_lines.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1250 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/test_parser.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7827 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/test_shell.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      894 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/test_util.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)       83 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/utf-8-bom.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1815 2022-07-30 17:52:35.000000 pycodestyle-2.9.0/testsuite/utf-8.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-03 23:13:14.211308 pycodestyle-2.9.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    26671 2022-08-03 23:12:27.000000 pycodestyle-2.9.1/CHANGES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3109 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      243 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/MANIFEST.in
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    31514 2022-08-03 23:13:14.211308 pycodestyle-2.9.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3684 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/README.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        4 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/dev-requirements.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-03 23:13:14.203308 pycodestyle-2.9.1/docs/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5584 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/docs/Makefile
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2721 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/docs/advanced.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2582 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/docs/api.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8339 2022-07-30 18:16:16.000000 pycodestyle-2.9.1/docs/conf.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4207 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/docs/developer.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1906 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/docs/index.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    27283 2022-07-30 18:35:01.000000 pycodestyle-2.9.1/docs/intro.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5106 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/docs/make.bat
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-03 23:13:14.207308 pycodestyle-2.9.1/pycodestyle.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    31514 2022-08-03 23:13:13.000000 pycodestyle-2.9.1/pycodestyle.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1277 2022-08-03 23:13:14.000000 pycodestyle-2.9.1/pycodestyle.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-08-03 23:13:13.000000 pycodestyle-2.9.1/pycodestyle.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       50 2022-08-03 23:13:13.000000 pycodestyle-2.9.1/pycodestyle.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-08-03 23:13:13.000000 pycodestyle-2.9.1/pycodestyle.egg-info/not-zip-safe
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2022-08-03 23:13:14.000000 pycodestyle-2.9.1/pycodestyle.egg-info/top_level.txt
+-rwxr-xr-x   0 asottile  (1000) asottile  (1000)   103501 2022-08-03 23:12:27.000000 pycodestyle-2.9.1/pycodestyle.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      191 2022-08-03 23:13:14.211308 pycodestyle-2.9.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1858 2022-07-30 18:16:16.000000 pycodestyle-2.9.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-08-03 23:13:14.211308 pycodestyle-2.9.1/testsuite/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      740 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E10.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      737 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E11.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7394 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E12.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13378 2022-07-30 18:35:01.000000 pycodestyle-2.9.1/testsuite/E12not.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1157 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E20.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      226 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E21.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2100 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E22.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      163 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E23.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      216 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E24.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1214 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E25.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1370 2022-07-30 18:16:16.000000 pycodestyle-2.9.1/testsuite/E26.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2022-08-03 22:52:37.000000 pycodestyle-2.9.1/testsuite/E27.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1996 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E30.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2752 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E30not.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      776 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E40.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3129 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E50.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      502 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E70.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1245 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E71.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1284 2022-07-30 19:17:48.000000 pycodestyle-2.9.1/testsuite/E72.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      262 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E73.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      436 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/E90.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2693 2022-07-30 18:35:01.000000 pycodestyle-2.9.1/testsuite/W19.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      460 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/W29.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      269 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/W39.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1348 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/W60.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/crlf.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      152 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/latin-1.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      408 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/noqa.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      925 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/python3.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      372 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/python310.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      266 2022-07-30 18:35:01.000000 pycodestyle-2.9.1/testsuite/python311.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       76 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/python35.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      681 2022-07-30 18:16:16.000000 pycodestyle-2.9.1/testsuite/python38.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8176 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/support.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1553 2022-07-30 18:35:01.000000 pycodestyle-2.9.1/testsuite/test_all.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    16581 2022-07-30 18:35:01.000000 pycodestyle-2.9.1/testsuite/test_api.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11155 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/test_blank_lines.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1250 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/test_parser.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7827 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/test_shell.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      894 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/test_util.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       83 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/utf-8-bom.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1815 2022-07-30 17:52:35.000000 pycodestyle-2.9.1/testsuite/utf-8.py
```

### Comparing `pycodestyle-2.9.0/CHANGES.txt` & `pycodestyle-2.9.1/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.9.1 (2022-08-03)
+------------------
+
+Changes:
+
+* E275: fix false positive for yield expressions.
+
 2.9.0 (2022-07-30)
 ------------------
 
 Changes:
 
 * E221, E222, E223, E224: add support for ``:=`` operator.  PR #1032.
 * Drop python 2.7 / 3.5.
```

### Comparing `pycodestyle-2.9.0/CONTRIBUTING.rst` & `pycodestyle-2.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/LICENSE` & `pycodestyle-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/PKG-INFO` & `pycodestyle-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodestyle
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python style guide checker
 Home-page: https://pycodestyle.pycqa.org/
 Author: Johann C. Rocholl
 Author-email: johann@rocholl.net
 Maintainer: Ian Lee
 Maintainer-email: IanLee1521@gmail.com
 License: Expat license
@@ -136,14 +136,21 @@
 
 * `Fork me on GitHub <http://github.com/PyCQA/pycodestyle>`_
 
 
 Changelog
 =========
 
+2.9.1 (2022-08-03)
+------------------
+
+Changes:
+
+* E275: fix false positive for yield expressions.
+
 2.9.0 (2022-07-30)
 ------------------
 
 Changes:
 
 * E221, E222, E223, E224: add support for ``:=`` operator.  PR #1032.
 * Drop python 2.7 / 3.5.
```

### Comparing `pycodestyle-2.9.0/README.rst` & `pycodestyle-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/Makefile` & `pycodestyle-2.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/advanced.rst` & `pycodestyle-2.9.1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/api.rst` & `pycodestyle-2.9.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/conf.py` & `pycodestyle-2.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/developer.rst` & `pycodestyle-2.9.1/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/index.rst` & `pycodestyle-2.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/intro.rst` & `pycodestyle-2.9.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/docs/make.bat` & `pycodestyle-2.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/pycodestyle.egg-info/PKG-INFO` & `pycodestyle-2.9.1/pycodestyle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodestyle
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python style guide checker
 Home-page: https://pycodestyle.pycqa.org/
 Author: Johann C. Rocholl
 Author-email: johann@rocholl.net
 Maintainer: Ian Lee
 Maintainer-email: IanLee1521@gmail.com
 License: Expat license
@@ -136,14 +136,21 @@
 
 * `Fork me on GitHub <http://github.com/PyCQA/pycodestyle>`_
 
 
 Changelog
 =========
 
+2.9.1 (2022-08-03)
+------------------
+
+Changes:
+
+* E275: fix false positive for yield expressions.
+
 2.9.0 (2022-07-30)
 ------------------
 
 Changes:
 
 * E221, E222, E223, E224: add support for ``:=`` operator.  PR #1032.
 * Drop python 2.7 / 3.5.
```

### Comparing `pycodestyle-2.9.0/pycodestyle.egg-info/SOURCES.txt` & `pycodestyle-2.9.1/pycodestyle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/pycodestyle.py` & `pycodestyle-2.9.1/pycodestyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: no cover (<py310)
     tokenize._compile = lru_cache()(tokenize._compile)  # type: ignore
 
-__version__ = '2.9.0'
+__version__ = '2.9.1'
 
 DEFAULT_EXCLUDE = '.svn,CVS,.bzr,.hg,.git,__pycache__,.tox'
 DEFAULT_IGNORE = 'E121,E123,E126,E226,E24,E704,W503,W504'
 try:
     if sys.platform == 'win32':
         USER_CONFIG = os.path.expanduser(r'~\.pycodestyle')
     else:
@@ -491,14 +491,15 @@
         # appear e.g. as "if x is None:", and async/await, which were
         # valid identifier names in old Python versions.
         if (tok0.end == tok1.start and
                 keyword.iskeyword(tok0.string) and
                 tok0.string not in SINGLETONS and
                 tok0.string not in ('async', 'await') and
                 not (tok0.string == 'except' and tok1.string == '*') and
+                not (tok0.string == 'yield' and tok1.string == ')') and
                 tok1.string not in ':\n'):
             yield tok0.end, "E275 missing whitespace after keyword"
 
 
 @register_check
 def missing_whitespace(logical_line):
     r"""Each comma, semicolon or colon should be followed by whitespace.
```

### Comparing `pycodestyle-2.9.0/setup.py` & `pycodestyle-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E10.py` & `pycodestyle-2.9.1/testsuite/E10.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E11.py` & `pycodestyle-2.9.1/testsuite/E11.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E12.py` & `pycodestyle-2.9.1/testsuite/E12.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E12not.py` & `pycodestyle-2.9.1/testsuite/E12not.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E20.py` & `pycodestyle-2.9.1/testsuite/E20.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E22.py` & `pycodestyle-2.9.1/testsuite/E22.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E25.py` & `pycodestyle-2.9.1/testsuite/E25.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E26.py` & `pycodestyle-2.9.1/testsuite/E26.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E27.py` & `pycodestyle-2.9.1/testsuite/E27.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,7 +48,11 @@
 else:
     pass
 #: Okay
 matched = {"true": True, "false": False}
 #: E275:2:11
 if True:
     assert(1)
+#: Okay
+def f():
+    print((yield))
+    x = (yield)
```

### Comparing `pycodestyle-2.9.0/testsuite/E30.py` & `pycodestyle-2.9.1/testsuite/E30.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E30not.py` & `pycodestyle-2.9.1/testsuite/E30not.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E40.py` & `pycodestyle-2.9.1/testsuite/E40.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E50.py` & `pycodestyle-2.9.1/testsuite/E50.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E71.py` & `pycodestyle-2.9.1/testsuite/E71.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/E72.py` & `pycodestyle-2.9.1/testsuite/E72.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/W19.py` & `pycodestyle-2.9.1/testsuite/W19.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/W60.py` & `pycodestyle-2.9.1/testsuite/W60.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/python3.py` & `pycodestyle-2.9.1/testsuite/python3.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/python38.py` & `pycodestyle-2.9.1/testsuite/python38.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/support.py` & `pycodestyle-2.9.1/testsuite/support.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/test_all.py` & `pycodestyle-2.9.1/testsuite/test_all.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/test_api.py` & `pycodestyle-2.9.1/testsuite/test_api.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/test_blank_lines.py` & `pycodestyle-2.9.1/testsuite/test_blank_lines.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/test_parser.py` & `pycodestyle-2.9.1/testsuite/test_parser.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/test_shell.py` & `pycodestyle-2.9.1/testsuite/test_shell.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/test_util.py` & `pycodestyle-2.9.1/testsuite/test_util.py`

 * *Files identical despite different names*

### Comparing `pycodestyle-2.9.0/testsuite/utf-8.py` & `pycodestyle-2.9.1/testsuite/utf-8.py`

 * *Files identical despite different names*

