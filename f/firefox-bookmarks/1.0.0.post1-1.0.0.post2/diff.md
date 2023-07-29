# Comparing `tmp/firefox_bookmarks-1.0.0.post1.tar.gz` & `tmp/firefox_bookmarks-1.0.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefox_bookmarks-1.0.0.post1.tar", max compression
+gzip compressed data, was "firefox_bookmarks-1.0.0.post2.tar", max compression
```

## Comparing `firefox_bookmarks-1.0.0.post1.tar` & `firefox_bookmarks-1.0.0.post2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    19028 2023-07-29 20:13:57.122984 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/__init__.py
--rw-r--r--   0        0        0     4451 2023-07-29 20:13:57.138108 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/bookmark.py
--rw-r--r--   0        0        0     1268 2023-07-25 08:53:37.841063 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/connect.py
--rw-r--r--   0        0        0      437 2023-07-29 21:08:46.723557 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/constants.py
--rw-r--r--   0        0        0     2391 2023-07-24 14:39:36.813164 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/locate.py
--rw-r--r--   0        0        0     3974 2023-07-29 20:13:57.164801 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/models.py
--rw-r--r--   0        0        0    35184 2023-07-21 16:18:12.325494 firefox_bookmarks-1.0.0.post1/LICENSE
--rw-r--r--   0        0        0     1423 2023-07-29 21:03:36.778493 firefox_bookmarks-1.0.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2059 2023-07-29 21:08:19.526471 firefox_bookmarks-1.0.0.post1/README.md
--rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 firefox_bookmarks-1.0.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    19028 2023-07-29 20:13:57.122984 firefox_bookmarks-1.0.0.post2/firefox_bookmarks/__init__.py
+-rw-r--r--   0        0        0     4451 2023-07-29 20:13:57.138108 firefox_bookmarks-1.0.0.post2/firefox_bookmarks/bookmark.py
+-rw-r--r--   0        0        0     1268 2023-07-25 08:53:37.841063 firefox_bookmarks-1.0.0.post2/firefox_bookmarks/connect.py
+-rw-r--r--   0        0        0      437 2023-07-29 21:15:08.530104 firefox_bookmarks-1.0.0.post2/firefox_bookmarks/constants.py
+-rw-r--r--   0        0        0     2391 2023-07-24 14:39:36.813164 firefox_bookmarks-1.0.0.post2/firefox_bookmarks/locate.py
+-rw-r--r--   0        0        0     3974 2023-07-29 20:13:57.164801 firefox_bookmarks-1.0.0.post2/firefox_bookmarks/models.py
+-rw-r--r--   0        0        0    35184 2023-07-21 16:18:12.325494 firefox_bookmarks-1.0.0.post2/LICENSE
+-rw-r--r--   0        0        0     1423 2023-07-29 21:14:39.920338 firefox_bookmarks-1.0.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     1985 2023-07-29 21:13:43.581133 firefox_bookmarks-1.0.0.post2/README.md
+-rw-r--r--   0        0        0     3426 1970-01-01 00:00:00.000000 firefox_bookmarks-1.0.0.post2/PKG-INFO
```

### Comparing `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/__init__.py` & `firefox_bookmarks-1.0.0.post2/firefox_bookmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/bookmark.py` & `firefox_bookmarks-1.0.0.post2/firefox_bookmarks/bookmark.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/connect.py` & `firefox_bookmarks-1.0.0.post2/firefox_bookmarks/connect.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/locate.py` & `firefox_bookmarks-1.0.0.post2/firefox_bookmarks/locate.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/models.py` & `firefox_bookmarks-1.0.0.post2/firefox_bookmarks/models.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0.post1/LICENSE` & `firefox_bookmarks-1.0.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0.post1/pyproject.toml` & `firefox_bookmarks-1.0.0.post2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firefox-bookmarks"
-version = "1.0.0.post1"
+version = "1.0.0.post2"
 description = "Manage your Firefox bookmarks with ease"
 authors = ["Aditya Rajput <adiraj20072002@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [{ include = "firefox_bookmarks" }]
 repository = "https://github.com/BURG3R5/firefox-bookmarks"
 documentation = "https://github.com/BURG3R5/firefox-bookmarks"
```

### Comparing `firefox_bookmarks-1.0.0.post1/README.md` & `firefox_bookmarks-1.0.0.post2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-<img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/BURG3R5/firefox-bookmarks/ci.yml?branch=main&style=flat-square">
-<img alt="PyPI" src="https://img.shields.io/pypi/v/firefox-bookmarks?style=flat-square">
-<img alt="License - AGPL v3 or later" src="https://img.shields.io/pypi/l/firefox-bookmarks?style=flat-square">
-<img alt="Code style: YAPF" src="https://img.shields.io/badge/code%20style-yapf-blue?style=flat-square">
-<img alt="Code style: isort" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square">
+![CI Status](https://img.shields.io/github/actions/workflow/status/BURG3R5/firefox-bookmarks/ci.yml?branch=main&style=flat-square) ![PyPI](https://img.shields.io/pypi/v/firefox-bookmarks?style=flat-square) ![License - AGPL v3 or later](https://img.shields.io/pypi/l/firefox-bookmarks?style=flat-square) ![Code style: YAPF](https://img.shields.io/badge/code%20style-yapf-blue?style=flat-square) ![Code style: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square)
 
 # firefox-bookmarks
 
 Manage your Firefox bookmarks with ease
 
 ## installation
```

### Comparing `firefox_bookmarks-1.0.0.post1/PKG-INFO` & `firefox_bookmarks-1.0.0.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefox-bookmarks
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: Manage your Firefox bookmarks with ease
 Home-page: https://github.com/BURG3R5/firefox-bookmarks
 License: AGPL-3.0-or-later
 Keywords: firefox,bookmarks,browser,util
 Author: Aditya Rajput
 Author-email: adiraj20072002@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -26,19 +26,15 @@
 Classifier: Topic :: Utilities
 Requires-Dist: peewee (>=3.16.2,<4.0.0)
 Project-URL: Changelog, https://github.com/BURG3R5/firefox-bookmarks/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/BURG3R5/firefox-bookmarks
 Project-URL: Repository, https://github.com/BURG3R5/firefox-bookmarks
 Description-Content-Type: text/markdown
 
-<img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/BURG3R5/firefox-bookmarks/ci.yml?branch=main&style=flat-square">
-<img alt="PyPI" src="https://img.shields.io/pypi/v/firefox-bookmarks?style=flat-square">
-<img alt="License - AGPL v3 or later" src="https://img.shields.io/pypi/l/firefox-bookmarks?style=flat-square">
-<img alt="Code style: YAPF" src="https://img.shields.io/badge/code%20style-yapf-blue?style=flat-square">
-<img alt="Code style: isort" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square">
+![CI Status](https://img.shields.io/github/actions/workflow/status/BURG3R5/firefox-bookmarks/ci.yml?branch=main&style=flat-square) ![PyPI](https://img.shields.io/pypi/v/firefox-bookmarks?style=flat-square) ![License - AGPL v3 or later](https://img.shields.io/pypi/l/firefox-bookmarks?style=flat-square) ![Code style: YAPF](https://img.shields.io/badge/code%20style-yapf-blue?style=flat-square) ![Code style: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square)
 
 # firefox-bookmarks
 
 Manage your Firefox bookmarks with ease
 
 ## installation
```

