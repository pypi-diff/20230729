# Comparing `tmp/ixBrowser-1.0.0.tar.gz` & `tmp/ixBrowser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ixBrowser-1.0.0.tar", last modified: Sat Jul 29 03:52:06 2023, max compression
+gzip compressed data, was "dist\ixBrowser-1.0.1.tar", last modified: Sat Jul 29 03:54:53 2023, max compression
```

## Comparing `ixBrowser-1.0.0.tar` & `ixBrowser-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 03:52:06.648785 ixBrowser-1.0.0/
--rw-rw-rw-   0        0        0     1119 2023-07-29 03:38:21.000000 ixBrowser-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      633 2023-07-29 03:52:06.647787 ixBrowser-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 03:52:06.639813 ixBrowser-1.0.0/ixBrowser/
--rw-rw-rw-   0        0        0        0 2023-07-29 03:36:18.000000 ixBrowser-1.0.0/ixBrowser/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-07-29 03:35:16.000000 ixBrowser-1.0.0/ixBrowser/client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:52:06.646789 ixBrowser-1.0.0/ixBrowser.egg-info/
--rw-rw-rw-   0        0        0      633 2023-07-29 03:52:06.000000 ixBrowser-1.0.0/ixBrowser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-07-29 03:52:06.000000 ixBrowser-1.0.0/ixBrowser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 03:52:06.000000 ixBrowser-1.0.0/ixBrowser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-07-29 03:52:06.000000 ixBrowser-1.0.0/ixBrowser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 03:52:06.000000 ixBrowser-1.0.0/ixBrowser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 03:52:06.648785 ixBrowser-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1462 2023-07-29 03:52:03.000000 ixBrowser-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:54:53.323321 ixBrowser-1.0.1/
+-rw-rw-rw-   0        0        0     1119 2023-07-29 03:38:21.000000 ixBrowser-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      633 2023-07-29 03:54:53.322324 ixBrowser-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 03:54:53.311361 ixBrowser-1.0.1/ixBrowser/
+-rw-rw-rw-   0        0        0        0 2023-07-29 03:36:18.000000 ixBrowser-1.0.1/ixBrowser/__init__.py
+-rw-rw-rw-   0        0        0     9475 2023-07-29 03:35:16.000000 ixBrowser-1.0.1/ixBrowser/client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:54:53.320331 ixBrowser-1.0.1/ixBrowser.egg-info/
+-rw-rw-rw-   0        0        0      633 2023-07-29 03:54:53.000000 ixBrowser-1.0.1/ixBrowser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-29 03:54:53.000000 ixBrowser-1.0.1/ixBrowser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 03:54:53.000000 ixBrowser-1.0.1/ixBrowser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      339 2023-07-29 03:54:53.000000 ixBrowser-1.0.1/ixBrowser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 03:54:53.000000 ixBrowser-1.0.1/ixBrowser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 03:54:53.323321 ixBrowser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1462 2023-07-29 03:54:50.000000 ixBrowser-1.0.1/setup.py
```

### Comparing `ixBrowser-1.0.0/LICENSE` & `ixBrowser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.0.0/PKG-INFO` & `ixBrowser-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.0.0
+Version: 1.0.1
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `ixBrowser-1.0.0/ixBrowser/client.py` & `ixBrowser-1.0.1/ixBrowser/client.py`

 * *Files identical despite different names*

### Comparing `ixBrowser-1.0.0/ixBrowser.egg-info/PKG-INFO` & `ixBrowser-1.0.1/ixBrowser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ixBrowser
-Version: 1.0.0
+Version: 1.0.1
 Summary: A SDK for ixBrowser
 Home-page: https://github.com/ontisme/ixBrowser
 Download-URL: https://pypi.org/project/ixBrowser/
 Author: Alan Ting & Ontisme
 Author-email: alanting0716@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `ixBrowser-1.0.0/setup.py` & `ixBrowser-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 PACKAGE_NAME = "ixBrowser"
 AUTHOR = "Alan Ting & Ontisme"
 AUTHOR_EMAIL = "alanting0716@gmail.com"
 URL = "https://github.com/ontisme/ixBrowser"
 DOWNLOAD_URL = "https://pypi.org/project/ixBrowser/"
 
 LICENSE = "MIT"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "A SDK for ixBrowser"
 LONG_DESCRIPTION = (HERE / "docs" / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
 
 with open((HERE / "requirements.txt"), encoding="utf8", errors='ignore') as f:
     requirements = f.read()
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 
 with open((HERE / "dev_requirements.txt"), encoding="utf8", errors='ignore') as f:
     dev_requirements = f.read()
 EXTRAS_REQUIRE = {"dev": [s.strip() for s in dev_requirements.split("\n")]}
 
 CLASSIFIERS = [f"Programming Language :: Python :: 3.{str(v)}" for v in range(7, 12)]
-PYTHON_REQUIRES = ">=3.7"
+PYTHON_REQUIRES = ">=3.9"
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
```

