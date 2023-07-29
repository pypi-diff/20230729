# Comparing `tmp/purgatory-1.0.2.tar.gz` & `tmp/purgatory-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purgatory-1.0.2.tar", max compression
+gzip compressed data, was "purgatory-1.0.3.tar", max compression
```

## Comparing `purgatory-1.0.2.tar` & `purgatory-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1523 2021-12-28 07:38:48.830707 purgatory-1.0.2/LICENSE
--rw-r--r--   0        0        0     3314 2022-01-04 12:22:12.260583 purgatory-1.0.2/README.rst
--rw-r--r--   0        0        0     1559 2023-05-10 11:38:05.322742 purgatory-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1199 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/__init__.py
--rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/__init__.py
--rw-r--r--   0        0        0       85 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/__init__.py
--rw-r--r--   0        0        0      304 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/base.py
--rw-r--r--   0        0        0      221 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/commands.py
--rw-r--r--   0        0        0      554 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/events.py
--rw-r--r--   0        0        0     7510 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/model.py
--rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/py.typed
--rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/__init__.py
--rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/__init__.py
--rw-r--r--   0        0        0     5795 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/circuitbreaker.py
--rw-r--r--   0        0        0     1633 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/message_handlers.py
--rw-r--r--   0        0        0     3723 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/messagebus.py
--rw-r--r--   0        0        0     4614 2023-05-10 11:37:55.332762 purgatory-1.0.2/src/purgatory/service/_async/repository.py
--rw-r--r--   0        0        0     1833 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/unit_of_work.py
--rw-r--r--   0        0        0      274 2023-05-10 11:37:55.332762 purgatory-1.0.2/src/purgatory/service/_redis.py
--rw-r--r--   0        0        0        0 2023-05-10 11:38:00.232752 purgatory-1.0.2/src/purgatory/service/_sync/__init__.py
--rw-r--r--   0        0        0     5663 2023-05-10 11:38:00.239419 purgatory-1.0.2/src/purgatory/service/_sync/circuitbreaker.py
--rw-r--r--   0        0        0     1573 2023-05-10 11:38:00.866084 purgatory-1.0.2/src/purgatory/service/_sync/message_handlers.py
--rw-r--r--   0        0        0     3692 2023-05-10 11:38:00.242752 purgatory-1.0.2/src/purgatory/service/_sync/messagebus.py
--rw-r--r--   0        0        0     4433 2023-05-10 11:38:00.899418 purgatory-1.0.2/src/purgatory/service/_sync/repository.py
--rw-r--r--   0        0        0     1746 2023-05-10 11:38:00.242752 purgatory-1.0.2/src/purgatory/service/_sync/unit_of_work.py
--rw-r--r--   0        0        0      945 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/typing.py
--rw-r--r--   0        0        0      383 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/typing.py
--rw-r--r--   0        0        0     4379 1970-01-01 00:00:00.000000 purgatory-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1523 2021-12-28 07:38:48.830707 purgatory-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3410 2023-07-23 15:11:39.521798 purgatory-1.0.3/README.rst
+-rw-r--r--   0        0        0     1590 2023-07-29 13:03:59.770700 purgatory-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1199 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/__init__.py
+-rw-r--r--   0        0        0      304 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/base.py
+-rw-r--r--   0        0        0      221 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/commands.py
+-rw-r--r--   0        0        0      554 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/messages/events.py
+-rw-r--r--   0        0        0     7510 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/domain/model.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/py.typed
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/__init__.py
+-rw-r--r--   0        0        0     5795 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/circuitbreaker.py
+-rw-r--r--   0        0        0     1633 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/message_handlers.py
+-rw-r--r--   0        0        0     3723 2023-05-10 11:55:56.516868 purgatory-1.0.3/src/purgatory/service/_async/messagebus.py
+-rw-r--r--   0        0        0     4614 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/_async/repository.py
+-rw-r--r--   0        0        0     1833 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/_async/unit_of_work.py
+-rw-r--r--   0        0        0      274 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/_redis.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:03:55.197350 purgatory-1.0.3/src/purgatory/service/_sync/__init__.py
+-rw-r--r--   0        0        0     5663 2023-07-29 13:03:55.200683 purgatory-1.0.3/src/purgatory/service/_sync/circuitbreaker.py
+-rw-r--r--   0        0        0     1573 2023-07-29 13:03:55.754019 purgatory-1.0.3/src/purgatory/service/_sync/message_handlers.py
+-rw-r--r--   0        0        0     3692 2023-07-29 13:03:55.204017 purgatory-1.0.3/src/purgatory/service/_sync/messagebus.py
+-rw-r--r--   0        0        0     4433 2023-07-29 13:03:55.780686 purgatory-1.0.3/src/purgatory/service/_sync/repository.py
+-rw-r--r--   0        0        0     1746 2023-07-29 13:03:55.207350 purgatory-1.0.3/src/purgatory/service/_sync/unit_of_work.py
+-rw-r--r--   0        0        0      945 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/service/typing.py
+-rw-r--r--   0        0        0      383 2023-05-10 11:55:56.520201 purgatory-1.0.3/src/purgatory/typing.py
+-rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 purgatory-1.0.3/PKG-INFO
```

### Comparing `purgatory-1.0.2/LICENSE` & `purgatory-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/README.rst` & `purgatory-1.0.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Purgatory
 =========
 
-.. image:: https://readthedocs.org/projects/purgatory/badge/?version=latest
-   :target: https://purgatory.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
+.. image:: https://github.com/mardiros/purgatory/actions/workflows/gh-pages.yml/badge.svg
+   :target: https://mardiros.github.io/purgatory/
+   :alt: Documentation
 
 .. image:: https://github.com/mardiros/purgatory/actions/workflows/main.yml/badge.svg
    :target: https://github.com/mardiros/purgatory/actions/workflows/main.yml
    :alt: Continuous Integration Status
 
 .. image:: https://codecov.io/gh/mardiros/purgatory/branch/main/graph/badge.svg?token=LFVOQC2C9E
    :target: https://codecov.io/gh/mardiros/purgatory
@@ -29,15 +29,15 @@
 --------------------------------------------
 
 The Purgatory library has been develop to be used in `blacksmith`_ where
 the library aiobreaker was used but I encountered limitation so, I decide
 to build my own implementation that feet well with `blacksmith`_.
 
 
-.. _`blacksmith`: https://python-blacksmith.readthedocs.io/en/latest/
+.. _`blacksmith`: https://mardiros.github.io/blacksmith/
 
 
 Features
 --------
 
 Purgatory supports the creation of many circuit breakers easily, that 
 can be used as context manager or decorator.
@@ -94,17 +94,22 @@
 
 
 Read More
 ---------
 
 You can read the `full documentation of this library here`_.
 
-.. _`full documentation of this library here`: https://purgatory.readthedocs.io/en/latest/user/introduction.html
+.. _`full documentation of this library here`: https://mardiros.github.io/purgatory/user/introduction.html
 
 
+.. important::
+
+   | The documentation has been moved to github pages.
+   | The documentation under readthedocs is obsolete. 
+
 Alternatives
 ------------
 
 Here is a list of alternatives, which may or may not support coroutines.
 
  * aiobreaker - https://pypi.org/project/aiobreaker/
  * circuitbreaker - https://pypi.org/project/circuitbreaker/
```

### Comparing `purgatory-1.0.2/pyproject.toml` & `purgatory-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -12,50 +12,51 @@
 homepage = "https://github.com/mardiros/purgatory"
 license = "BSD-derived"
 name = "purgatory"
 packages = [
   {include = "purgatory", from = "src"},
 ]
 readme = "README.rst"
-version = "1.0.2"
+version = "1.0.3"
 
 [tool.pyright]
 include = ["src"]
 typeCheckingMode = "strict"
 
 [[tool.mypy.overrides]]
 module = "purgatory.*"
 disallow_untyped_defs = true
 disallow_any_generics = true
 
 [tool.poetry.dependencies]
 python = "^3.7"
-redis = {version = "^4.2.0", optional = true}
+redis = {version = "^4.6.0", optional = true}
 
 [tool.poetry.extras]
 aioredis = ["redis"]  # kept for compat
 redis = ["redis"]
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 coverage = {version = "^6.2", extras = ["toml"]}
 flake8 = "^5.0.4"
+furo = "^2022"
 isort = "^5.10.1"
 pytest = "^7.1.3"
-pytest-asyncio = "^0.20.1"
-pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.1"
+pytest-cov = "^4.1.0"
 Sphinx = "^4.3.2"
-sphinx-rtd-theme = "^1.0.0"
-tomlkit = "^0.11.0"
+sphinx-autodoc-typehints = "^1.12.0"
+tomlkit = "^0.12.1"
 unasync = "^0.5.0"
-redis = "^4.2.0"
-mypy = "^1.2"
-typing-extensions = "^4.4.0"
-types-redis = "^4.3.21"
-types-setuptools = "^65.5.0"
+redis = "^4.6.0"
+mypy = "^1.4.1"
+typing-extensions = "^4.7.1"
+types-redis = "^4.6.0"
+types-setuptools = "^68.0.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.coverage.report]
 exclude_lines = [
   "except ImportError:",
```

### Comparing `purgatory-1.0.2/src/purgatory/__init__.py` & `purgatory-1.0.3/src/purgatory/__init__.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/domain/messages/events.py` & `purgatory-1.0.3/src/purgatory/domain/messages/events.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/domain/model.py` & `purgatory-1.0.3/src/purgatory/domain/model.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_async/circuitbreaker.py` & `purgatory-1.0.3/src/purgatory/service/_async/circuitbreaker.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_async/message_handlers.py` & `purgatory-1.0.3/src/purgatory/service/_async/message_handlers.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_async/messagebus.py` & `purgatory-1.0.3/src/purgatory/service/_async/messagebus.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_async/repository.py` & `purgatory-1.0.3/src/purgatory/service/_async/repository.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_async/unit_of_work.py` & `purgatory-1.0.3/src/purgatory/service/_async/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_sync/circuitbreaker.py` & `purgatory-1.0.3/src/purgatory/service/_sync/circuitbreaker.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_sync/message_handlers.py` & `purgatory-1.0.3/src/purgatory/service/_sync/message_handlers.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_sync/messagebus.py` & `purgatory-1.0.3/src/purgatory/service/_sync/messagebus.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_sync/repository.py` & `purgatory-1.0.3/src/purgatory/service/_sync/repository.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/_sync/unit_of_work.py` & `purgatory-1.0.3/src/purgatory/service/_sync/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/src/purgatory/service/typing.py` & `purgatory-1.0.3/src/purgatory/service/typing.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.2/PKG-INFO` & `purgatory-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: purgatory
-Version: 1.0.2
+Version: 1.0.3
 Summary: A circuit breaker implementation for asyncio
 Home-page: https://github.com/mardiros/purgatory
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -18,23 +18,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: aioredis
 Provides-Extra: redis
-Requires-Dist: redis (>=4.2.0,<5.0.0) ; extra == "aioredis" or extra == "redis"
+Requires-Dist: redis (>=4.6.0,<5.0.0) ; extra == "aioredis" or extra == "redis"
 Description-Content-Type: text/x-rst
 
 Purgatory
 =========
 
-.. image:: https://readthedocs.org/projects/purgatory/badge/?version=latest
-   :target: https://purgatory.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
+.. image:: https://github.com/mardiros/purgatory/actions/workflows/gh-pages.yml/badge.svg
+   :target: https://mardiros.github.io/purgatory/
+   :alt: Documentation
 
 .. image:: https://github.com/mardiros/purgatory/actions/workflows/main.yml/badge.svg
    :target: https://github.com/mardiros/purgatory/actions/workflows/main.yml
    :alt: Continuous Integration Status
 
 .. image:: https://codecov.io/gh/mardiros/purgatory/branch/main/graph/badge.svg?token=LFVOQC2C9E
    :target: https://codecov.io/gh/mardiros/purgatory
@@ -56,15 +56,15 @@
 --------------------------------------------
 
 The Purgatory library has been develop to be used in `blacksmith`_ where
 the library aiobreaker was used but I encountered limitation so, I decide
 to build my own implementation that feet well with `blacksmith`_.
 
 
-.. _`blacksmith`: https://python-blacksmith.readthedocs.io/en/latest/
+.. _`blacksmith`: https://mardiros.github.io/blacksmith/
 
 
 Features
 --------
 
 Purgatory supports the creation of many circuit breakers easily, that 
 can be used as context manager or decorator.
@@ -121,17 +121,22 @@
 
 
 Read More
 ---------
 
 You can read the `full documentation of this library here`_.
 
-.. _`full documentation of this library here`: https://purgatory.readthedocs.io/en/latest/user/introduction.html
+.. _`full documentation of this library here`: https://mardiros.github.io/purgatory/user/introduction.html
 
 
+.. important::
+
+   | The documentation has been moved to github pages.
+   | The documentation under readthedocs is obsolete. 
+
 Alternatives
 ------------
 
 Here is a list of alternatives, which may or may not support coroutines.
 
  * aiobreaker - https://pypi.org/project/aiobreaker/
  * circuitbreaker - https://pypi.org/project/circuitbreaker/
```

