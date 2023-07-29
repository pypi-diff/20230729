# Comparing `tmp/ixBrowser-1.6.0.tar.gz` & `tmp/ixBrowser-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ixBrowser-1.6.0.tar", last modified: Sat Jul 29 07:36:50 2023, max compression
+gzip compressed data, was "dist\ixBrowser-1.6.1.tar", last modified: Sat Jul 29 07:44:19 2023, max compression
```

## Comparing `ixBrowser-1.6.0.tar` & `ixBrowser-1.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/
--rw-rw-rw-   0        0        0     1119 2023-07-29 07:13:14.000000 ixBrowser-1.6.0/LICENSE
--rw-rw-rw-   0        0        0      633 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-07-29 07:13:14.000000 ixBrowser-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.6.0/ixBrowser/__init__.py
--rw-rw-rw-   0        0        0     9546 2023-07-29 07:31:13.000000 ixBrowser-1.6.0/ixBrowser/client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser/tests/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.6.0/ixBrowser/tests/__init__.py
--rw-rw-rw-   0        0        0     1626 2023-07-29 07:13:14.000000 ixBrowser-1.6.0/ixBrowser/tests/test_ixbrowser.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser/utils/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.6.0/ixBrowser/utils/__init__.py
--rw-rw-rw-   0        0        0     1714 2023-07-29 07:13:14.000000 ixBrowser-1.6.0/ixBrowser/utils/use_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser.egg-info/
--rw-rw-rw-   0        0        0      633 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/ixBrowser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 07:36:50.000000 ixBrowser-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1462 2023-07-29 07:36:47.000000 ixBrowser-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:44:19.000000 ixBrowser-1.6.1/
+-rw-rw-rw-   0        0        0     1119 2023-07-29 07:13:14.000000 ixBrowser-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     1163 2023-07-29 07:44:19.000000 ixBrowser-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-29 07:43:57.000000 ixBrowser-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 07:44:19.000000 ixBrowser-1.6.1/ixBrowser/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.6.1/ixBrowser/__init__.py
+-rw-rw-rw-   0        0        0     9546 2023-07-29 07:31:13.000000 ixBrowser-1.6.1/ixBrowser/client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:44:19.000000 ixBrowser-1.6.1/ixBrowser/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.6.1/ixBrowser/tests/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-07-29 07:13:14.000000 ixBrowser-1.6.1/ixBrowser/tests/test_ixbrowser.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:44:19.000000 ixBrowser-1.6.1/ixBrowser/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:13:14.000000 ixBrowser-1.6.1/ixBrowser/utils/__init__.py
+-rw-rw-rw-   0        0        0     1714 2023-07-29 07:13:14.000000 ixBrowser-1.6.1/ixBrowser/utils/use_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:44:19.000000 ixBrowser-1.6.1/ixBrowser.egg-info/
+-rw-rw-rw-   0        0        0     1163 2023-07-29 07:44:18.000000 ixBrowser-1.6.1/ixBrowser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-07-29 07:44:18.000000 ixBrowser-1.6.1/ixBrowser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 07:44:18.000000 ixBrowser-1.6.1/ixBrowser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-07-29 07:44:18.000000 ixBrowser-1.6.1/ixBrowser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 07:44:18.000000 ixBrowser-1.6.1/ixBrowser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 07:44:19.000000 ixBrowser-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-07-29 07:42:39.000000 ixBrowser-1.6.1/setup.py
```

### Comparing `ixBrowser-1.6.0/LICENSE` & `ixBrowser-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.6.0/ixBrowser/client.py` & `ixBrowser-1.6.1/ixBrowser/client.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.6.0/ixBrowser/tests/test_ixbrowser.py` & `ixBrowser-1.6.1/ixBrowser/tests/test_ixbrowser.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.6.0/ixBrowser/utils/use_logger.py` & `ixBrowser-1.6.1/ixBrowser/utils/use_logger.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.6.0/setup.py` & `ixBrowser-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 PACKAGE_NAME = "ixBrowser"
 AUTHOR = "Alan Ting & Ontisme"
 AUTHOR_EMAIL = "alanting0716@gmail.com"
 URL = "https://github.com/ontisme/ixBrowser"
 DOWNLOAD_URL = "https://pypi.org/project/ixBrowser/"
 
 LICENSE = "MIT"
-VERSION = "1.6.0"
+VERSION = "1.6.1"
 DESCRIPTION = "A SDK for ixBrowser"
-LONG_DESCRIPTION = (HERE / "docs" / "README.md").read_text(encoding="utf8")
+LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 
 with open((HERE / "requirements.txt"), encoding="utf8", errors='ignore') as f:
     requirements = f.read()
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 
 with open((HERE / "dev_requirements.txt"), encoding="utf8", errors='ignore') as f:
```

