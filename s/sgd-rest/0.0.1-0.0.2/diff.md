# Comparing `tmp/sgd_rest-0.0.1.tar.gz` & `tmp/sgd_rest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgd_rest-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sgd_rest-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sgd_rest-0.0.1.tar` & `sgd_rest-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       83 2023-07-28 20:05:08.942291 sgd_rest-0.0.1/.flake8
--rw-r--r--   0        0        0      170 2023-07-29 16:32:47.775361 sgd_rest-0.0.1/.github/dependabot.yaml
--rw-r--r--   0        0        0      635 2023-07-29 16:33:55.841454 sgd_rest-0.0.1/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     3078 2023-07-26 19:12:59.055162 sgd_rest-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2023-07-26 19:12:59.055317 sgd_rest-0.0.1/LICENSE
--rw-r--r--   0        0        0      897 2023-07-28 20:07:26.866494 sgd_rest-0.0.1/Makefile
--rw-r--r--   0        0        0     4588 2023-07-29 16:07:35.926440 sgd_rest-0.0.1/README.md
--rw-r--r--   0        0        0       26 2023-07-28 19:54:17.063480 sgd_rest-0.0.1/conftest.py
--rw-r--r--   0        0        0      791 2023-07-29 16:36:20.929255 sgd_rest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       32 2023-07-28 16:33:46.903493 sgd_rest-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0        9 2023-07-28 16:32:29.411112 sgd_rest-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1169 2023-07-29 16:34:04.470794 sgd_rest-0.0.1/setup.cfg
--rw-r--r--   0        0        0      114 2023-07-29 16:31:42.225530 sgd_rest-0.0.1/sgd/__init__.py
--rw-r--r--   0        0        0     8091 2023-07-28 20:08:01.613736 sgd_rest-0.0.1/sgd/api.py
--rw-r--r--   0        0        0      225 2023-07-28 19:59:01.313282 sgd_rest-0.0.1/sgd/constants.py
--rw-r--r--   0        0        0   305093 2023-07-26 19:44:32.597219 sgd_rest-0.0.1/sgd/data/genes_to_loci.json
--rw-r--r--   0        0        0      109 2023-07-28 19:53:17.407918 sgd_rest-0.0.1/sgd/exceptions.py
--rw-r--r--   0        0        0     4871 2023-07-28 19:53:17.391282 sgd_rest-0.0.1/tests/test_api.py
--rw-r--r--   0        0        0      814 2023-07-28 20:18:05.241377 sgd_rest-0.0.1/tests/test_constants.py
--rw-r--r--   0        0        0      285 2023-07-28 19:54:08.182118 sgd_rest-0.0.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 sgd_rest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       83 2023-07-28 20:05:08.942291 sgd_rest-0.0.2/.flake8
+-rw-r--r--   0        0        0      170 2023-07-29 16:32:47.775361 sgd_rest-0.0.2/.github/dependabot.yaml
+-rw-r--r--   0        0        0      635 2023-07-29 16:33:55.841454 sgd_rest-0.0.2/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     3078 2023-07-26 19:12:59.055162 sgd_rest-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2023-07-26 19:12:59.055317 sgd_rest-0.0.2/LICENSE
+-rw-r--r--   0        0        0      897 2023-07-28 20:07:26.866494 sgd_rest-0.0.2/Makefile
+-rw-r--r--   0        0        0     5086 2023-07-29 17:03:15.468772 sgd_rest-0.0.2/README.md
+-rw-r--r--   0        0        0       26 2023-07-28 19:54:17.063480 sgd_rest-0.0.2/conftest.py
+-rw-r--r--   0        0        0      791 2023-07-29 16:36:20.929255 sgd_rest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-07-28 16:33:46.903493 sgd_rest-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0        9 2023-07-28 16:32:29.411112 sgd_rest-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1169 2023-07-29 16:34:04.470794 sgd_rest-0.0.2/setup.cfg
+-rw-r--r--   0        0        0      114 2023-07-29 17:05:13.554796 sgd_rest-0.0.2/sgd/__init__.py
+-rw-r--r--   0        0        0     8091 2023-07-28 20:08:01.613736 sgd_rest-0.0.2/sgd/api.py
+-rw-r--r--   0        0        0      225 2023-07-28 19:59:01.313282 sgd_rest-0.0.2/sgd/constants.py
+-rw-r--r--   0        0        0   305093 2023-07-26 19:44:32.597219 sgd_rest-0.0.2/sgd/data/genes_to_loci.json
+-rw-r--r--   0        0        0      109 2023-07-28 19:53:17.407918 sgd_rest-0.0.2/sgd/exceptions.py
+-rw-r--r--   0        0        0     4871 2023-07-28 19:53:17.391282 sgd_rest-0.0.2/tests/test_api.py
+-rw-r--r--   0        0        0      814 2023-07-28 20:18:05.241377 sgd_rest-0.0.2/tests/test_constants.py
+-rw-r--r--   0        0        0      285 2023-07-28 19:54:08.182118 sgd_rest-0.0.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0     5829 1970-01-01 00:00:00.000000 sgd_rest-0.0.2/PKG-INFO
```

### Comparing `sgd_rest-0.0.1/.github/workflows/ci.yaml` & `sgd_rest-0.0.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/.gitignore` & `sgd_rest-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/LICENSE` & `sgd_rest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/Makefile` & `sgd_rest-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/README.md` & `sgd_rest-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # sgd-rest
 
 Saccharomyces Genome Database ([SGD](https://www.yeastgenome.org/)) REST API wrapper. Refer to the [SGD REST](https://www.yeastgenome.org/api/doc) page for information about API usage and terms of service.
 
+[![pypiv](https://img.shields.io/pypi/v/sgd-rest.svg)](https://pypi.python.org/pypi/sgd-rest)
+[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![continuous-integration](https://github.com/irahorecka/sgd-rest/workflows/continuous-integration/badge.svg?branch=main)](https://github.com/irahorecka/sgd-rest/actions)
+[![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/irahorecka/sgd-rest/main/LICENSE)
+
 ## Installation
 
 ```bash
 pip install sgd-rest
 ```
 
 ## Quick start
@@ -95,15 +100,15 @@
 
 * `url`: Gets the endpoint's URL. Available for all classes.
 * `locus_id`: Gets the endpoint's locus ID. Avaialble for `locus` and `gene` classes.
 
 ```python
 import sgd
 
-tor2 = sgd.locus("TOR2")
+tor2 = sgd.gene("TOR2")
 
 # 1 
 print(tor2.url)
 # >>> 'https://www.yeastgenome.org/backend/locus/S000001686'
 
 # 2
 print(tor2.locus_id)
@@ -123,15 +128,15 @@
 except InvalidGene:
     print("Whoops, an invalid gene was queried.")
 ```
 
 ## Contribute
 
 * [Issues Tracker](https://github.com/irahorecka/sgd-rest/issues)
-* [Source Code](https://github.com/irahorecka/sgd-rest/tree/master/sgd)
+* [Source Code](https://github.com/irahorecka/sgd-rest/tree/main/sgd)
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/sgd-rest/issues).
 
 ## License
```

### Comparing `sgd_rest-0.0.1/pyproject.toml` & `sgd_rest-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/setup.cfg` & `sgd_rest-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/sgd/api.py` & `sgd_rest-0.0.2/sgd/api.py`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/sgd/data/genes_to_loci.json` & `sgd_rest-0.0.2/sgd/data/genes_to_loci.json`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/tests/test_api.py` & `sgd_rest-0.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/tests/test_constants.py` & `sgd_rest-0.0.2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.1/PKG-INFO` & `sgd_rest-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgd-rest
-Version: 0.0.1
+Version: 0.0.2
 Summary: sgd
 Home-page: https://github.com/irahorecka/sgd-rest
 Author: Ira Horecka
 Author-email: ira89@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -19,14 +19,19 @@
 Classifier: Topic :: Utilities
 Requires-Dist: requests>=2.28.0
 
 # sgd-rest
 
 Saccharomyces Genome Database ([SGD](https://www.yeastgenome.org/)) REST API wrapper. Refer to the [SGD REST](https://www.yeastgenome.org/api/doc) page for information about API usage and terms of service.
 
+[![pypiv](https://img.shields.io/pypi/v/sgd-rest.svg)](https://pypi.python.org/pypi/sgd-rest)
+[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![continuous-integration](https://github.com/irahorecka/sgd-rest/workflows/continuous-integration/badge.svg?branch=main)](https://github.com/irahorecka/sgd-rest/actions)
+[![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/irahorecka/sgd-rest/main/LICENSE)
+
 ## Installation
 
 ```bash
 pip install sgd-rest
 ```
 
 ## Quick start
@@ -116,15 +121,15 @@
 
 * `url`: Gets the endpoint's URL. Available for all classes.
 * `locus_id`: Gets the endpoint's locus ID. Avaialble for `locus` and `gene` classes.
 
 ```python
 import sgd
 
-tor2 = sgd.locus("TOR2")
+tor2 = sgd.gene("TOR2")
 
 # 1 
 print(tor2.url)
 # >>> 'https://www.yeastgenome.org/backend/locus/S000001686'
 
 # 2
 print(tor2.locus_id)
@@ -144,15 +149,15 @@
 except InvalidGene:
     print("Whoops, an invalid gene was queried.")
 ```
 
 ## Contribute
 
 * [Issues Tracker](https://github.com/irahorecka/sgd-rest/issues)
-* [Source Code](https://github.com/irahorecka/sgd-rest/tree/master/sgd)
+* [Source Code](https://github.com/irahorecka/sgd-rest/tree/main/sgd)
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/sgd-rest/issues).
 
 ## License
```

