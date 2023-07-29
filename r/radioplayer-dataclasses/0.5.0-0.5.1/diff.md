# Comparing `tmp/radioplayer_dataclasses-0.5.0.tar.gz` & `tmp/radioplayer_dataclasses-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radioplayer_dataclasses-0.5.0.tar", max compression
+gzip compressed data, was "radioplayer_dataclasses-0.5.1.tar", max compression
```

## Comparing `radioplayer_dataclasses-0.5.0.tar` & `radioplayer_dataclasses-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34520 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/LICENSE
--rw-r--r--   0        0        0     3627 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/README.md
--rw-r--r--   0        0        0     2203 2023-07-02 10:35:28.864344 radioplayer_dataclasses-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2351 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/__init__.py
--rw-r--r--   0        0        0    56457 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/dataclasses.py
--rw-r--r--   0        0        0        0 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/py.typed
--rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-07-29 11:04:52.882740 radioplayer_dataclasses-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3627 2023-07-29 11:04:52.882740 radioplayer_dataclasses-0.5.1/README.md
+-rw-r--r--   0        0        0     2203 2023-07-29 11:05:17.774929 radioplayer_dataclasses-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2351 2023-07-29 11:04:52.890740 radioplayer_dataclasses-0.5.1/radioplayer/dataclasses/__init__.py
+-rw-r--r--   0        0        0    56457 2023-07-29 11:04:52.890740 radioplayer_dataclasses-0.5.1/radioplayer/dataclasses/dataclasses.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:04:52.890740 radioplayer_dataclasses-0.5.1/radioplayer/dataclasses/py.typed
+-rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.5.1/PKG-INFO
```

### Comparing `radioplayer_dataclasses-0.5.0/LICENSE` & `radioplayer_dataclasses-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.0/README.md` & `radioplayer_dataclasses-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.0/pyproject.toml` & `radioplayer_dataclasses-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radioplayer-dataclasses"
-version = "v0.5.0" # 0.0.0 placeholder is replaced on release
+version = "v0.5.1" # 0.0.0 placeholder is replaced on release
 description = "Python dataclasses for radioplayer generated from XSD"
 repository = "https://github.com/radiorabe/python-radioplayer-dataclasses"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -28,15 +28,15 @@
 flake8-isort = ">=5.0.3,<7.0.0"
 flake8-string-format = "^0.3.0"
 flake8-tuple = "^0.4.1"
 lxml = "^4.9.2"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-pylint = "^0.19.0"
-wheel = ">=0.38.4,<0.41.0"
+wheel = ">=0.38.4,<0.42.0"
 xmldiff = "^2.4"
 xsdata = {extras = ["cli"], version = ">=22.12,<24.0"}
 pytest-random-order = "^1.1.0"
 pytest-mypy = "^0.10.3"
 mkdocstrings = {extras = ["python"], version = ">=0.20,<0.23"}
 mkdocs-material = ">=8,<10"
 mkdocs = "^1.4.2"
```

### Comparing `radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/__init__.py` & `radioplayer_dataclasses-0.5.1/radioplayer/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/dataclasses.py` & `radioplayer_dataclasses-0.5.1/radioplayer/dataclasses/dataclasses.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.0/PKG-INFO` & `radioplayer_dataclasses-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radioplayer-dataclasses
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python dataclasses for radioplayer generated from XSD
 Home-page: https://github.com/radiorabe/python-radioplayer-dataclasses
 License: AGPL-3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

