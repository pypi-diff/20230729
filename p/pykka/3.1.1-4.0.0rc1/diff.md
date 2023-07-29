# Comparing `tmp/pykka-3.1.1.tar.gz` & `tmp/pykka-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykka-3.1.1.tar", max compression
+gzip compressed data, was "pykka-4.0.0rc1.tar", max compression
```

## Comparing `pykka-3.1.1.tar` & `pykka-4.0.0rc1.tar`

### file list

```diff
@@ -1,71 +1,66 @@
--rw-r--r--   0        0        0    11358 2022-05-27 22:21:34.897569 pykka-3.1.1/LICENSE
--rw-r--r--   0        0        0     1553 2022-05-27 22:21:34.897569 pykka-3.1.1/README.md
--rw-r--r--   0        0        0     4572 2022-05-27 22:21:34.897569 pykka-3.1.1/docs/Makefile
--rw-r--r--   0        0        0        0 2022-05-27 22:21:34.897569 pykka-3.1.1/docs/_build/.gitignore
--rw-r--r--   0        0        0      108 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/actors.rst
--rw-r--r--   0        0        0     3752 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/debug.rst
--rw-r--r--   0        0        0      108 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/exceptions.rst
--rw-r--r--   0        0        0      100 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/futures.rst
--rw-r--r--   0        0        0     3132 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/logging.rst
--rw-r--r--   0        0        0      100 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/messages.rst
--rw-r--r--   0        0        0      132 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/module.rst
--rw-r--r--   0        0        0      188 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/proxies.rst
--rw-r--r--   0        0        0       77 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/api/registry.rst
--rw-r--r--   0        0        0      755 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/conf.py
--rw-r--r--   0        0        0     4515 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/examples.rst
--rw-r--r--   0        0        0     1969 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/index.rst
--rw-r--r--   0        0        0    10111 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/quickstart.rst
--rw-r--r--   0        0        0       57 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/requirements.txt
--rw-r--r--   0        0        0      534 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/runtimes/index.rst
--rw-r--r--   0        0        0      279 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/runtimes/threading.rst
--rw-r--r--   0        0        0     1244 2022-05-27 22:21:34.901569 pykka-3.1.1/docs/testing.rst
--rwxr-xr-x   0        0        0      631 2022-05-27 22:21:34.901569 pykka-3.1.1/examples/counter.py
--rwxr-xr-x   0        0        0     1269 2022-05-27 22:21:34.901569 pykka-3.1.1/examples/deadlock_debugging.py
--rwxr-xr-x   0        0        0      563 2022-05-27 22:21:34.901569 pykka-3.1.1/examples/plain_actor.py
--rw-r--r--   0        0        0      260 2022-05-27 22:21:34.901569 pykka-3.1.1/examples/producer.py
--rw-r--r--   0        0        0      828 2022-05-27 22:21:34.901569 pykka-3.1.1/examples/producer_test.py
--rwxr-xr-x   0        0        0     1311 2022-05-27 22:21:34.901569 pykka-3.1.1/examples/resolver.py
--rwxr-xr-x   0        0        0     1437 2022-05-27 22:21:34.901569 pykka-3.1.1/examples/typed_actor.py
--rw-r--r--   0        0        0     1616 2022-05-27 22:21:34.901569 pykka-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     1115 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/__init__.py
--rw-r--r--   0        0        0    11878 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_actor.py
--rw-r--r--   0        0        0     1627 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_actor.pyi
--rw-r--r--   0        0        0      629 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_envelope.py
--rw-r--r--   0        0        0      192 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_envelope.pyi
--rw-r--r--   0        0        0      244 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_exceptions.py
--rw-r--r--   0        0        0     8543 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_future.py
--rw-r--r--   0        0        0     1199 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_future.pyi
--rw-r--r--   0        0        0    11792 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_proxy.py
--rw-r--r--   0        0        0     1574 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_proxy.pyi
--rw-r--r--   0        0        0     5380 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_ref.py
--rw-r--r--   0        0        0     1386 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_ref.pyi
--rw-r--r--   0        0        0     5159 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_registry.py
--rw-r--r--   0        0        0     1407 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_registry.pyi
--rw-r--r--   0        0        0     3526 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_threading.py
--rw-r--r--   0        0        0      429 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_threading.pyi
--rw-r--r--   0        0        0      256 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/_types.py
--rw-r--r--   0        0        0     2181 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/debug.py
--rw-r--r--   0        0        0       90 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/debug.pyi
--rw-r--r--   0        0        0     1801 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/messages.py
--rw-r--r--   0        0        0        0 2022-05-27 22:21:34.901569 pykka-3.1.1/src/pykka/py.typed
--rw-r--r--   0        0        0        0 2022-05-27 22:21:34.901569 pykka-3.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3286 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1313 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/log_handler.py
--rw-r--r--   0        0        0     1387 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/performance.py
--rw-r--r--   0        0        0        0 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/proxy/__init__.py
--rw-r--r--   0        0        0     2246 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/proxy/test_attribute_access.py
--rw-r--r--   0        0        0     1231 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/proxy/test_dynamic_method_calls.py
--rw-r--r--   0        0        0     2203 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/proxy/test_mocking.py
--rw-r--r--   0        0        0     3658 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/proxy/test_proxy.py
--rw-r--r--   0        0        0     3014 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/proxy/test_static_method_calls.py
--rw-r--r--   0        0        0     2806 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/proxy/test_traversable.py
--rw-r--r--   0        0        0     7581 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_actor.py
--rw-r--r--   0        0        0      188 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_envelope.py
--rw-r--r--   0        0        0     6910 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_future.py
--rw-r--r--   0        0        0     4858 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_logging.py
--rw-r--r--   0        0        0      869 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_messages.py
--rw-r--r--   0        0        0     3690 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_ref.py
--rw-r--r--   0        0        0     5406 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_registry.py
--rw-r--r--   0        0        0     1263 2022-05-27 22:21:34.905569 pykka-3.1.1/tests/test_threading_actor.py
--rw-r--r--   0        0        0     2352 2022-05-27 22:24:53.655977 pykka-3.1.1/setup.py
--rw-r--r--   0        0        0     2547 2022-05-27 22:24:53.656321 pykka-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     1582 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/README.md
+-rw-r--r--   0        0        0     4572 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/Makefile
+-rw-r--r--   0        0        0        0 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/_build/.gitignore
+-rw-r--r--   0        0        0      108 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/actors.rst
+-rw-r--r--   0        0        0     3752 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/debug.rst
+-rw-r--r--   0        0        0      108 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/exceptions.rst
+-rw-r--r--   0        0        0      100 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/futures.rst
+-rw-r--r--   0        0        0     3132 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/logging.rst
+-rw-r--r--   0        0        0      100 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/messages.rst
+-rw-r--r--   0        0        0      132 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/module.rst
+-rw-r--r--   0        0        0      188 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/proxies.rst
+-rw-r--r--   0        0        0       77 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/registry.rst
+-rw-r--r--   0        0        0      176 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/api/typing.rst
+-rw-r--r--   0        0        0      786 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/conf.py
+-rw-r--r--   0        0        0     4515 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/examples.rst
+-rw-r--r--   0        0        0     1984 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/index.rst
+-rw-r--r--   0        0        0    10111 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/quickstart.rst
+-rw-r--r--   0        0        0      534 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/runtimes/index.rst
+-rw-r--r--   0        0        0      279 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/runtimes/threading.rst
+-rw-r--r--   0        0        0     1244 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/docs/testing.rst
+-rwxr-xr-x   0        0        0      631 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/examples/counter.py
+-rwxr-xr-x   0        0        0     1269 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/examples/deadlock_debugging.py
+-rwxr-xr-x   0        0        0      565 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/examples/plain_actor.py
+-rw-r--r--   0        0        0      260 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/examples/producer.py
+-rw-r--r--   0        0        0      833 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/examples/producer_test.py
+-rwxr-xr-x   0        0        0     1310 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/examples/resolver.py
+-rwxr-xr-x   0        0        0     1437 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/examples/typed_actor.py
+-rw-r--r--   0        0        0     3974 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1076 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/__init__.py
+-rw-r--r--   0        0        0    12510 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/_actor.py
+-rw-r--r--   0        0        0      902 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/_envelope.py
+-rw-r--r--   0        0        0      238 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/_exceptions.py
+-rw-r--r--   0        0        0     9689 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/_future.py
+-rw-r--r--   0        0        0     2720 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/_introspection.py
+-rw-r--r--   0        0        0    10925 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/_proxy.py
+-rw-r--r--   0        0        0     7082 2023-07-29 16:29:41.081338 pykka-4.0.0rc1/src/pykka/_ref.py
+-rw-r--r--   0        0        0     6364 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/src/pykka/_registry.py
+-rw-r--r--   0        0        0     4063 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/src/pykka/_threading.py
+-rw-r--r--   0        0        0      411 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/src/pykka/_types.py
+-rw-r--r--   0        0        0     2256 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/src/pykka/debug.py
+-rw-r--r--   0        0        0     1916 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/src/pykka/messages.py
+-rw-r--r--   0        0        0        0 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/src/pykka/py.typed
+-rw-r--r--   0        0        0     2920 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/src/pykka/typing.py
+-rw-r--r--   0        0        0        0 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     3831 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     1804 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/log_handler.py
+-rw-r--r--   0        0        0     1559 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/performance.py
+-rw-r--r--   0        0        0        0 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/__init__.py
+-rw-r--r--   0        0        0     3122 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/test_attribute_access.py
+-rw-r--r--   0        0        0     1829 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/test_dynamic_method_calls.py
+-rw-r--r--   0        0        0     2859 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/test_mocking.py
+-rw-r--r--   0        0        0     4855 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/test_proxy.py
+-rw-r--r--   0        0        0     4008 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/test_static_method_calls.py
+-rw-r--r--   0        0        0     3477 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/test_traversable.py
+-rw-r--r--   0        0        0     1632 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/proxy/test_typed_proxy.py
+-rw-r--r--   0        0        0     8837 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_actor.py
+-rw-r--r--   0        0        0      237 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_envelope.py
+-rw-r--r--   0        0        0     8224 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_future.py
+-rw-r--r--   0        0        0     6218 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_logging.py
+-rw-r--r--   0        0        0      903 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_messages.py
+-rw-r--r--   0        0        0     5013 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_ref.py
+-rw-r--r--   0        0        0     7139 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_registry.py
+-rw-r--r--   0        0        0     1576 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/test_threading_actor.py
+-rw-r--r--   0        0        0      802 2023-07-29 16:29:41.085338 pykka-4.0.0rc1/tests/types.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 pykka-4.0.0rc1/PKG-INFO
```

### Comparing `pykka-3.1.1/LICENSE` & `pykka-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/README.md` & `pykka-4.0.0rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # &#x1F300; Pykka
 
 _Pykka makes it easier to build concurrent applications._
 
-[![CI](https://img.shields.io/github/workflow/status/jodal/pykka/CI)](https://github.com/jodal/pykka/actions?workflow=CI)
+[![CI](https://img.shields.io/github/actions/workflow/status/jodal/pykka/ci.yml?branch=main)](https://github.com/jodal/pykka/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/pykka)](https://pykka.readthedocs.io/en/latest/)
 [![Coverage](https://img.shields.io/codecov/c/gh/jodal/pykka)](https://codecov.io/gh/jodal/pykka)
 [![PyPI](https://img.shields.io/pypi/v/pykka)](https://pypi.org/project/pykka/)
 
 ---
 
 Pykka is a Python implementation of the
@@ -16,15 +16,15 @@
 which makes it easier to build concurrent applications.
 
 For a quickstart guide and a complete API reference,
 see the [documentation](https://pykka.readthedocs.io/).
 
 ## Installation
 
-Pykka requires Python 3.7 or newer.
+Pykka requires Python 3.8 or newer.
 
 Pykka is available from [PyPI](https://pypi.org/project/pykka/):
 
 ```
 python3 -m pip install pykka
 ```
 
@@ -35,10 +35,10 @@
 - [Releases](https://github.com/jodal/pykka/releases)
 - [Issue tracker](https://github.com/jodal/pykka/issues)
 - [Contributors](https://github.com/jodal/pykka/graphs/contributors)
 - [Users](https://github.com/jodal/pykka/wiki/Users)
 
 ## License
 
-Pykka is copyright 2010-2022 Stein Magnus Jodal and contributors.
+Pykka is copyright 2010-2023 Stein Magnus Jodal and contributors.
 Pykka is licensed under the
 [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
```

### Comparing `pykka-3.1.1/docs/Makefile` & `pykka-4.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/docs/api/debug.rst` & `pykka-4.0.0rc1/docs/api/debug.rst`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/docs/api/logging.rst` & `pykka-4.0.0rc1/docs/api/logging.rst`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/docs/examples.rst` & `pykka-4.0.0rc1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/docs/index.rst` & `pykka-4.0.0rc1/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 For details and code examples, see the `Pykka documentation
 <https://pykka.readthedocs.io/>`_.
 
 Pykka is available from PyPI. To install it, run::
 
     pip install pykka
 
-Pykka works with Python 3.7 or newer.
+Pykka works with Python 3.8 or newer.
 
 
 Inpiration
 ==========
 
 Much of the naming of concepts and methods in Pykka is taken from the `Akka
 <https://akka.io/>`_ project which implements actors on the JVM. Though, Pykka
@@ -64,15 +64,16 @@
     api/proxies
     api/futures
     api/registry
     api/exceptions
     api/messages
     api/logging
     api/debug
+    api/typing
 
 
 License
 =======
 
-Pykka is copyright 2010-2022 Stein Magnus Jodal and contributors.
+Pykka is copyright 2010-2023 Stein Magnus Jodal and contributors.
 Pykka is licensed under the
 `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_.
```

### Comparing `pykka-3.1.1/docs/quickstart.rst` & `pykka-4.0.0rc1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/docs/runtimes/index.rst` & `pykka-4.0.0rc1/docs/runtimes/index.rst`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/docs/testing.rst` & `pykka-4.0.0rc1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/examples/counter.py` & `pykka-4.0.0rc1/examples/counter.py`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/examples/deadlock_debugging.py` & `pykka-4.0.0rc1/examples/deadlock_debugging.py`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/examples/plain_actor.py` & `pykka-4.0.0rc1/examples/plain_actor.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     def __init__(self):
         super().__init__()
         self.stored_messages = []
 
     def on_receive(self, message):
         if message is GetMessages:
             return self.stored_messages
-        else:
-            self.stored_messages.append(message)
+        self.stored_messages.append(message)
+        return None
 
 
 if __name__ == "__main__":
     actor = PlainActor.start()
     actor.tell({"no": "Norway", "se": "Sweden"})
     actor.tell({"a": 3, "b": 4, "c": 5})
     print(actor.ask(GetMessages))
```

### Comparing `pykka-3.1.1/examples/producer_test.py` & `pykka-4.0.0rc1/examples/producer_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 from producer import ProducerActor
 
 
-@pytest.fixture
+@pytest.fixture()
 def consumer_mock(mocker):
-    yield mocker.Mock()
+    return mocker.Mock()
 
 
-@pytest.fixture
+@pytest.fixture()
 def producer(consumer_mock):
     # Step 1: The actor under test is wired up with
     # its dependencies and is started.
     proxy = ProducerActor.start(consumer_mock).proxy()
 
     yield proxy
```

### Comparing `pykka-3.1.1/examples/resolver.py` & `pykka-4.0.0rc1/examples/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 
-"""
-Resolve a bunch of IP addresses using a pool of resolver actors.
+"""Resolve a bunch of IP addresses using a pool of resolver actors.
 
 Based on example contributed by Kristian Klette <klette@klette.us>.
 
 Either run without arguments:
 
     ./resolver.py
```

### Comparing `pykka-3.1.1/examples/typed_actor.py` & `pykka-4.0.0rc1/examples/typed_actor.py`

 * *Files identical despite different names*

### Comparing `pykka-3.1.1/src/pykka/__init__.py` & `pykka-4.0.0rc1/src/pykka/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
+"""Pykka is a Python implementation of the actor model."""
+
+import importlib.metadata as _importlib_metadata
 import logging as _logging
 
 from pykka._exceptions import ActorDeadError, Timeout
 from pykka._future import Future, get_all
 from pykka._proxy import ActorProxy, CallableProxy, traversable
 from pykka._ref import ActorRef
 from pykka._registry import ActorRegistry
 
 # The following must be imported late, in this specific order.
 from pykka._actor import Actor  # isort:skip
 from pykka._threading import ThreadingActor, ThreadingFuture  # isort:skip
 
-try:
-    import importlib.metadata as _importlib_metadata
-except ImportError:
-    import importlib_metadata as _importlib_metadata  # type: ignore
-
 
 __all__ = [
     "Actor",
     "ActorDeadError",
     "ActorProxy",
     "ActorRef",
     "ActorRegistry",
```

### Comparing `pykka-3.1.1/src/pykka/_actor.py` & `pykka-4.0.0rc1/src/pykka/_actor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,47 @@
+from __future__ import annotations
+
 import logging
 import sys
 import threading
 import uuid
+from typing import TYPE_CHECKING, Any, Optional, Protocol, TypeVar
 
 from pykka import ActorDeadError, ActorRef, ActorRegistry, messages
+from pykka._introspection import get_attr_directly
+
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from pykka import Future
+    from pykka._envelope import Envelope
 
 __all__ = ["Actor"]
 
+
 logger = logging.getLogger("pykka")
 
 
+A = TypeVar("A", bound="Actor")
+
+
+class ActorInbox(Protocol):
+    def put(self, envelope: Envelope[Any], /) -> None:
+        ...
+
+    def get(self) -> Envelope[Any]:
+        ...
+
+    def empty(self) -> bool:
+        ...
+
+
 class Actor:
-    """
+    """An actor is an execution unit that executes concurrently with other actors.
+
     To create an actor:
 
     1. subclass one of the :class:`Actor` implementations:
 
        - :class:`~pykka.ThreadingActor`
 
     2. implement your methods, including :meth:`__init__`, as usual,
@@ -49,17 +75,22 @@
                 ... # My regular method to be used through an ActorProxy
 
         my_actor_ref = MyActor.start(my_arg=...)
         my_actor_ref.stop()
     """
 
     @classmethod
-    def start(cls, *args, **kwargs):
-        """
-        Start an actor and register it in the
+    def start(
+        cls: type[A],
+        *args: Any,
+        **kwargs: Any,
+    ) -> ActorRef[A]:
+        """Start an actor.
+
+        Starting an actor also registers it in the
         :class:`ActorRegistry <pykka.ActorRegistry>`.
 
         Any arguments passed to :meth:`start` will be passed on to the class
         constructor.
 
         Behind the scenes, the following is happening when you call
         :meth:`start`:
@@ -86,49 +117,68 @@
         obj = cls(*args, **kwargs)
         assert obj.actor_ref is not None, (
             "Actor.__init__() have not been called. "
             "Did you forget to call super() in your override?"
         )
         ActorRegistry.register(obj.actor_ref)
         logger.debug(f"Starting {obj}")
-        obj._start_actor_loop()
+        obj._start_actor_loop()  # noqa: SLF001
         return obj.actor_ref
 
     @staticmethod
-    def _create_actor_inbox():
-        """Internal method for implementors of new actor types."""
+    def _create_actor_inbox() -> ActorInbox:
+        """Create an inbox for the actor.
+
+        Internal method for implementors of new actor types.
+        """
         raise NotImplementedError("Use a subclass of Actor")
 
     @staticmethod
-    def _create_future():
-        """Internal method for implementors of new actor types."""
+    def _create_future() -> Future[Any]:
+        """Create a future for the actor.
+
+        Internal method for implementors of new actor types.
+        """
         raise NotImplementedError("Use a subclass of Actor")
 
-    def _start_actor_loop(self):
-        """Internal method for implementors of new actor types."""
+    def _start_actor_loop(self) -> None:
+        """Create and start the actor's event loop.
+
+        Internal method for implementors of new actor types.
+        """
         raise NotImplementedError("Use a subclass of Actor")
 
     #: The actor URN string is a universally unique identifier for the actor.
     #: It may be used for looking up a specific actor using
     #: :meth:`ActorRegistry.get_by_urn`.
-    actor_urn = None
+    actor_urn: str
 
     #: The actor's inbox. Use :meth:`ActorRef.tell`, :meth:`ActorRef.ask`, and
     #: friends to put messages in the inbox.
-    actor_inbox = None
+    actor_inbox: ActorInbox
 
-    #: The actor's :class:`ActorRef` instance.
-    actor_ref = None
+    _actor_ref: ActorRef[Any]
+
+    @property
+    def actor_ref(self: A) -> ActorRef[A]:
+        """The actor's :class:`ActorRef` instance."""
+        # This property only exists to improve the typing of the ActorRef.
+        return self._actor_ref
 
     #: A :class:`threading.Event` representing whether or not the actor should
     #: continue processing messages. Use :meth:`stop` to change it.
-    actor_stopped = None
+    actor_stopped: threading.Event
+
+    def __init__(
+        self,
+        *_args: Any,
+        **_kwargs: Any,
+    ) -> None:
+        """Create actor.
 
-    def __init__(self, *args, **kwargs):
-        """
         Your are free to override :meth:`__init__`, but you must call your
         superclass' :meth:`__init__` to ensure that fields :attr:`actor_urn`,
         :attr:`actor_inbox`, and :attr:`actor_ref` are initialized.
 
         You can use :func:`super`::
 
             super().__init__()
@@ -140,50 +190,52 @@
         :meth:`__init__` is called before the actor is started and registered
         in :class:`ActorRegistry <pykka.ActorRegistry>`.
         """
         self.actor_urn = uuid.uuid4().urn
         self.actor_inbox = self._create_actor_inbox()
         self.actor_stopped = threading.Event()
 
-        self.actor_ref = ActorRef(self)
+        self._actor_ref = ActorRef(self)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.__class__.__name__} ({self.actor_urn})"
 
-    def stop(self):
-        """
-        Stop the actor.
+    def stop(self) -> None:
+        """Stop the actor.
 
         It's equivalent to calling :meth:`ActorRef.stop` with ``block=False``.
         """
-        self.actor_ref.tell(messages._ActorStop())
+        self.actor_ref.tell(messages._ActorStop())  # noqa: SLF001
 
-    def _stop(self):
-        """
-        Stops the actor immediately without processing the rest of the inbox.
-        """
+    def _stop(self) -> None:
+        """Stop the actor immediately without processing the rest of the inbox."""
         ActorRegistry.unregister(self.actor_ref)
         self.actor_stopped.set()
         logger.debug(f"Stopped {self}")
         try:
             self.on_stop()
         except Exception:
             self._handle_failure(*sys.exc_info())
 
-    def _actor_loop(self):
-        """
-        The actor's event loop.
+    def _actor_loop(self) -> None:
+        """Run the actor's core loop.
 
         This is the method that will be executed by the thread or greenlet.
         """
+        self._actor_loop_setup()
+        self._actor_loop_running()
+        self._actor_loop_teardown()
+
+    def _actor_loop_setup(self) -> None:
         try:
             self.on_start()
         except Exception:
             self._handle_failure(*sys.exc_info())
 
+    def _actor_loop_running(self) -> None:
         while not self.actor_stopped.is_set():
             envelope = self.actor_inbox.get()
             try:
                 response = self._handle_receive(envelope.message)
                 if envelope.reply_to is not None:
                     envelope.reply_to.set(response)
             except Exception:
@@ -201,140 +253,115 @@
                         self._handle_failure(*sys.exc_info())
             except BaseException:
                 exception_value = sys.exc_info()[1]
                 logger.debug(f"{exception_value!r} in {self}. Stopping all actors.")
                 self._stop()
                 ActorRegistry.stop_all()
 
+    def _actor_loop_teardown(self) -> None:
         while not self.actor_inbox.empty():
             envelope = self.actor_inbox.get()
             if envelope.reply_to is not None:
-                if isinstance(envelope.message, messages._ActorStop):
+                if isinstance(envelope.message, messages._ActorStop):  # noqa: SLF001
                     envelope.reply_to.set(None)
                 else:
                     envelope.reply_to.set_exception(
                         exc_info=(
                             ActorDeadError,
                             ActorDeadError(
                                 f"{self.actor_ref} stopped before "
                                 f"handling the message"
                             ),
                             None,
                         )
                     )
 
-    def on_start(self):
-        """
+    def on_start(self) -> None:
+        """Run code at the beginning of the actor's life.
+
         Hook for doing any setup that should be done *after* the actor is
         started, but *before* it starts processing messages.
 
         For :class:`ThreadingActor`, this method is executed in the actor's own
         thread, while :meth:`__init__` is executed in the thread that created
         the actor.
 
         If an exception is raised by this method the stack trace will be
         logged, and the actor will stop.
         """
-        pass
 
-    def on_stop(self):
-        """
+    def on_stop(self) -> None:
+        """Run code at the end of the actor's life.
+
         Hook for doing any cleanup that should be done *after* the actor has
         processed the last message, and *before* the actor stops.
 
         This hook is *not* called when the actor stops because of an unhandled
         exception. In that case, the :meth:`on_failure` hook is called instead.
 
         For :class:`ThreadingActor` this method is executed in the actor's own
         thread, immediately before the thread exits.
 
         If an exception is raised by this method the stack trace will be
         logged, and the actor will stop.
         """
-        pass
 
-    def _handle_failure(self, exception_type, exception_value, traceback):
-        """Logs unexpected failures, unregisters and stops the actor."""
+    def _handle_failure(
+        self,
+        exception_type: Optional[type[BaseException]],
+        exception_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        """Log unexpected failures, unregisters and stops the actor."""
         logger.error(
             f"Unhandled exception in {self}:",
-            exc_info=(exception_type, exception_value, traceback),
+            exc_info=(exception_type, exception_value, traceback),  # type: ignore[arg-type]  # noqa: E501
         )
         ActorRegistry.unregister(self.actor_ref)
         self.actor_stopped.set()
 
-    def on_failure(self, exception_type, exception_value, traceback):
-        """
+    def on_failure(
+        self,
+        exception_type: Optional[type[BaseException]],
+        exception_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        """Run code when an unhandled exception is raised.
+
         Hook for doing any cleanup *after* an unhandled exception is raised,
         and *before* the actor stops.
 
         For :class:`ThreadingActor` this method is executed in the actor's own
         thread, immediately before the thread exits.
 
         The method's arguments are the relevant information from
         :func:`sys.exc_info`.
 
         If an exception is raised by this method the stack trace will be
         logged, and the actor will stop.
         """
-        pass
 
-    def _handle_receive(self, message):
-        """Handles messages sent to the actor."""
-        if isinstance(message, messages._ActorStop):
+    def _handle_receive(self, message: Any) -> Any:
+        """Handle messages sent to the actor."""
+        if isinstance(message, messages._ActorStop):  # noqa: SLF001
             return self._stop()
         if isinstance(message, messages.ProxyCall):
-            callee = self._get_attribute_from_path(message.attr_path)
+            callee = get_attr_directly(self, message.attr_path)
             return callee(*message.args, **message.kwargs)
         if isinstance(message, messages.ProxyGetAttr):
-            attr = self._get_attribute_from_path(message.attr_path)
+            attr = get_attr_directly(self, message.attr_path)
             return attr
         if isinstance(message, messages.ProxySetAttr):
-            parent_attr = self._get_attribute_from_path(message.attr_path[:-1])
+            parent_attr = get_attr_directly(self, message.attr_path[:-1])
             attr_name = message.attr_path[-1]
             return setattr(parent_attr, attr_name, message.value)
         return self.on_receive(message)
 
-    def on_receive(self, message):
-        """
-        May be implemented for the actor to handle regular non-proxy messages.
+    def on_receive(self, message: Any) -> Any:
+        """May be implemented for the actor to handle regular non-proxy messages.
 
         :param message: the message to handle
         :type message: any
 
         :returns: anything that should be sent as a reply to the sender
         """
         logger.warning(f"Unexpected message received by {self}: {message}")
-
-    def _get_attribute_from_path(self, attr_path):
-        """
-        Traverses the path and returns the attribute at the end of the path.
-        """
-        attr = self
-        for attr_name in attr_path:
-            attr = getattr(attr, attr_name)
-        return attr
-
-    def _introspect_attribute_from_path(self, attr_path):
-        """Get attribute information from ``__dict__`` on the container."""
-        if not attr_path:
-            return self
-
-        parent = self._get_attribute_from_path(attr_path[:-1])
-        parent_attrs = self._introspect_attributes(parent)
-        attr_name = attr_path[-1]
-
-        try:
-            return parent_attrs[attr_name]
-        except KeyError:
-            raise AttributeError(
-                f"type object {parent.__class__.__name__!r} "
-                f"has no attribute {attr_name!r}"
-            )
-
-    def _introspect_attributes(self, obj):
-        """Combine ``__dict__`` from ``obj`` and all its superclasses."""
-        result = {}
-        for cls in reversed(obj.__class__.mro()):
-            result.update(cls.__dict__)
-        if hasattr(obj, "__dict__"):
-            result.update(obj.__dict__)
-        return result
```

### Comparing `pykka-3.1.1/src/pykka/_future.py` & `pykka-4.0.0rc1/src/pykka/_future.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,64 @@
+from __future__ import annotations
+
 import functools
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generator,
+    Generic,
+    Iterable,
+    Optional,
+    TypeVar,
+    cast,
+)
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
+    from pykka._types import OptExcInfo
 
 __all__ = ["Future", "get_all"]
 
 
-class Future:
-    """
-    A :class:`Future` is a handle to a value which is available or will be
-    available in the future.
+T = TypeVar("T")
+J = TypeVar("J")  # For when T is Iterable[J]
+M = TypeVar("M")  # Result of Future.map()
+R = TypeVar("R")  # Result of Future.reduce()
+
+GetHookFunc: TypeAlias = Callable[[Optional[float]], T]
+
+
+class Future(Generic[T]):
+    """A handle to a value which is available now or in the future.
 
     Typically returned by calls to actor methods or accesses to actor fields.
 
     To get hold of the encapsulated value, call :meth:`Future.get` or
     ``await`` the future.
     """
 
-    def __init__(self):
+    _get_hook: Optional[GetHookFunc[T]]
+    _get_hook_result: Optional[T]
+
+    def __init__(self) -> None:
         super().__init__()
         self._get_hook = None
         self._get_hook_result = None
 
-    def get(self, timeout=None):
-        """
-        Get the value encapsulated by the future.
+    def __repr__(self) -> str:
+        return "<pykka.Future>"
+
+    def get(
+        self,
+        *,
+        timeout: Optional[float] = None,
+    ) -> T:
+        """Get the value encapsulated by the future.
 
         If the encapsulated value is an exception, it is raised instead of
         returned.
 
         If ``timeout`` is :class:`None`, as default, the method will block
         until it gets a reply, potentially forever. If ``timeout`` is an
         integer or float, the method will wait for a reply for ``timeout``
@@ -43,59 +76,67 @@
         """
         if self._get_hook is not None:
             if self._get_hook_result is None:
                 self._get_hook_result = self._get_hook(timeout)
             return self._get_hook_result
         raise NotImplementedError
 
-    def set(self, value=None):
-        """
-        Set the encapsulated value.
+    def set(
+        self,
+        value: Optional[T] = None,
+    ) -> None:
+        """Set the encapsulated value.
 
         :param value: the encapsulated value or nothing
         :type value: any object or :class:`None`
         :raise: an exception if set is called multiple times
         """
         raise NotImplementedError
 
-    def set_exception(self, exc_info=None):
-        """
-        Set an exception as the encapsulated value.
+    def set_exception(
+        self,
+        exc_info: Optional[OptExcInfo] = None,
+    ) -> None:
+        """Set an exception as the encapsulated value.
 
         You can pass an ``exc_info`` three-tuple, as returned by
         :func:`sys.exc_info`. If you don't pass ``exc_info``,
         :func:`sys.exc_info` will be called and the value returned by it used.
 
         In other words, if you're calling :meth:`set_exception`, without any
         arguments, from an except block, the exception you're currently
         handling will automatically be set on the future.
 
         :param exc_info: the encapsulated exception
         :type exc_info: three-tuple of (exc_class, exc_instance, traceback)
         """
         raise NotImplementedError
 
-    def set_get_hook(self, func):
-        """
-        Set a function to be executed when :meth:`get` is called.
+    def set_get_hook(
+        self,
+        func: GetHookFunc[T],
+    ) -> None:
+        """Set a function to be executed when :meth:`get` is called.
 
         The function will be called when :meth:`get` is called, with the
         ``timeout`` value as the only argument. The function's return value
         will be returned from :meth:`get`.
 
         .. versionadded:: 1.2
 
         :param func: called to produce return value of :meth:`get`
         :type func: function accepting a timeout value
         """
         self._get_hook = func
 
-    def filter(self, func):
-        """
-        Return a new future with only the items passing the predicate function.
+    def filter(
+        self: Future[Iterable[J]],
+        func: Callable[[J], bool],
+    ) -> Future[Iterable[J]]:
+        """Return a new future with only the items passing the predicate function.
 
         If the future's value is an iterable, :meth:`filter` will return a new
         future whose value is another iterable with only the items from the
         first iterable for which ``func(item)`` is true. If the future's value
         isn't an iterable, a :exc:`TypeError` will be raised when :meth:`get`
         is called.
 
@@ -111,20 +152,24 @@
             [5, 6, 7, 8, 9, 10, 11, 12, 13, 14]
             >>> g.get()
             [11, 12, 13, 14]
 
         .. versionadded:: 1.2
         """
         future = self.__class__()
-        future.set_get_hook(lambda timeout: list(filter(func, self.get(timeout))))
+        future.set_get_hook(
+            lambda timeout: list(filter(func, self.get(timeout=timeout)))
+        )
         return future
 
-    def join(self, *futures):
-        """
-        Return a new future with a list of the result of multiple futures.
+    def join(
+        self: Future[Any],
+        *futures: Future[Any],
+    ) -> Future[Iterable[Any]]:
+        """Return a new future with a list of the result of multiple futures.
 
         One or more futures can be passed as arguments to :meth:`join`. The new
         future returns a list with the results from all the joined futures.
 
         Example::
 
             >>> import pykka
@@ -136,24 +181,25 @@
             >>> b.set(123)
             >>> c.set(False)
             >>> f.get()
             ['def', 123, False]
 
         .. versionadded:: 1.2
         """
-        future = self.__class__()
+        future = cast(Future[Iterable[Any]], self.__class__())
         future.set_get_hook(
-            lambda timeout: [f.get(timeout) for f in [self] + list(futures)]
+            lambda timeout: [f.get(timeout=timeout) for f in [self, *futures]]
         )
         return future
 
-    def map(self, func):
-        """
-        Return a new future with the result of the future passed through a
-        function.
+    def map(
+        self,
+        func: Callable[[T], M],
+    ) -> Future[M]:
+        """Pass the result of the future through a function.
 
         Example::
 
             >>> import pykka
             >>> f = pykka.ThreadingFuture()
             >>> g = f.map(lambda x: x + 10)
             >>> f.set(30)
@@ -172,24 +218,24 @@
             Previously, if the future's result was an iterable (except a
             string), the function was applied to each item in the iterable.
             This behavior is unpredictable and makes regular use cases like
             extracting a single field from a dict difficult, thus the
             behavior has been simplified. Now, the entire result value is
             passed to the function.
         """
-        future = self.__class__()
-        future.set_get_hook(lambda timeout: func(self.get(timeout)))
+        future = cast(Future[M], self.__class__())
+        future.set_get_hook(lambda timeout: func(self.get(timeout=timeout)))
         return future
 
-    def reduce(self, func, *args):
-        """
-        reduce(func[, initial])
-
-        Return a new future with the result of reducing the future's iterable
-        into a single value.
+    def reduce(
+        self: Future[Iterable[J]],
+        func: Callable[[R, J], R],
+        *args: R,
+    ) -> Future[R]:
+        """Reduce a future's iterable result to a single value.
 
         The function of two arguments is applied cumulatively to the items of
         the iterable, from left to right. The result of the first function call
         is used as the first argument to the second function call, and so on,
         until the end of the iterable. If the future's value isn't an iterable,
         a :exc:`TypeError` is raised.
 
@@ -226,31 +272,34 @@
             >>> g = f.reduce(lambda x, y: x + y, 5)
             >>> f.set([])
             >>> g.get()
             5
 
         .. versionadded:: 1.2
         """
-        future = self.__class__()
+        future = cast(Future[R], self.__class__())
         future.set_get_hook(
-            lambda timeout: functools.reduce(func, self.get(timeout), *args)
+            lambda timeout: functools.reduce(func, self.get(timeout=timeout), *args)
         )
         return future
 
-    def __await__(self):
+    def __await__(self) -> Generator[None, None, T]:
         yield
         value = self.get()
         return value
 
     __iter__ = __await__
 
 
-def get_all(futures, timeout=None):
-    """
-    Collect all values encapsulated in the list of futures.
+def get_all(
+    futures: Iterable[Future[Any]],
+    *,
+    timeout: Optional[float] = None,
+) -> Iterable[Any]:
+    """Collect all values encapsulated in the list of futures.
 
     If ``timeout`` is not :class:`None`, the method will wait for a reply for
     ``timeout`` seconds, and then raise :exc:`pykka.Timeout`.
 
     :param futures: futures for the results to collect
     :type futures: list of :class:`pykka.Future`
```

### Comparing `pykka-3.1.1/src/pykka/_proxy.py` & `pykka-4.0.0rc1/src/pykka/_proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+from __future__ import annotations
+
 import logging
-from collections.abc import Callable
-from typing import NamedTuple
+from typing import TYPE_CHECKING, Any, Generic, Optional, TypeVar
 
 from pykka import ActorDeadError, messages
+from pykka._introspection import AttrInfo, introspect_attrs
+
+if TYPE_CHECKING:
+    from pykka import Actor, ActorRef, Future
+    from pykka._types import AttrPath
 
 __all__ = ["ActorProxy"]
 
+
 logger = logging.getLogger("pykka")
 
 
-class AttrInfo(NamedTuple):
-    callable: bool
-    traversable: bool
+T = TypeVar("T")
+A = TypeVar("A", bound="Actor")
 
 
-class ActorProxy:
-    """
-    An :class:`ActorProxy` wraps an :class:`ActorRef <pykka.ActorRef>`
-    instance. The proxy allows the referenced actor to be used through regular
+class ActorProxy(Generic[A]):
+    """An :class:`ActorProxy` wraps an :class:`ActorRef <pykka.ActorRef>` instance.
+
+    The proxy allows the referenced actor to be used through regular
     method calls and field access.
 
     You can create an :class:`ActorProxy` from any :class:`ActorRef
     <pykka.ActorRef>`::
 
         actor_ref = MyActor.start()
         actor_proxy = ActorProxy(actor_ref)
@@ -109,146 +115,113 @@
     :param actor_ref: reference to the actor to proxy
     :type actor_ref: :class:`pykka.ActorRef`
 
     :raise: :exc:`pykka.ActorDeadError` if actor is not available
     """
 
     #: The actor's :class:`pykka.ActorRef` instance.
-    actor_ref = None
+    actor_ref: ActorRef[A]
 
-    def __init__(self, actor_ref, attr_path=None):
+    _actor: A
+    _attr_path: AttrPath
+    _known_attrs: dict[AttrPath, AttrInfo]
+    _actor_proxies: dict[AttrPath, ActorProxy[A]]
+    _callable_proxies: dict[AttrPath, CallableProxy[A]]
+
+    def __init__(
+        self,
+        *,
+        actor_ref: ActorRef[A],
+        attr_path: Optional[AttrPath] = None,
+    ) -> None:
         if not actor_ref.is_alive():
             raise ActorDeadError(f"{actor_ref} not found")
         self.actor_ref = actor_ref
-        self._actor = actor_ref._actor
-        self._attr_path = attr_path or tuple()
-        self._known_attrs = self._introspect_attributes()
+        self._actor = actor_ref._actor  # noqa: SLF001
+        self._attr_path = attr_path or ()
+        self._known_attrs = introspect_attrs(root=self._actor, proxy=self)
         self._actor_proxies = {}
         self._callable_proxies = {}
 
-    def _introspect_attributes(self):
-        """Introspects the actor's attributes."""
-        result = {}
-        attr_paths_to_visit = [[attr_name] for attr_name in dir(self._actor)]
-
-        while attr_paths_to_visit:
-            attr_path = attr_paths_to_visit.pop(0)
-
-            if not self._is_exposable_attribute(attr_path[-1]):
-                continue
-
-            attr = self._actor._introspect_attribute_from_path(attr_path)
-
-            if self._is_self_proxy(attr):
-                logger.warning(
-                    f"{self._actor} attribute {'.'.join(attr_path)!r} "
-                    f"is a proxy to itself. "
-                    f"Consider making it private "
-                    f"by renaming it to {'_' + attr_path[-1]!r}."
-                )
-                continue
-
-            attr_info = AttrInfo(
-                callable=self._is_callable_attribute(attr),
-                traversable=self._is_traversable_attribute(attr),
-            )
-            result[tuple(attr_path)] = attr_info
-
-            if attr_info.traversable:
-                for attr_name in dir(attr):
-                    attr_paths_to_visit.append(attr_path + [attr_name])
-
-        return result
-
-    def _is_exposable_attribute(self, attr_name):
-        """
-        Returns true for any attribute name that may be exposed through
-        :class:`ActorProxy`.
-        """
-        return not attr_name.startswith("_")
-
-    def _is_self_proxy(self, attr):
-        """Returns true if attribute is an equivalent actor proxy."""
-        return attr == self
-
-    def _is_callable_attribute(self, attr):
-        """Returns true for any attribute that is callable."""
-        return isinstance(attr, Callable)
-
-    def _is_traversable_attribute(self, attr):
-        """
-        Returns true for any attribute that may be traversed from another
-        actor through a proxy.
-        """
-        return (
-            getattr(attr, "_pykka_traversable", False) is True
-            or getattr(attr, "pykka_traversable", False) is True
-        )
-
-    def __eq__(self, other):
+    def __eq__(
+        self,
+        other: object,
+    ) -> bool:
         if not isinstance(other, ActorProxy):
             return False
-        if self._actor != other._actor:
+        if (
+            self._actor
+            != other._actor  # noqa: SLF001  # pyright: ignore[reportUnknownMemberType]
+        ):
             return False
-        if self._attr_path != other._attr_path:
+        if self._attr_path != other._attr_path:  # noqa: SLF001
             return False
         return True
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash((self._actor, self._attr_path))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<ActorProxy for {self.actor_ref}, attr_path={self._attr_path!r}>"
 
-    def __dir__(self):
+    def __dir__(self) -> list[str]:
         result = ["__class__"]
         result += list(self.__class__.__dict__.keys())
         result += list(self.__dict__.keys())
         result += [attr_path[0] for attr_path in list(self._known_attrs.keys())]
         return sorted(result)
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> Any:
         """Get a field or callable from the actor."""
-        attr_path = self._attr_path + (name,)
+        attr_path: AttrPath = (*self._attr_path, name)
 
         if attr_path not in self._known_attrs:
-            self._known_attrs = self._introspect_attributes()
+            self._known_attrs = introspect_attrs(root=self._actor, proxy=self)
 
         attr_info = self._known_attrs.get(attr_path)
         if attr_info is None:
             raise AttributeError(f"{self} has no attribute {name!r}")
 
         if attr_info.callable:
             if attr_path not in self._callable_proxies:
                 self._callable_proxies[attr_path] = CallableProxy(
-                    self.actor_ref, attr_path
+                    actor_ref=self.actor_ref,
+                    attr_path=attr_path,
                 )
             return self._callable_proxies[attr_path]
-        elif attr_info.traversable:
+
+        if attr_info.traversable:
             if attr_path not in self._actor_proxies:
-                self._actor_proxies[attr_path] = ActorProxy(self.actor_ref, attr_path)
+                self._actor_proxies[attr_path] = ActorProxy(
+                    actor_ref=self.actor_ref,
+                    attr_path=attr_path,
+                )
             return self._actor_proxies[attr_path]
-        else:
-            message = messages.ProxyGetAttr(attr_path=attr_path)
-            return self.actor_ref.ask(message, block=False)
 
-    def __setattr__(self, name, value):
-        """
-        Set a field on the actor.
+        message = messages.ProxyGetAttr(attr_path=attr_path)
+        return self.actor_ref.ask(message, block=False)
+
+    def __setattr__(
+        self,
+        name: str,
+        value: Any,
+    ) -> None:
+        """Set a field on the actor.
 
         Blocks until the field is set to check if any exceptions was raised.
         """
         if name == "actor_ref" or name.startswith("_"):
             return super().__setattr__(name, value)
-        attr_path = self._attr_path + (name,)
+        attr_path = (*self._attr_path, name)
         message = messages.ProxySetAttr(attr_path=attr_path, value=value)
         self.actor_ref.ask(message)
+        return None
 
 
-class CallableProxy:
+class CallableProxy(Generic[A]):
     """Proxy to a single method.
 
     :class:`CallableProxy` instances are returned when accessing methods on a
     :class:`ActorProxy` without calling them.
 
     Example::
 
@@ -257,34 +230,50 @@
         # Ask semantics returns a future. See `__call__()` docs.
         future = proxy.do_work()
 
         # Tell semantics are fire and forget. See `defer()` docs.
         proxy.do_work.defer()
     """
 
-    def __init__(self, actor_ref, attr_path):
+    actor_ref: ActorRef[A]
+    _attr_path: AttrPath
+
+    def __init__(
+        self,
+        *,
+        actor_ref: ActorRef[A],
+        attr_path: AttrPath,
+    ) -> None:
         self.actor_ref = actor_ref
         self._attr_path = attr_path
 
-    def __call__(self, *args, **kwargs):
+    def __call__(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Future[Any]:
         """Call with :meth:`~pykka.ActorRef.ask` semantics.
 
         Returns a future which will yield the called method's return value.
 
         If the call raises an exception is set on the future, and will be
         reraised by :meth:`~pykka.Future.get`. If the future is left unused,
         the exception will not be reraised. Either way, the exception will
         also be logged. See :ref:`logging` for details.
         """
         message = messages.ProxyCall(
             attr_path=self._attr_path, args=args, kwargs=kwargs
         )
         return self.actor_ref.ask(message, block=False)
 
-    def defer(self, *args, **kwargs):
+    def defer(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         """Call with :meth:`~pykka.ActorRef.tell` semantics.
 
         Does not create or return a future.
 
         If the call raises an exception, there is no future to set the
         exception on. Thus, the actor's :meth:`~pykka.Actor.on_failure` hook
         is called instead.
@@ -293,16 +282,16 @@
         """
         message = messages.ProxyCall(
             attr_path=self._attr_path, args=args, kwargs=kwargs
         )
         self.actor_ref.tell(message)
 
 
-def traversable(obj):
-    """Marks an actor attribute as traversable.
+def traversable(obj: T) -> T:
+    """Mark an actor attribute as traversable.
 
     The traversable marker makes the actor attribute's own methods and
     attributes available to users of the actor through an
     :class:`~pykka.ActorProxy`.
 
     Used as a function to mark a single attribute::
 
@@ -342,13 +331,13 @@
 
         proxy = AnActor.start().proxy()
         assert proxy.playback.play().get() is True
 
     .. versionadded:: 2.0
     """
     if hasattr(obj, "__slots__"):
-        raise Exception(
+        raise ValueError(
             "pykka.traversable() cannot be used to mark "
             "an object using slots as traversable."
         )
-    obj._pykka_traversable = True
+    obj._pykka_traversable = True  # type: ignore[attr-defined]  # noqa: SLF001
     return obj
```

### Comparing `pykka-3.1.1/src/pykka/_registry.py` & `pykka-4.0.0rc1/src/pykka/_registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,50 @@
+from __future__ import annotations
+
 import logging
 import threading
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    ClassVar,
+    Literal,
+    Optional,
+    TypeVar,
+    Union,
+    overload,
+)
+
+if TYPE_CHECKING:
+    from pykka import Actor, ActorRef, Future
+
+__all__ = ["ActorRegistry"]
+
 
 logger = logging.getLogger("pykka")
 
 
-__all__ = ["ActorRegistry"]
+A = TypeVar("A", bound="Actor")
 
 
 class ActorRegistry:
-    """
-    Registry which provides easy access to all running actors.
+    """Registry which provides easy access to all running actors.
 
     Contains global state, but should be thread-safe.
     """
 
-    _actor_refs = []
-    _actor_refs_lock = threading.RLock()
+    _actor_refs: ClassVar[list[ActorRef[Any]]] = []
+    _actor_refs_lock: ClassVar[threading.RLock] = threading.RLock()
 
     @classmethod
-    def broadcast(cls, message, target_class=None):
-        """
-        Broadcast ``message`` to all actors of the specified ``target_class``.
+    def broadcast(
+        cls,
+        message: Any,
+        target_class: Union[str, type[Actor], None] = None,
+    ) -> None:
+        """Broadcast ``message`` to all actors of the specified ``target_class``.
 
         If no ``target_class`` is specified, the message is broadcasted to all
         actors.
 
         :param message: the message to send
         :type message: any
 
@@ -37,93 +57,133 @@
             targets = cls.get_by_class(target_class)
         else:
             targets = cls.get_all()
         for ref in targets:
             ref.tell(message)
 
     @classmethod
-    def get_all(cls):
-        """
-        Get :class:`ActorRef <pykka.ActorRef>` for all running actors.
+    def get_all(cls) -> list[ActorRef[Any]]:
+        """Get all running actors.
 
         :returns: list of :class:`pykka.ActorRef`
         """
         with cls._actor_refs_lock:
             return cls._actor_refs[:]
 
     @classmethod
-    def get_by_class(cls, actor_class):
-        """
-        Get :class:`ActorRef` for all running actors of the given class, or of
-        any subclass of the given class.
+    def get_by_class(
+        cls,
+        actor_class: type[A],
+    ) -> list[ActorRef[A]]:
+        """Get all running actors of the given class or a subclass.
 
         :param actor_class: actor class, or any superclass of the actor
         :type actor_class: class
 
         :returns: list of :class:`pykka.ActorRef`
         """
         with cls._actor_refs_lock:
             return [
                 ref
                 for ref in cls._actor_refs
                 if issubclass(ref.actor_class, actor_class)
             ]
 
     @classmethod
-    def get_by_class_name(cls, actor_class_name):
-        """
-        Get :class:`ActorRef` for all running actors of the given class
-        name.
+    def get_by_class_name(
+        cls,
+        actor_class_name: str,
+    ) -> list[ActorRef[Any]]:
+        """Get all running actors of the given class name.
 
         :param actor_class_name: actor class name
         :type actor_class_name: string
 
         :returns: list of :class:`pykka.ActorRef`
         """
         with cls._actor_refs_lock:
             return [
                 ref
                 for ref in cls._actor_refs
                 if ref.actor_class.__name__ == actor_class_name
             ]
 
     @classmethod
-    def get_by_urn(cls, actor_urn):
-        """
-        Get an actor by its universally unique URN.
+    def get_by_urn(
+        cls,
+        actor_urn: str,
+    ) -> Optional[ActorRef[Any]]:
+        """Get an actor by its universally unique URN.
 
         :param actor_urn: actor URN
         :type actor_urn: string
 
         :returns: :class:`pykka.ActorRef` or :class:`None` if not found
         """
         with cls._actor_refs_lock:
             refs = [ref for ref in cls._actor_refs if ref.actor_urn == actor_urn]
-            if refs:
-                return refs[0]
+            if not refs:
+                return None
+            return refs[0]
 
     @classmethod
-    def register(cls, actor_ref):
-        """
-        Register an :class:`ActorRef` in the registry.
+    def register(
+        cls,
+        actor_ref: ActorRef[Any],
+    ) -> None:
+        """Register an :class:`ActorRef` in the registry.
 
         This is done automatically when an actor is started, e.g. by calling
         :meth:`Actor.start() <pykka.Actor.start>`.
 
         :param actor_ref: reference to the actor to register
         :type actor_ref: :class:`pykka.ActorRef`
         """
         with cls._actor_refs_lock:
             cls._actor_refs.append(actor_ref)
         logger.debug(f"Registered {actor_ref}")
 
+    @overload
     @classmethod
-    def stop_all(cls, block=True, timeout=None):
-        """
-        Stop all running actors.
+    def stop_all(
+        cls,
+        *,
+        block: Literal[True],
+        timeout: float | None = ...,
+    ) -> list[bool]:
+        ...
+
+    @overload
+    @classmethod
+    def stop_all(
+        cls,
+        *,
+        block: Literal[False],
+        timeout: float | None = ...,
+    ) -> list[Future[bool]]:
+        ...
+
+    @overload
+    @classmethod
+    def stop_all(
+        cls,
+        *,
+        block: bool = True,
+        timeout: Optional[float] = None,
+    ) -> Union[list[bool], list[Future[bool]]]:
+        ...
+
+    @classmethod
+    def stop_all(
+        cls,
+        *,
+        block: bool = True,
+        timeout: Optional[float] = None,
+    ) -> Union[list[bool], list[Future[bool]]]:
+        """Stop all running actors.
 
         ``block`` and ``timeout`` works as for
         :meth:`ActorRef.stop() <pykka.ActorRef.stop>`.
 
         If ``block`` is :class:`True`, the actors are guaranteed to be stopped
         in the reverse of the order they were started in. This is helpful if
         you have simple dependencies in between your actors, where it is
@@ -135,20 +195,24 @@
         by stopping dependees from a dependency's
         :meth:`on_stop() <pykka.Actor.on_stop>` method.
 
         :returns: If not blocking, a list with a future for each stop action.
             If blocking, a list of return values from
             :meth:`pykka.ActorRef.stop`.
         """
-        return [ref.stop(block, timeout) for ref in reversed(cls.get_all())]
+        return [
+            ref.stop(block=block, timeout=timeout) for ref in reversed(cls.get_all())
+        ]
 
     @classmethod
-    def unregister(cls, actor_ref):
-        """
-        Remove an :class:`ActorRef <pykka.ActorRef>` from the registry.
+    def unregister(
+        cls,
+        actor_ref: ActorRef[A],
+    ) -> None:
+        """Remove an :class:`ActorRef <pykka.ActorRef>` from the registry.
 
         This is done automatically when an actor is stopped, e.g. by calling
         :meth:`Actor.stop() <pykka.Actor.stop>`.
 
         :param actor_ref: reference to the actor to unregister
         :type actor_ref: :class:`pykka.ActorRef`
         """
```

### Comparing `pykka-3.1.1/src/pykka/_threading.py` & `pykka-4.0.0rc1/src/pykka/_threading.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,100 @@
+from __future__ import annotations
+
 import queue
 import sys
 import threading
-from typing import Any, NamedTuple, Optional
+from typing import TYPE_CHECKING, Any, ClassVar, NamedTuple, Optional, TypeVar
 
 from pykka import Actor, Future, Timeout
-from pykka._types import OptExcInfo
+
+if TYPE_CHECKING:
+    from pykka._actor import ActorInbox
+    from pykka._envelope import Envelope
+    from pykka._types import OptExcInfo
 
 __all__ = ["ThreadingActor", "ThreadingFuture"]
 
 
+T = TypeVar("T")
+
+
 class ThreadingFutureResult(NamedTuple):
     value: Optional[Any] = None
     exc_info: Optional[OptExcInfo] = None
 
 
-class ThreadingFuture(Future):
-    """
-    :class:`ThreadingFuture` implements :class:`Future` for use with
-    :class:`ThreadingActor <pykka.ThreadingActor>`.
+class ThreadingFuture(Future[T]):
+    """Implementation of :class:`Future` for use with regular Python threads`.
 
     The future is implemented using a :class:`queue.Queue`.
 
     The future does *not* make a copy of the object which is :meth:`set()
     <pykka.Future.set>` on it. It is the setters responsibility to only pass
     immutable objects or make a copy of the object before setting it on the
     future.
 
     .. versionchanged:: 0.14
         Previously, the encapsulated value was a copy made with
         :func:`copy.deepcopy`, unless the encapsulated value was a future, in
         which case the original future was encapsulated.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self._queue = queue.Queue(maxsize=1)
-        self._result = None
+        self._queue: queue.Queue[ThreadingFutureResult] = queue.Queue(maxsize=1)
+        self._result: Optional[ThreadingFutureResult] = None
 
-    def get(self, timeout=None):
+    def get(
+        self,
+        *,
+        timeout: Optional[float] = None,
+    ) -> Any:
         try:
             return super().get(timeout=timeout)
         except NotImplementedError:
             pass
 
         try:
             if self._result is None:
                 self._result = self._queue.get(True, timeout)
+
             if self._result.exc_info is not None:
                 (exc_type, exc_value, exc_traceback) = self._result.exc_info
+                assert exc_type is not None
                 if exc_value is None:
                     exc_value = exc_type()
                 if exc_value.__traceback__ is not exc_traceback:
-                    raise exc_value.with_traceback(exc_traceback)
-                raise exc_value
-            else:
-                return self._result.value
+                    raise exc_value.with_traceback(exc_traceback)  # noqa: TRY301
+                raise exc_value  # noqa: TRY301
         except queue.Empty:
-            raise Timeout(f"{timeout} seconds")
-
-    def set(self, value=None):
+            raise Timeout(f"{timeout} seconds") from None
+        else:
+            return self._result.value
+
+    def set(
+        self,
+        value: Optional[Any] = None,
+    ) -> None:
         self._queue.put(ThreadingFutureResult(value=value), block=False)
 
-    def set_exception(self, exc_info=None):
+    def set_exception(
+        self,
+        exc_info: Optional[OptExcInfo] = None,
+    ) -> None:
         assert exc_info is None or len(exc_info) == 3
         if exc_info is None:
             exc_info = sys.exc_info()
         self._queue.put(ThreadingFutureResult(exc_info=exc_info))
 
 
 class ThreadingActor(Actor):
-    """
-    :class:`ThreadingActor` implements :class:`Actor` using regular Python
-    threads.
-    """
+    """Implementation of :class:`Actor` using regular Python threads."""
 
-    use_daemon_thread = False
+    use_daemon_thread: ClassVar[bool] = False
     """
     A boolean value indicating whether this actor is executed on a thread that
     is a daemon thread (:class:`True`) or not (:class:`False`). This must be
     set before :meth:`pykka.Actor.start` is called, otherwise
     :exc:`RuntimeError` is raised.
 
     The entire Python program exits when no alive non-daemon threads are left.
@@ -87,19 +103,20 @@
     :meth:`pykka.Actor.on_stop` will be called.
 
     Actors do not inherit the daemon flag from the actor that made it. It
     always has to be set explicitly for the actor to run on a daemonic thread.
     """
 
     @staticmethod
-    def _create_actor_inbox():
-        return queue.Queue()
+    def _create_actor_inbox() -> ActorInbox:
+        inbox: queue.Queue[Envelope[Any]] = queue.Queue()
+        return inbox
 
     @staticmethod
-    def _create_future():
+    def _create_future() -> Future[Any]:
         return ThreadingFuture()
 
-    def _start_actor_loop(self):
+    def _start_actor_loop(self) -> None:
         thread = threading.Thread(target=self._actor_loop)
         thread.name = thread.name.replace("Thread", self.__class__.__name__)
         thread.daemon = self.use_daemon_thread
         thread.start()
```

### Comparing `pykka-3.1.1/src/pykka/debug.py` & `pykka-4.0.0rc1/src/pykka/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+"""Debug helpers."""
+
 import logging
 import sys
 import threading
 import traceback
+from typing import Any
 
-logger = logging.getLogger("pykka")
+__all__ = ["log_thread_tracebacks"]
 
 
-__all__ = ["log_thread_tracebacks"]
+logger = logging.getLogger("pykka")
 
 
-def log_thread_tracebacks(*args, **kwargs):
-    """Logs at :attr:`logging.CRITICAL` level a traceback for each running
-    thread.
+def log_thread_tracebacks(*_args: Any, **_kwargs: Any) -> None:
+    """Log a traceback for each running thread at :attr:`logging.CRITICAL` level.
 
     This can be a convenient tool for debugging deadlocks.
 
     The function accepts any arguments so that it can easily be used as e.g. a
     signal handler, but it does not use the arguments for anything.
 
     To use this function as a signal handler, setup logging with a
@@ -49,14 +51,13 @@
 
     The morale is: setup signals using your main thread, start your actors,
     then let your main thread relax for the rest of your application's life
     cycle.
 
     .. versionadded:: 1.1
     """
-
     thread_names = {t.ident: t.name for t in threading.enumerate()}
 
-    for ident, frame in sys._current_frames().items():
+    for ident, frame in sys._current_frames().items():  # noqa: SLF001
         name = thread_names.get(ident, "?")
         stack = "".join(traceback.format_stack(frame))
         logger.critical(f"Current state of {name} (ident: {ident}):\n{stack}")
```

### Comparing `pykka-3.1.1/src/pykka/messages.py` & `pykka-4.0.0rc1/src/pykka/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-The :mod:`pykka.messages` module contains Pykka's own actor messages.
+"""The :mod:`pykka.messages` module contains Pykka's own actor messages.
 
 In general, you should not need to use any of these classes. However, they have
 been made part of the public API so that certain optimizations can be done
 without touching Pykka's internals.
 
 An example is to combine :meth:`~pykka.ActorRef.ask` and :class:`ProxyCall`
 to call a method on an actor without having to spend any resources on creating
@@ -21,44 +20,47 @@
 :meth:`~pykka.ActorRef.ask` for the proxy method call, and thus avoid the
 creation of a future for the return value if you don't need it.
 
 It should be noted that these optimizations should only be necessary in very
 special circumstances.
 """
 
-from typing import Any, Dict, NamedTuple, Sequence, Tuple
+from __future__ import annotations
 
+from typing import TYPE_CHECKING, Any, Dict, NamedTuple, Tuple
 
-class _ActorStop(NamedTuple):
-    """Internal message."""
+if TYPE_CHECKING:
+    from pykka._types import AttrPath
 
-    pass
+
+class _ActorStop(NamedTuple):  # pyright: ignore[reportUnusedClass]
+    """Internal message."""
 
 
 class ProxyCall(NamedTuple):
     """Message to ask the actor to call the method with the arguments."""
 
     #: List with the path from the actor to the method.
-    attr_path: Sequence[str]
+    attr_path: AttrPath
 
     #: List with positional arguments.
-    args: Tuple[Any]
+    args: Tuple[Any, ...]
 
     #: Dict with keyword arguments.
     kwargs: Dict[str, Any]
 
 
 class ProxyGetAttr(NamedTuple):
     """Message to ask the actor to return the value of the attribute."""
 
     #: List with the path from the actor to the attribute.
-    attr_path: Sequence[str]
+    attr_path: AttrPath
 
 
 class ProxySetAttr(NamedTuple):
     """Message to ask the actor to set the attribute to the value."""
 
     #: List with the path from the actor to the attribute.
-    attr_path: Sequence[str]
+    attr_path: AttrPath
 
     #: The value to set the attribute to.
     value: Any
```

### Comparing `pykka-3.1.1/tests/test_actor.py` & `pykka-4.0.0rc1/tests/test_actor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,239 +1,305 @@
+from __future__ import annotations
+
 import uuid
+from typing import TYPE_CHECKING, Any, Iterator
 
 import pytest
 
-from pykka import ActorDeadError, ActorRegistry
+from pykka import Actor, ActorDeadError, ActorRegistry
 
-pytestmark = pytest.mark.usefixtures("stop_all")
+if TYPE_CHECKING:
+    from pykka import ActorRef
+    from tests.types import Events, Runtime
 
+pytestmark = pytest.mark.usefixtures("_stop_all")
 
-@pytest.fixture(scope="module")
-def actor_class(runtime):
-    class ActorA(runtime.actor_class):
-        def __init__(self, events):
-            super().__init__()
-            self.events = events
-
-        def on_start(self):
-            self.events.on_start_was_called.set()
-            if ActorRegistry.get_by_urn(self.actor_urn) is not None:
-                self.events.actor_registered_before_on_start_was_called.set()
-
-        def on_stop(self):
-            self.events.on_stop_was_called.set()
-
-        def on_failure(self, *args):
-            self.events.on_failure_was_called.set()
-
-        def on_receive(self, message):
-            if message.get("command") == "raise exception":
-                raise Exception("foo")
-            elif message.get("command") == "raise base exception":
-                raise BaseException()
-            elif message.get("command") == "stop twice":
-                self.stop()
-                self.stop()
-            elif message.get("command") == "message self then stop":
-                self.actor_ref.tell({"command": "greetings"})
-                self.stop()
-            elif message.get("command") == "greetings":
-                self.events.greetings_was_received.set()
-            elif message.get("command") == "callback":
-                message["callback"]()
-            else:
-                super().on_receive(message)
 
-    return ActorA
+class AnActor(Actor):
+    def __init__(self, events: Events) -> None:
+        super().__init__()
+        self.events = events
+
+    def on_start(self) -> None:
+        self.events.on_start_was_called.set()
+        if ActorRegistry.get_by_urn(self.actor_urn) is not None:
+            self.events.actor_registered_before_on_start_was_called.set()
+
+    def on_stop(self) -> None:
+        self.events.on_stop_was_called.set()
+
+    def on_failure(self, *args: Any) -> None:
+        self.events.on_failure_was_called.set()
 
+    def on_receive(self, message: Any) -> None:
+        if message.get("command") == "raise exception":
+            raise Exception("foo")
+
+        if message.get("command") == "raise base exception":
+            raise BaseException
+
+        if message.get("command") == "stop twice":
+            self.stop()
+            self.stop()
+        elif message.get("command") == "message self then stop":
+            self.actor_ref.tell({"command": "greetings"})
+            self.stop()
+        elif message.get("command") == "greetings":
+            self.events.greetings_was_received.set()
+        elif message.get("command") == "callback":
+            message["callback"]()
+        else:
+            super().on_receive(message)
+
+
+class EarlyStoppingActor(Actor):
+    def __init__(self, events: Events) -> None:
+        super().__init__()
+        self.events = events
 
-@pytest.fixture
-def actor_ref(actor_class, events):
+    def on_start(self) -> None:
+        self.stop()
+
+    def on_stop(self) -> None:
+        self.events.on_stop_was_called.set()
+
+
+@pytest.fixture(scope="module")
+def actor_class(runtime: Runtime) -> type[AnActor]:
+    class ActorAImpl(AnActor, runtime.actor_class):  # type: ignore[name-defined]  # noqa: E501
+        pass
+
+    return ActorAImpl
+
+
+@pytest.fixture()
+def actor_ref(
+    actor_class: type[AnActor],
+    events: Events,
+) -> Iterator[ActorRef[AnActor]]:
     ref = actor_class.start(events)
     yield ref
     ref.stop()
 
 
 @pytest.fixture(scope="module")
-def early_stopping_actor_class(runtime):
-    class EarlyStoppingActor(runtime.actor_class):
-        def __init__(self, events):
-            super().__init__()
-            self.events = events
-
-        def on_start(self):
-            self.stop()
-
-        def on_stop(self):
-            self.events.on_stop_was_called.set()
+def early_stopping_actor_class(runtime: Runtime) -> type[EarlyStoppingActor]:
+    class EarlyStoppingActorImpl(EarlyStoppingActor, runtime.actor_class):  # type: ignore[name-defined]  # noqa: E501
+        pass
 
-    return EarlyStoppingActor
+    return EarlyStoppingActorImpl
 
 
-def test_messages_left_in_queue_after_actor_stops_receive_an_error(runtime, actor_ref):
+def test_messages_left_in_queue_after_actor_stops_receive_an_error(
+    runtime: Runtime,
+    actor_ref: ActorRef[AnActor],
+) -> None:
     event = runtime.event_class()
 
     actor_ref.tell({"command": "callback", "callback": event.wait})
     actor_ref.stop(block=False)
     response = actor_ref.ask({"command": "irrelevant"}, block=False)
     event.set()
 
     with pytest.raises(ActorDeadError):
         response.get(timeout=0.5)
 
 
-def test_stop_requests_left_in_queue_after_actor_stops_are_handled(runtime, actor_ref):
+def test_stop_requests_left_in_queue_after_actor_stops_are_handled(
+    runtime: Runtime,
+    actor_ref: ActorRef[AnActor],
+) -> None:
     event = runtime.event_class()
 
     actor_ref.tell({"command": "callback", "callback": event.wait})
     actor_ref.stop(block=False)
     response = actor_ref.stop(block=False)
     event.set()
 
     response.get(timeout=0.5)
 
 
-def test_actor_has_an_uuid4_based_urn(actor_ref):
+def test_actor_has_an_uuid4_based_urn(actor_ref: ActorRef[AnActor]) -> None:
     assert uuid.UUID(actor_ref.actor_urn).version == 4
 
 
-def test_actor_has_unique_uuid(actor_class, events):
+def test_actor_has_unique_uuid(
+    actor_class: type[AnActor],
+    events: Events,
+) -> None:
     actors = [actor_class.start(events) for _ in range(3)]
 
     assert actors[0].actor_urn != actors[1].actor_urn
     assert actors[1].actor_urn != actors[2].actor_urn
     assert actors[2].actor_urn != actors[0].actor_urn
 
 
-def test_str_on_raw_actor_contains_actor_class_name(actor_class, events):
+def test_str_on_raw_actor_contains_actor_class_name(
+    actor_class: type[AnActor],
+    events: Events,
+) -> None:
     unstarted_actor = actor_class(events)
 
     assert "ActorA" in str(unstarted_actor)
 
 
-def test_str_on_raw_actor_contains_actor_urn(actor_class, events):
+def test_str_on_raw_actor_contains_actor_urn(
+    actor_class: type[AnActor],
+    events: Events,
+) -> None:
     unstarted_actor = actor_class(events)
 
     assert unstarted_actor.actor_urn in str(unstarted_actor)
 
 
-def test_init_can_be_called_with_arbitrary_arguments(runtime):
+def test_init_can_be_called_with_arbitrary_arguments(runtime: Runtime) -> None:
     runtime.actor_class(1, 2, 3, foo="bar")
 
 
-def test_on_start_is_called_before_first_message_is_processed(actor_ref, events):
+def test_on_start_is_called_before_first_message_is_processed(
+    actor_ref: ActorRef[AnActor],
+    events: Events,
+) -> None:
     events.on_start_was_called.wait(5)
     assert events.on_start_was_called.is_set()
 
 
-def test_on_start_is_called_after_the_actor_is_registered(actor_ref, events):
+def test_on_start_is_called_after_the_actor_is_registered(
+    actor_ref: ActorRef[AnActor],
+    events: Events,
+) -> None:
     # NOTE: If the actor is registered after the actor is started, this
     # test may still occasionally pass, as it is dependant on the exact
     # timing of events. When the actor is first registered and then
     # started, this test should always pass.
     events.on_start_was_called.wait(5)
     assert events.on_start_was_called.is_set()
 
     events.actor_registered_before_on_start_was_called.wait(0.1)
     assert events.actor_registered_before_on_start_was_called.is_set()
 
 
 def test_on_start_can_stop_actor_before_receive_loop_is_started(
-    early_stopping_actor_class, events
-):
+    early_stopping_actor_class: type[AnActor],
+    events: Events,
+) -> None:
     # NOTE: This test will pass even if the actor is allowed to start the
     # receive loop, but it will cause the test suite to hang, as the actor
     # thread is blocking on receiving messages to the actor inbox forever.
     # If one made this test specifically for ThreadingActor, one could add
     # an assertFalse(actor_thread.is_alive()), which would cause the test
     # to fail properly.
     actor_ref = early_stopping_actor_class.start(events)
 
     events.on_stop_was_called.wait(5)
     assert events.on_stop_was_called.is_set()
     assert not actor_ref.is_alive()
 
 
-def test_on_start_failure_causes_actor_to_stop(early_failing_actor_class, events):
+def test_on_start_failure_causes_actor_to_stop(
+    early_failing_actor_class: type[AnActor],
+    events: Events,
+) -> None:
     # Actor should not be alive if on_start fails.
 
     actor_ref = early_failing_actor_class.start(events)
     events.on_start_was_called.wait(5)
 
     actor_ref.actor_stopped.wait(5)
     assert not actor_ref.is_alive()
 
 
-def test_on_stop_is_called_when_actor_is_stopped(actor_ref, events):
+def test_on_stop_is_called_when_actor_is_stopped(
+    actor_ref: ActorRef[AnActor],
+    events: Events,
+) -> None:
     assert not events.on_stop_was_called.is_set()
 
     actor_ref.stop()
 
     events.on_stop_was_called.wait(5)
     assert events.on_stop_was_called.is_set()
 
 
-def test_on_stop_failure_causes_actor_to_stop(late_failing_actor_class, events):
+def test_on_stop_failure_causes_actor_to_stop(
+    late_failing_actor_class: type[AnActor],
+    events: Events,
+) -> None:
     actor_ref = late_failing_actor_class.start(events)
 
     events.on_stop_was_called.wait(5)
     assert not actor_ref.is_alive()
 
 
-def test_on_failure_is_called_when_exception_cannot_be_returned(actor_ref, events):
+def test_on_failure_is_called_when_exception_cannot_be_returned(
+    actor_ref: ActorRef[AnActor],
+    events: Events,
+) -> None:
     assert not events.on_failure_was_called.is_set()
 
     actor_ref.tell({"command": "raise exception"})
 
     events.on_failure_was_called.wait(5)
     assert events.on_failure_was_called.is_set()
     assert not events.on_stop_was_called.is_set()
 
 
 def test_on_failure_failure_causes_actor_to_stop(
-    failing_on_failure_actor_class, events
-):
+    failing_on_failure_actor_class: type[AnActor],
+    events: Events,
+) -> None:
     actor_ref = failing_on_failure_actor_class.start(events)
 
     actor_ref.tell({"command": "raise exception"})
 
     events.on_failure_was_called.wait(5)
     assert not actor_ref.is_alive()
 
 
-def test_actor_is_stopped_when_unhandled_exceptions_are_raised(actor_ref, events):
+def test_actor_is_stopped_when_unhandled_exceptions_are_raised(
+    actor_ref: ActorRef[AnActor],
+    events: Events,
+) -> None:
     assert not events.on_failure_was_called.is_set()
 
     actor_ref.tell({"command": "raise exception"})
 
     events.on_failure_was_called.wait(5)
     assert events.on_failure_was_called.is_set()
     assert len(ActorRegistry.get_all()) == 0
 
 
-def test_all_actors_are_stopped_on_base_exception(events, actor_ref):
+def test_all_actors_are_stopped_on_base_exception(
+    actor_ref: ActorRef[AnActor],
+    events: Events,
+) -> None:
     assert len(ActorRegistry.get_all()) == 1
     assert not events.on_stop_was_called.is_set()
 
     actor_ref.tell({"command": "raise base exception"})
 
     events.on_stop_was_called.wait(5)
     assert events.on_stop_was_called.is_set()
     assert len(ActorRegistry.get_all()) == 0
 
     events.on_stop_was_called.wait(5)
     assert events.on_stop_was_called.is_set()
     assert len(ActorRegistry.get_all()) == 0
 
 
-def test_actor_can_call_stop_on_self_multiple_times(actor_ref):
+def test_actor_can_call_stop_on_self_multiple_times(
+    actor_ref: ActorRef[AnActor],
+) -> None:
     actor_ref.ask({"command": "stop twice"})
 
 
-def test_actor_processes_all_messages_before_stop_on_self_stops_it(actor_ref, events):
+def test_actor_processes_all_messages_before_stop_on_self_stops_it(
+    actor_ref: ActorRef[AnActor],
+    events: Events,
+) -> None:
     actor_ref.ask({"command": "message self then stop"})
 
     events.greetings_was_received.wait(5)
     assert events.greetings_was_received.is_set()
 
     events.on_stop_was_called.wait(5)
     assert len(ActorRegistry.get_all()) == 0
```

### Comparing `pykka-3.1.1/tests/test_future.py` & `pykka-4.0.0rc1/tests/test_future.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,117 @@
+from __future__ import annotations
+
 import asyncio
 import sys
 import traceback
+from typing import TYPE_CHECKING, Any, Generator, Iterable, List
 
 import pytest
 
 from pykka import Future, Timeout, get_all
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tests.types import Runtime
+
 
-def run_async(coroutine):
+def run_async(coroutine: Any) -> Any:
     loop = asyncio.get_event_loop()
     f = asyncio.ensure_future(coroutine, loop=loop)
     return loop.run_until_complete(f)
 
 
-def test_base_future_get_is_not_implemented():
-    future = Future()
+def test_base_future_get_is_not_implemented() -> None:
+    future: Future[Any] = Future()
 
     with pytest.raises(NotImplementedError):
         future.get()
 
 
-def test_base_future_set_is_not_implemented():
-    future = Future()
+def test_base_future_set_is_not_implemented() -> None:
+    future: Future[Any] = Future()
 
     with pytest.raises(NotImplementedError):
         future.set(None)
 
 
-def test_base_future_set_exception_is_not_implemented():
-    future = Future()
+def test_base_future_set_exception_is_not_implemented() -> None:
+    future: Future[Any] = Future()
 
     with pytest.raises(NotImplementedError):
         future.set_exception(None)
 
 
-def test_set_multiple_times_fails(future):
+def test_set_multiple_times_fails(
+    future: Future[int],
+) -> None:
     future.set(0)
 
-    with pytest.raises(Exception):
+    with pytest.raises(Exception):  # noqa: B017, PT011
         future.set(0)
 
 
-def test_get_all_blocks_until_all_futures_are_available(futures):
+def test_get_all_blocks_until_all_futures_are_available(
+    futures: list[Future[int]],
+) -> None:
     futures[0].set(0)
     futures[1].set(1)
     futures[2].set(2)
 
     result = get_all(futures)
 
     assert result == [0, 1, 2]
 
 
-def test_get_all_raises_timeout_if_not_all_futures_are_available(futures):
+def test_get_all_raises_timeout_if_not_all_futures_are_available(
+    futures: list[Future[int]],
+) -> None:
     futures[0].set(0)
     futures[1].set(1)
-    # futures[2] is unset
+    # futures[2] has not been set
 
     with pytest.raises(Timeout):
         get_all(futures, timeout=0)
 
 
-def test_get_all_can_be_called_multiple_times(futures):
+def test_get_all_can_be_called_multiple_times(
+    futures: list[Future[int]],
+) -> None:
     futures[0].set(0)
     futures[1].set(1)
     futures[2].set(2)
 
     result1 = get_all(futures)
     result2 = get_all(futures)
 
     assert result1 == result2
 
 
-def test_future_in_future_works(runtime):
+def test_future_in_future_works(runtime: Runtime) -> None:
     inner_future = runtime.future_class()
     inner_future.set("foo")
 
     outer_future = runtime.future_class()
     outer_future.set(inner_future)
 
     assert outer_future.get().get() == "foo"
 
 
-def test_get_raises_exception_with_full_traceback(runtime):
+def test_get_raises_exception_with_full_traceback(runtime: Runtime) -> None:
     exc_class_get = None
     exc_class_set = None
     exc_instance_get = None
     exc_instance_set = None
     exc_traceback_get = None
     exc_traceback_set = None
     future = runtime.future_class()
 
     try:
-        raise NameError("foo")
+        raise NameError("foo")  # noqa: TRY301
     except NameError:
         exc_class_set, exc_instance_set, exc_traceback_set = sys.exc_info()
         future.set_exception()
 
     # We could move to another thread at this point
 
     try:
@@ -112,158 +128,197 @@
     # All frames from the first traceback should be included in the
     # traceback from the future.get() reraise
     assert len(exc_traceback_list_set) < len(exc_traceback_list_get)
     for i, frame in enumerate(exc_traceback_list_set):
         assert frame == exc_traceback_list_get[i]
 
 
-def test_future_supports_await_syntax(future):
-    async def get_value():
+def test_future_supports_await_syntax(
+    future: Future[int],
+) -> None:
+    async def get_value() -> int:
         return await future
 
     future.set(1)
     assert run_async(get_value()) == 1
 
 
-def test_future_supports_yield_from_syntax(future):
-    def get_value():
+def test_future_supports_yield_from_syntax(
+    future: Future[int],
+) -> None:
+    def get_value() -> Generator[None, None, int]:
         val = yield from future
         return val
 
     future.set(1)
     assert run_async(get_value()) == 1
 
 
-def test_filter_excludes_items_not_matching_predicate(future):
+def test_filter_excludes_items_not_matching_predicate(
+    future: Future[Iterable[int]],
+) -> None:
     filtered = future.filter(lambda x: x > 10)
     future.set([1, 3, 5, 7, 9, 11, 13, 15, 17, 19])
 
     assert filtered.get(timeout=0) == [11, 13, 15, 17, 19]
 
 
-def test_filter_on_noniterable(future):
-    filtered = future.filter(lambda x: x > 10)
+def test_filter_on_noniterable(
+    future: Future[int],
+) -> None:
+    filtered = future.filter(lambda x: x > 10)  # type: ignore  # noqa: PGH003
     future.set(1)
 
     with pytest.raises(TypeError):
         filtered.get(timeout=0)
 
 
-def test_filter_preserves_the_timeout_kwarg(future):
+def test_filter_preserves_the_timeout_kwarg(
+    future: Future[Iterable[int]],
+) -> None:
     filtered = future.filter(lambda x: x > 10)
 
     with pytest.raises(Timeout):
         filtered.get(timeout=0)
 
 
-def test_filter_reuses_result_if_called_multiple_times(future, mocker):
+def test_filter_reuses_result_if_called_multiple_times(
+    future: Future[Iterable[int]],
+    mocker: MockerFixture,
+) -> None:
     raise_on_reuse_func = mocker.Mock(side_effect=[False, True, Exception])
 
     filtered = future.filter(raise_on_reuse_func)
     future.set([1, 2])
 
     assert filtered.get(timeout=0) == [2]
     assert filtered.get(timeout=0) == [2]  # First result is reused
     assert filtered.get(timeout=0) == [2]  # First result is reused
 
 
-def test_join_combines_multiple_futures_into_one(futures):
+def test_join_combines_multiple_futures_into_one(
+    futures: List[Future[int]],
+) -> None:
     joined = futures[0].join(futures[1], futures[2])
     futures[0].set(0)
     futures[1].set(1)
     futures[2].set(2)
 
     assert joined.get(timeout=0) == [0, 1, 2]
 
 
-def test_join_preserves_timeout_kwarg(futures):
+def test_join_preserves_timeout_kwarg(
+    futures: List[Future[int]],
+) -> None:
     joined = futures[0].join(futures[1], futures[2])
     futures[0].set(0)
     futures[1].set(1)
-    # futures[2] is unset
+    # futures[2] has not been set
 
     with pytest.raises(Timeout):
         joined.get(timeout=0)
 
 
-def test_map_returns_future_which_passes_result_through_func(future):
+def test_map_returns_future_which_passes_result_through_func(
+    future: Future[int],
+) -> None:
     mapped = future.map(lambda x: x + 10)
     future.set(30)
 
     assert mapped.get(timeout=0) == 40
 
 
-def test_map_works_on_dict(future):
+def test_map_works_on_dict(
+    future: Future[dict[str, str]],
+) -> None:
     # Regression test for issue #64
 
     mapped = future.map(lambda x: x["foo"])
     future.set({"foo": "bar"})
 
     assert mapped.get(timeout=0) == "bar"
 
 
-def test_map_does_not_map_each_value_in_futures_iterable_result(future):
+def test_map_does_not_map_each_value_in_futures_iterable_result(
+    future: Future[Iterable[int]],
+) -> None:
     # Behavior changed in Pykka 2.0:
     # This used to map each value in the future's result through the func,
     # yielding [20, 30, 40].
 
-    mapped = future.map(lambda x: x + 10)
+    mapped = future.map(lambda x: x + 10)  # type: ignore  # noqa: PGH003
     future.set([10, 20, 30])
 
     with pytest.raises(TypeError):
         mapped.get(timeout=0)
 
 
-def test_map_preserves_timeout_kwarg(future):
+def test_map_preserves_timeout_kwarg(
+    future: Future[int],
+) -> None:
     mapped = future.map(lambda x: x + 10)
 
     with pytest.raises(Timeout):
         mapped.get(timeout=0)
 
 
-def test_map_reuses_result_if_called_multiple_times(future, mocker):
+def test_map_reuses_result_if_called_multiple_times(
+    future: Future[int],
+    mocker: MockerFixture,
+) -> None:
     raise_on_reuse_func = mocker.Mock(side_effect=[10, Exception])
 
     mapped = future.map(raise_on_reuse_func)
     future.set(30)
 
     assert mapped.get(timeout=0) == 10
     assert mapped.get(timeout=0) == 10  # First result is reused
 
 
-def test_reduce_applies_function_cumulatively_from_the_left(future):
-    reduced = future.reduce(lambda x, y: x + y)
+def test_reduce_applies_function_cumulatively_from_the_left(
+    future: Future[Iterable[int]],
+) -> None:
+    reduced: Future[int] = future.reduce(lambda x, y: x + y)
     future.set([1, 2, 3, 4])
 
     assert reduced.get(timeout=0) == 10
 
 
-def test_reduce_accepts_an_initial_value(future):
+def test_reduce_accepts_an_initial_value(
+    future: Future[Iterable[int]],
+) -> None:
     reduced = future.reduce(lambda x, y: x + y, 5)
     future.set([1, 2, 3, 4])
 
     assert reduced.get(timeout=0) == 15
 
 
-def test_reduce_on_noniterable(future):
-    reduced = future.reduce(lambda x, y: x + y)
+def test_reduce_on_noniterable(
+    future: Future[int],
+) -> None:
+    reduced = future.reduce(lambda x, y: x + y)  # type: ignore  # noqa: PGH003
     future.set(1)
 
     with pytest.raises(TypeError):
         reduced.get(timeout=0)
 
 
-def test_reduce_preserves_the_timeout_kwarg(future):
-    reduced = future.reduce(lambda x, y: x + y)
+def test_reduce_preserves_the_timeout_kwarg(
+    future: Future[Iterable[int]],
+) -> None:
+    reduced: Future[int] = future.reduce(lambda x, y: x + y)
 
     with pytest.raises(Timeout):
         reduced.get(timeout=0)
 
 
-def test_reduce_reuses_result_if_called_multiple_times(future, mocker):
+def test_reduce_reuses_result_if_called_multiple_times(
+    future: Future[Iterable[int]],
+    mocker: MockerFixture,
+) -> None:
     raise_on_reuse_func = mocker.Mock(side_effect=[3, 6, Exception])
 
     reduced = future.reduce(raise_on_reuse_func)
     future.set([1, 2, 3])
 
     assert reduced.get(timeout=0) == 6
     assert reduced.get(timeout=0) == 6  # First result is reused
```

### Comparing `pykka-3.1.1/tests/test_ref.py` & `pykka-4.0.0rc1/tests/test_ref.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,150 +1,212 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Callable, Iterator
+
 import pytest
 
-from pykka import ActorDeadError, Timeout
+from pykka import Actor, ActorDeadError, Timeout
+
+if TYPE_CHECKING:
+    from pykka import ActorRef, Future
+    from tests.types import Runtime
+
+
+class ReferencableActor(Actor):
+    received_messages = None
+
+    def __init__(
+        self,
+        sleep_func: Callable[[float], None],
+        received_message: Future[str],
+    ) -> None:
+        super().__init__()
+        self.sleep_func = sleep_func
+        self.received_message = received_message
+
+    def on_receive(self, message: str) -> Any:
+        if message == "ping":
+            self.sleep_func(0.01)
+            return "pong"
+
+        self.received_message.set(message)
+        return None
 
 
 @pytest.fixture(scope="module")
-def actor_class(runtime):
-    class ActorA(runtime.actor_class):
-        received_messages = None
-
-        def __init__(self, received_message):
-            super(runtime.actor_class, self).__init__()
-            self.received_message = received_message
-
-        def on_receive(self, message):
-            if isinstance(message, dict) and message.get("command") == "ping":
-                runtime.sleep_func(0.01)
-                return "pong"
-            else:
-                self.received_message.set(message)
+def actor_class(runtime: Runtime) -> type[ReferencableActor]:
+    class ReferencableActorImpl(ReferencableActor, runtime.actor_class):  # type: ignore[name-defined]  # noqa: E501
+        pass
 
-    return ActorA
+    return ReferencableActorImpl
 
 
-@pytest.fixture
-def received_messages(runtime):
+@pytest.fixture()
+def received_message(runtime: Runtime) -> Future[str]:
     return runtime.future_class()
 
 
-@pytest.fixture
-def actor_ref(actor_class, received_messages):
-    ref = actor_class.start(received_messages)
+@pytest.fixture()
+def actor_ref(
+    runtime: Runtime,
+    actor_class: type[ReferencableActor],
+    received_message: Future[str],
+) -> Iterator[ActorRef[ReferencableActor]]:
+    ref = actor_class.start(
+        runtime.sleep_func,
+        received_message,
+    )
     yield ref
     ref.stop()
 
 
-def test_repr_is_wrapped_in_lt_and_gt(actor_ref):
+def test_repr_is_wrapped_in_lt_and_gt(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     result = repr(actor_ref)
 
     assert result.startswith("<")
     assert result.endswith(">")
 
 
-def test_repr_reveals_that_this_is_a_ref(actor_ref):
+def test_repr_reveals_that_this_is_a_ref(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     assert "ActorRef" in repr(actor_ref)
 
 
-def test_repr_contains_actor_class_name(actor_ref):
-    assert "ActorA" in repr(actor_ref)
+def test_repr_contains_actor_class_name(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
+    assert "ReferencableActor" in repr(actor_ref)
 
 
-def test_repr_contains_actor_urn(actor_ref):
+def test_repr_contains_actor_urn(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     assert actor_ref.actor_urn in repr(actor_ref)
 
 
-def test_str_contains_actor_class_name(actor_ref):
-    assert "ActorA" in str(actor_ref)
+def test_str_contains_actor_class_name(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
+    assert "ReferencableActor" in str(actor_ref)
 
 
-def test_str_contains_actor_urn(actor_ref):
+def test_str_contains_actor_urn(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     assert actor_ref.actor_urn in str(actor_ref)
 
 
-def test_is_alive_returns_true_for_running_actor(actor_ref):
+def test_is_alive_returns_true_for_running_actor(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     assert actor_ref.is_alive()
 
 
-def test_is_alive_returns_false_for_dead_actor(actor_ref):
+def test_is_alive_returns_false_for_dead_actor(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     actor_ref.stop()
 
     assert not actor_ref.is_alive()
 
 
-def test_stop_returns_true_if_actor_is_stopped(actor_ref):
+def test_stop_returns_true_if_actor_is_stopped(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     assert actor_ref.stop()
 
 
-def test_stop_does_not_stop_already_dead_actor(actor_ref):
+def test_stop_does_not_stop_already_dead_actor(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     assert actor_ref.stop()
     assert not actor_ref.stop()
 
 
 def test_tell_delivers_message_to_actors_custom_on_receive(
-    actor_ref, received_messages
-):
-    actor_ref.tell({"command": "a custom message"})
+    actor_ref: ActorRef[ReferencableActor],
+    received_message: Future[str],
+) -> None:
+    actor_ref.tell("a custom message")
 
-    assert received_messages.get(timeout=1) == {"command": "a custom message"}
+    assert received_message.get(timeout=1) == "a custom message"
 
 
 @pytest.mark.parametrize(
     "message",
     [
         123,
         123.456,
         {"a": "dict"},
         ("a", "tuple"),
         ["a", "list"],
         Exception("an exception"),
     ],
 )
-def test_tell_accepts_any_object_as_the_message(actor_ref, message, received_messages):
+def test_tell_accepts_any_object_as_the_message(
+    actor_ref: ActorRef[ReferencableActor],
+    message: Any,
+    received_message: Future[Any],
+) -> None:
     actor_ref.tell(message)
 
-    assert received_messages.get(timeout=1) == message
+    assert received_message.get(timeout=1) == message
 
 
-def test_tell_fails_if_actor_is_stopped(actor_ref):
+def test_tell_fails_if_actor_is_stopped(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     actor_ref.stop()
 
     with pytest.raises(ActorDeadError) as exc_info:
-        actor_ref.tell({"command": "a custom message"})
+        actor_ref.tell("a custom message")
 
     assert str(exc_info.value) == f"{actor_ref} not found"
 
 
-def test_ask_blocks_until_response_arrives(actor_ref):
-    result = actor_ref.ask({"command": "ping"})
+def test_ask_blocks_until_response_arrives(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
+    result = actor_ref.ask("ping")
 
     assert result == "pong"
 
 
-def test_ask_can_timeout_if_blocked_too_long(actor_ref):
+def test_ask_can_timeout_if_blocked_too_long(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     with pytest.raises(Timeout):
-        actor_ref.ask({"command": "ping"}, timeout=0)
+        actor_ref.ask("ping", timeout=0)
 
 
-def test_ask_can_return_future_instead_of_blocking(actor_ref):
-    future = actor_ref.ask({"command": "ping"}, block=False)
+def test_ask_can_return_future_instead_of_blocking(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
+    future = actor_ref.ask("ping", block=False)
 
     assert future.get() == "pong"
 
 
-def test_ask_fails_if_actor_is_stopped(actor_ref):
+def test_ask_fails_if_actor_is_stopped(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     actor_ref.stop()
 
     with pytest.raises(ActorDeadError) as exc_info:
-        actor_ref.ask({"command": "ping"})
+        actor_ref.ask("ping")
 
     assert str(exc_info.value) == f"{actor_ref} not found"
 
 
-def test_ask_nonblocking_fails_future_if_actor_is_stopped(actor_ref):
+def test_ask_nonblocking_fails_future_if_actor_is_stopped(
+    actor_ref: ActorRef[ReferencableActor],
+) -> None:
     actor_ref.stop()
-    future = actor_ref.ask({"command": "ping"}, block=False)
+    future = actor_ref.ask("ping", block=False)
 
     with pytest.raises(ActorDeadError) as exc_info:
         future.get()
 
     assert str(exc_info.value) == f"{actor_ref} not found"
```

### Comparing `pykka-3.1.1/tests/test_threading_actor.py` & `pykka-4.0.0rc1/tests/test_threading_actor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,65 @@
+from __future__ import annotations
+
 import threading
+from typing import TYPE_CHECKING, Iterator
 
 import pytest
 
 from pykka import ThreadingActor
 
+if TYPE_CHECKING:
+    from pykka import ActorRef
+
 
 class RegularActor(ThreadingActor):
     pass
 
 
 class DaemonActor(ThreadingActor):
     use_daemon_thread = True
 
 
-@pytest.fixture
-def regular_actor_ref():
+@pytest.fixture()
+def regular_actor_ref() -> Iterator[ActorRef[RegularActor]]:
     ref = RegularActor.start()
     yield ref
     ref.stop()
 
 
-@pytest.fixture
-def daemon_actor_ref():
+@pytest.fixture()
+def daemon_actor_ref() -> Iterator[ActorRef[DaemonActor]]:
     ref = DaemonActor.start()
     yield ref
     ref.stop()
 
 
-def test_actor_thread_is_named_after_pykka_actor_class(regular_actor_ref):
+def test_actor_thread_is_named_after_pykka_actor_class(
+    regular_actor_ref: ActorRef[RegularActor],
+) -> None:
     alive_threads = threading.enumerate()
     alive_thread_names = [t.name for t in alive_threads]
     named_correctly = [
         name.startswith(RegularActor.__name__) for name in alive_thread_names
     ]
 
     assert any(named_correctly)
 
 
-def test_actor_thread_is_not_daemonic_by_default(regular_actor_ref):
+def test_actor_thread_is_not_daemonic_by_default(
+    regular_actor_ref: ActorRef[RegularActor],
+) -> None:
     alive_threads = threading.enumerate()
     actor_threads = [t for t in alive_threads if t.name.startswith("RegularActor")]
 
     assert len(actor_threads) == 1
     assert not actor_threads[0].daemon
 
 
 def test_actor_thread_is_daemonic_if_use_daemon_thread_flag_is_set(
-    daemon_actor_ref,
-):
+    daemon_actor_ref: ActorRef[DaemonActor],
+) -> None:
     alive_threads = threading.enumerate()
     actor_threads = [t for t in alive_threads if t.name.startswith("DaemonActor")]
 
     assert len(actor_threads) == 1
     assert actor_threads[0].daemon
```

### Comparing `pykka-3.1.1/PKG-INFO` & `pykka-4.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pykka
-Version: 3.1.1
+Version: 4.0.0rc1
 Summary: Pykka is a Python implementation of the actor model
 Home-page: https://github.com/jodal/pykka
 License: Apache-2.0
 Keywords: actor,concurrency,threading
 Author: Stein Magnus Jodal
 Author-email: stein.magnus@jodal.no
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: importlib_metadata (>=1.6); python_version < "3.8"
+Requires-Dist: typing-extensions (>=4.0.0,<5.0.0) ; python_version < "3.10"
 Project-URL: Documentation, https://pykka.readthedocs.io/
 Project-URL: Repository, https://github.com/jodal/pykka
 Description-Content-Type: text/markdown
 
 # &#x1F300; Pykka
 
 _Pykka makes it easier to build concurrent applications._
 
-[![CI](https://img.shields.io/github/workflow/status/jodal/pykka/CI)](https://github.com/jodal/pykka/actions?workflow=CI)
+[![CI](https://img.shields.io/github/actions/workflow/status/jodal/pykka/ci.yml?branch=main)](https://github.com/jodal/pykka/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/pykka)](https://pykka.readthedocs.io/en/latest/)
 [![Coverage](https://img.shields.io/codecov/c/gh/jodal/pykka)](https://codecov.io/gh/jodal/pykka)
 [![PyPI](https://img.shields.io/pypi/v/pykka)](https://pypi.org/project/pykka/)
 
 ---
 
 Pykka is a Python implementation of the
@@ -40,15 +40,15 @@
 which makes it easier to build concurrent applications.
 
 For a quickstart guide and a complete API reference,
 see the [documentation](https://pykka.readthedocs.io/).
 
 ## Installation
 
-Pykka requires Python 3.7 or newer.
+Pykka requires Python 3.8 or newer.
 
 Pykka is available from [PyPI](https://pypi.org/project/pykka/):
 
 ```
 python3 -m pip install pykka
 ```
 
@@ -59,11 +59,11 @@
 - [Releases](https://github.com/jodal/pykka/releases)
 - [Issue tracker](https://github.com/jodal/pykka/issues)
 - [Contributors](https://github.com/jodal/pykka/graphs/contributors)
 - [Users](https://github.com/jodal/pykka/wiki/Users)
 
 ## License
 
-Pykka is copyright 2010-2022 Stein Magnus Jodal and contributors.
+Pykka is copyright 2010-2023 Stein Magnus Jodal and contributors.
 Pykka is licensed under the
 [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
```

