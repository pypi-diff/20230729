# Comparing `tmp/gridworks_cert-0.3.0.tar.gz` & `tmp/gridworks_cert-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_cert-0.3.0.tar", max compression
+gzip compressed data, was "gridworks_cert-0.3.1.tar", max compression
```

## Comparing `gridworks_cert-0.3.0.tar` & `gridworks_cert-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/LICENSE
--rw-r--r--   0        0        0     3837 2023-07-27 23:18:42.450132 gridworks_cert-0.3.0/README.md
--rw-r--r--   0        0        0     2081 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/__init__.py
--rw-r--r--   0        0        0      455 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/__main__.py
--rw-r--r--   0        0        0       99 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/ca/__init__.py
--rw-r--r--   0        0        0     7416 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/src/gwcert/ca/__main__.py
--rw-r--r--   0        0        0      172 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/src/gwcert/key/__init__.py
--rw-r--r--   0        0        0    21478 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/src/gwcert/key/__main__.py
--rw-r--r--   0        0        0      196 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/paths.py
--rw-r--r--   0        0        0        0 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/py.typed
--rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 gridworks_cert-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-29 12:19:16.884257 gridworks_cert-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3837 2023-07-29 12:19:16.884257 gridworks_cert-0.3.1/README.md
+-rw-r--r--   0        0        0     2132 2023-07-29 12:19:37.828654 gridworks_cert-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/ca/__init__.py
+-rw-r--r--   0        0        0     7416 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/ca/__main__.py
+-rw-r--r--   0        0        0      172 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/key/__init__.py
+-rw-r--r--   0        0        0    21478 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/key/__main__.py
+-rw-r--r--   0        0        0      196 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/paths.py
+-rw-r--r--   0        0        0        0 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/py.typed
+-rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 gridworks_cert-0.3.1/PKG-INFO
```

### Comparing `gridworks_cert-0.3.0/LICENSE` & `gridworks_cert-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.0/README.md` & `gridworks_cert-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.0/pyproject.toml` & `gridworks_cert-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "gridworks-cert"
-version = "0.3.0"
-description = "gwcert"
+version = "0.3.1"
+description = "TLS certificate management tools for GridWorks"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://github.com/anschweitzer/gridworks-cert"
-repository = "https://github.com/anschweitzer/gridworks-cert"
+homepage = "https://github.com/thegridelectric/gridworks-cert"
+repository = "https://github.com/thegridelectric/gridworks-cert"
 documentation = "https://gridworks-cert.readthedocs.io"
 packages = [
     { include = "gwcert", from = "src" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
-Changelog = "https://github.com/anschweitzer/gridworks-cert/releases"
+Changelog = "https://github.com/thegridelectric/gridworks-cert/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ownca = ">=0.4.0"
 typer = ">=0.9.0"
-xdg = "^6.0.0"
-rich = "^13.4.2"
+xdg = ">=6.0.0"
+rich = ">=12.0.0"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `gridworks_cert-0.3.0/src/gwcert/ca/__main__.py` & `gridworks_cert-0.3.1/src/gwcert/ca/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.0/src/gwcert/key/__main__.py` & `gridworks_cert-0.3.1/src/gwcert/key/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.0/PKG-INFO` & `gridworks_cert-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gridworks-cert
-Version: 0.3.0
-Summary: gwcert
-Home-page: https://github.com/anschweitzer/gridworks-cert
+Version: 0.3.1
+Summary: TLS certificate management tools for GridWorks
+Home-page: https://github.com/thegridelectric/gridworks-cert
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ownca (>=0.4.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: rich (>=12.0.0)
 Requires-Dist: typer (>=0.9.0)
-Requires-Dist: xdg (>=6.0.0,<7.0.0)
-Project-URL: Changelog, https://github.com/anschweitzer/gridworks-cert/releases
+Requires-Dist: xdg (>=6.0.0)
+Project-URL: Changelog, https://github.com/thegridelectric/gridworks-cert/releases
 Project-URL: Documentation, https://gridworks-cert.readthedocs.io
-Project-URL: Repository, https://github.com/anschweitzer/gridworks-cert
+Project-URL: Repository, https://github.com/thegridelectric/gridworks-cert
 Description-Content-Type: text/markdown
 
 # gwcert
 
 [![PyPI](https://img.shields.io/pypi/v/gridworks-cert.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/gridworks-cert.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/gridworks-cert)][python version]
```

