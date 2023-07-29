# Comparing `tmp/blacksmith-2.3.2.tar.gz` & `tmp/blacksmith-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksmith-2.3.2.tar", max compression
+gzip compressed data, was "blacksmith-2.3.3.tar", max compression
```

## Comparing `blacksmith-2.3.2.tar` & `blacksmith-2.3.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1528 2022-01-06 07:33:14.770656 blacksmith-2.3.2/LICENSE
--rw-r--r--   0        0        0     3769 2022-01-23 14:09:10.817286 blacksmith-2.3.2/README.rst
--rw-r--r--   0        0        0     2231 2023-05-11 07:19:40.543421 blacksmith-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     4003 2022-10-11 10:09:17.048567 blacksmith-2.3.2/src/blacksmith/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 07:19:10.263612 blacksmith-2.3.2/src/blacksmith/adapters/__init__.py
--rw-r--r--   0        0        0        0 2021-10-23 20:54:22.320117 blacksmith-2.3.2/src/blacksmith/domain/__init__.py
--rw-r--r--   0        0        0      813 2022-10-11 10:09:17.048567 blacksmith-2.3.2/src/blacksmith/domain/error.py
--rw-r--r--   0        0        0     3665 2022-10-10 18:11:37.257590 blacksmith-2.3.2/src/blacksmith/domain/exceptions.py
--rw-r--r--   0        0        0     1043 2022-10-11 10:09:17.048567 blacksmith-2.3.2/src/blacksmith/domain/model/__init__.py
--rw-r--r--   0        0        0     3278 2022-10-09 05:40:41.790453 blacksmith-2.3.2/src/blacksmith/domain/model/http.py
--rw-r--r--   0        0        0        0 2022-01-20 21:42:27.593890 blacksmith-2.3.2/src/blacksmith/domain/model/middleware/__init__.py
--rw-r--r--   0        0        0     1201 2022-02-04 22:04:27.203840 blacksmith-2.3.2/src/blacksmith/domain/model/middleware/circuit_breaker.py
--rw-r--r--   0        0        0     4365 2022-01-20 21:42:27.593890 blacksmith-2.3.2/src/blacksmith/domain/model/middleware/http_cache.py
--rw-r--r--   0        0        0     2993 2022-02-07 21:56:12.757093 blacksmith-2.3.2/src/blacksmith/domain/model/middleware/prometheus.py
--rw-r--r--   0        0        0     1174 2022-01-24 20:07:20.433938 blacksmith-2.3.2/src/blacksmith/domain/model/middleware/zipkin.py
--rw-r--r--   0        0        0    14313 2023-05-10 11:48:05.014686 blacksmith-2.3.2/src/blacksmith/domain/model/params.py
--rw-r--r--   0        0        0     5095 2022-10-10 21:39:42.618378 blacksmith-2.3.2/src/blacksmith/domain/registry.py
--rw-r--r--   0        0        0      983 2022-01-18 22:18:53.863644 blacksmith-2.3.2/src/blacksmith/domain/scanner.py
--rw-r--r--   0        0        0      885 2022-10-07 21:02:49.023029 blacksmith-2.3.2/src/blacksmith/domain/typing.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/middleware/__init__.py
--rw-r--r--   0        0        0      716 2022-01-22 22:10:58.887280 blacksmith-2.3.2/src/blacksmith/middleware/_async/__init__.py
--rw-r--r--   0        0        0      802 2022-01-22 22:10:58.887280 blacksmith-2.3.2/src/blacksmith/middleware/_async/auth.py
--rw-r--r--   0        0        0     1472 2022-10-07 21:02:43.642963 blacksmith-2.3.2/src/blacksmith/middleware/_async/base.py
--rw-r--r--   0        0        0     2330 2022-01-22 22:10:58.887280 blacksmith-2.3.2/src/blacksmith/middleware/_async/circuit_breaker.py
--rw-r--r--   0        0        0     5933 2023-05-11 07:19:10.263612 blacksmith-2.3.2/src/blacksmith/middleware/_async/http_cache.py
--rw-r--r--   0        0        0     2436 2022-02-04 22:05:35.793843 blacksmith-2.3.2/src/blacksmith/middleware/_async/prometheus.py
--rw-r--r--   0        0        0     2869 2022-01-24 20:07:20.433938 blacksmith-2.3.2/src/blacksmith/middleware/_async/zipkin.py
--rw-r--r--   0        0        0      696 2023-05-11 07:19:19.486887 blacksmith-2.3.2/src/blacksmith/middleware/_sync/__init__.py
--rw-r--r--   0        0        0      797 2023-05-11 07:19:19.486887 blacksmith-2.3.2/src/blacksmith/middleware/_sync/auth.py
--rw-r--r--   0        0        0     1434 2023-05-11 07:19:19.490221 blacksmith-2.3.2/src/blacksmith/middleware/_sync/base.py
--rw-r--r--   0        0        0     2284 2023-05-11 07:19:19.490221 blacksmith-2.3.2/src/blacksmith/middleware/_sync/circuit_breaker.py
--rw-r--r--   0        0        0     5827 2023-05-11 07:19:19.493554 blacksmith-2.3.2/src/blacksmith/middleware/_sync/http_cache.py
--rw-r--r--   0        0        0     2418 2023-05-11 07:19:19.486887 blacksmith-2.3.2/src/blacksmith/middleware/_sync/prometheus.py
--rw-r--r--   0        0        0     2851 2023-05-11 07:19:19.490221 blacksmith-2.3.2/src/blacksmith/middleware/_sync/zipkin.py
--rw-r--r--   0        0        0        0 2022-01-18 22:18:53.866978 blacksmith-2.3.2/src/blacksmith/py.typed
--rw-r--r--   0        0        0       24 2021-10-24 11:21:34.426587 blacksmith-2.3.2/src/blacksmith/sd/__init__.py
--rw-r--r--   0        0        0      334 2022-01-25 07:30:46.663983 blacksmith-2.3.2/src/blacksmith/sd/_async/__init__.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/sd/_async/adapters/__init__.py
--rw-r--r--   0        0        0     5660 2022-11-15 09:34:44.244184 blacksmith-2.3.2/src/blacksmith/sd/_async/adapters/consul.py
--rw-r--r--   0        0        0     1693 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/sd/_async/adapters/router.py
--rw-r--r--   0        0        0     1010 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/sd/_async/adapters/static.py
--rw-r--r--   0        0        0      317 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/sd/_async/base.py
--rw-r--r--   0        0        0      326 2023-05-11 07:19:19.496887 blacksmith-2.3.2/src/blacksmith/sd/_sync/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 07:19:19.496887 blacksmith-2.3.2/src/blacksmith/sd/_sync/adapters/__init__.py
--rw-r--r--   0        0        0     5614 2023-05-11 07:19:19.500220 blacksmith-2.3.2/src/blacksmith/sd/_sync/adapters/consul.py
--rw-r--r--   0        0        0     1684 2023-05-11 07:19:19.496887 blacksmith-2.3.2/src/blacksmith/sd/_sync/adapters/router.py
--rw-r--r--   0        0        0     1001 2023-05-11 07:19:19.496887 blacksmith-2.3.2/src/blacksmith/sd/_sync/adapters/static.py
--rw-r--r--   0        0        0      310 2023-05-11 07:19:19.493554 blacksmith-2.3.2/src/blacksmith/sd/_sync/base.py
--rw-r--r--   0        0        0        0 2021-10-23 21:02:59.310144 blacksmith-2.3.2/src/blacksmith/service/__init__.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/service/_async/__init__.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/service/_async/adapters/__init__.py
--rw-r--r--   0        0        0     2391 2023-05-10 11:48:05.014686 blacksmith-2.3.2/src/blacksmith/service/_async/adapters/httpx.py
--rw-r--r--   0        0        0      420 2022-10-08 15:37:33.544758 blacksmith-2.3.2/src/blacksmith/service/_async/base.py
--rw-r--r--   0        0        0     5903 2022-10-11 05:00:19.426732 blacksmith-2.3.2/src/blacksmith/service/_async/client.py
--rw-r--r--   0        0        0    12871 2022-10-10 21:39:42.621711 blacksmith-2.3.2/src/blacksmith/service/_async/route_proxy.py
--rw-r--r--   0        0        0        0 2023-05-11 07:19:19.500220 blacksmith-2.3.2/src/blacksmith/service/_sync/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 07:19:19.510220 blacksmith-2.3.2/src/blacksmith/service/_sync/adapters/__init__.py
--rw-r--r--   0        0        0     2368 2023-05-11 07:19:19.510220 blacksmith-2.3.2/src/blacksmith/service/_sync/adapters/httpx.py
--rw-r--r--   0        0        0      417 2023-05-11 07:19:19.500220 blacksmith-2.3.2/src/blacksmith/service/_sync/base.py
--rw-r--r--   0        0        0     5837 2023-05-11 07:19:23.260197 blacksmith-2.3.2/src/blacksmith/service/_sync/client.py
--rw-r--r--   0        0        0    12490 2023-05-11 07:19:23.373529 blacksmith-2.3.2/src/blacksmith/service/_sync/route_proxy.py
--rw-r--r--   0        0        0      121 2022-01-06 07:13:35.813927 blacksmith-2.3.2/src/blacksmith/service/ports.py
--rw-r--r--   0        0        0      450 2022-01-19 08:38:32.683866 blacksmith-2.3.2/src/blacksmith/typing.py
--rw-r--r--   0        0        0     5195 1970-01-01 00:00:00.000000 blacksmith-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1528 2022-01-06 07:33:14.770656 blacksmith-2.3.3/LICENSE
+-rw-r--r--   0        0        0     3878 2023-07-23 15:11:35.288448 blacksmith-2.3.3/README.rst
+-rw-r--r--   0        0        0     2209 2023-07-29 13:25:37.098513 blacksmith-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4003 2022-10-11 10:09:17.048567 blacksmith-2.3.3/src/blacksmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 07:19:10.263612 blacksmith-2.3.3/src/blacksmith/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-23 20:54:22.320117 blacksmith-2.3.3/src/blacksmith/domain/__init__.py
+-rw-r--r--   0        0        0      813 2022-10-11 10:09:17.048567 blacksmith-2.3.3/src/blacksmith/domain/error.py
+-rw-r--r--   0        0        0     3665 2022-10-10 18:11:37.257590 blacksmith-2.3.3/src/blacksmith/domain/exceptions.py
+-rw-r--r--   0        0        0     1043 2022-10-11 10:09:17.048567 blacksmith-2.3.3/src/blacksmith/domain/model/__init__.py
+-rw-r--r--   0        0        0     3278 2022-10-09 05:40:41.790453 blacksmith-2.3.3/src/blacksmith/domain/model/http.py
+-rw-r--r--   0        0        0        0 2022-01-20 21:42:27.593890 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/__init__.py
+-rw-r--r--   0        0        0     1201 2022-02-04 22:04:27.203840 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/circuit_breaker.py
+-rw-r--r--   0        0        0     4365 2022-01-20 21:42:27.593890 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/http_cache.py
+-rw-r--r--   0        0        0     2993 2022-02-07 21:56:12.757093 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/prometheus.py
+-rw-r--r--   0        0        0     1174 2022-01-24 20:07:20.433938 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/zipkin.py
+-rw-r--r--   0        0        0    14313 2023-05-10 11:48:05.014686 blacksmith-2.3.3/src/blacksmith/domain/model/params.py
+-rw-r--r--   0        0        0     5095 2022-10-10 21:39:42.618378 blacksmith-2.3.3/src/blacksmith/domain/registry.py
+-rw-r--r--   0        0        0      983 2022-01-18 22:18:53.863644 blacksmith-2.3.3/src/blacksmith/domain/scanner.py
+-rw-r--r--   0        0        0      885 2022-10-07 21:02:49.023029 blacksmith-2.3.3/src/blacksmith/domain/typing.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/middleware/__init__.py
+-rw-r--r--   0        0        0      716 2022-01-22 22:10:58.887280 blacksmith-2.3.3/src/blacksmith/middleware/_async/__init__.py
+-rw-r--r--   0        0        0      802 2022-01-22 22:10:58.887280 blacksmith-2.3.3/src/blacksmith/middleware/_async/auth.py
+-rw-r--r--   0        0        0     1472 2022-10-07 21:02:43.642963 blacksmith-2.3.3/src/blacksmith/middleware/_async/base.py
+-rw-r--r--   0        0        0     2330 2022-01-22 22:10:58.887280 blacksmith-2.3.3/src/blacksmith/middleware/_async/circuit_breaker.py
+-rw-r--r--   0        0        0     5933 2023-05-11 07:19:10.263612 blacksmith-2.3.3/src/blacksmith/middleware/_async/http_cache.py
+-rw-r--r--   0        0        0     2436 2022-02-04 22:05:35.793843 blacksmith-2.3.3/src/blacksmith/middleware/_async/prometheus.py
+-rw-r--r--   0        0        0     2869 2022-01-24 20:07:20.433938 blacksmith-2.3.3/src/blacksmith/middleware/_async/zipkin.py
+-rw-r--r--   0        0        0      696 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/__init__.py
+-rw-r--r--   0        0        0      797 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/auth.py
+-rw-r--r--   0        0        0     1434 2023-07-29 13:25:25.858473 blacksmith-2.3.3/src/blacksmith/middleware/_sync/base.py
+-rw-r--r--   0        0        0     2284 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/circuit_breaker.py
+-rw-r--r--   0        0        0     5827 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/middleware/_sync/http_cache.py
+-rw-r--r--   0        0        0     2418 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/prometheus.py
+-rw-r--r--   0        0        0     2851 2023-07-29 13:25:25.858473 blacksmith-2.3.3/src/blacksmith/middleware/_sync/zipkin.py
+-rw-r--r--   0        0        0        0 2022-01-18 22:18:53.866978 blacksmith-2.3.3/src/blacksmith/py.typed
+-rw-r--r--   0        0        0       24 2021-10-24 11:21:34.426587 blacksmith-2.3.3/src/blacksmith/sd/__init__.py
+-rw-r--r--   0        0        0      334 2022-01-25 07:30:46.663983 blacksmith-2.3.3/src/blacksmith/sd/_async/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/__init__.py
+-rw-r--r--   0        0        0     5660 2022-11-15 09:34:44.244184 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/consul.py
+-rw-r--r--   0        0        0     1693 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/router.py
+-rw-r--r--   0        0        0     1010 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/static.py
+-rw-r--r--   0        0        0      317 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/base.py
+-rw-r--r--   0        0        0      326 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/__init__.py
+-rw-r--r--   0        0        0     5614 2023-07-29 13:25:25.865140 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/consul.py
+-rw-r--r--   0        0        0     1684 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/router.py
+-rw-r--r--   0        0        0     1001 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/static.py
+-rw-r--r--   0        0        0      310 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/base.py
+-rw-r--r--   0        0        0        0 2021-10-23 21:02:59.310144 blacksmith-2.3.3/src/blacksmith/service/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/service/_async/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/service/_async/adapters/__init__.py
+-rw-r--r--   0        0        0     2391 2023-05-10 11:48:05.014686 blacksmith-2.3.3/src/blacksmith/service/_async/adapters/httpx.py
+-rw-r--r--   0        0        0      420 2022-10-08 15:37:33.544758 blacksmith-2.3.3/src/blacksmith/service/_async/base.py
+-rw-r--r--   0        0        0     5903 2022-10-11 05:00:19.426732 blacksmith-2.3.3/src/blacksmith/service/_async/client.py
+-rw-r--r--   0        0        0    12871 2022-10-10 21:39:42.621711 blacksmith-2.3.3/src/blacksmith/service/_async/route_proxy.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.865140 blacksmith-2.3.3/src/blacksmith/service/_sync/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.875140 blacksmith-2.3.3/src/blacksmith/service/_sync/adapters/__init__.py
+-rw-r--r--   0        0        0     2368 2023-07-29 13:25:25.875140 blacksmith-2.3.3/src/blacksmith/service/_sync/adapters/httpx.py
+-rw-r--r--   0        0        0      417 2023-07-29 13:25:25.865140 blacksmith-2.3.3/src/blacksmith/service/_sync/base.py
+-rw-r--r--   0        0        0     5837 2023-07-29 13:25:28.985151 blacksmith-2.3.3/src/blacksmith/service/_sync/client.py
+-rw-r--r--   0        0        0    12490 2023-07-29 13:25:29.061818 blacksmith-2.3.3/src/blacksmith/service/_sync/route_proxy.py
+-rw-r--r--   0        0        0      121 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/service/ports.py
+-rw-r--r--   0        0        0      450 2022-01-19 08:38:32.683866 blacksmith-2.3.3/src/blacksmith/typing.py
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 blacksmith-2.3.3/PKG-INFO
```

### Comparing `blacksmith-2.3.2/LICENSE` & `blacksmith-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/README.rst` & `blacksmith-2.3.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Blacksmith
 ==========
 
-.. image:: https://readthedocs.org/projects/python-blacksmith/badge/?version=latest
-   :target: https://python-blacksmith.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
+.. image:: https://github.com/mardiros/blacksmith/actions/workflows/gh-pages.yml/badge.svg
+   :target: https://mardiros.github.io/blacksmith/user/introduction.html
+   :alt: Documentation
 
 .. image:: https://github.com/mardiros/blacksmith/actions/workflows/main.yml/badge.svg
    :target: https://github.com/mardiros/blacksmith/actions/workflows/main.yml
    :alt: Continuous Integration
 
 .. image:: https://codecov.io/gh/mardiros/blacksmith/branch/master/graph/badge.svg?token=17KAC0LW9H
    :target: https://codecov.io/gh/mardiros/blacksmith
@@ -100,8 +100,13 @@
 
 
 Read More
 ---------
 
 You can read the `full documentation of this library here`_.
 
-.. _`full documentation of this library here`: https://python-blacksmith.readthedocs.io/en/latest/user/introduction.html
+.. _`full documentation of this library here`: https://mardiros.github.io/blacksmith/user/introduction.html
+
+.. important::
+
+   | The documentation has been moved to github pages.
+   | The documentation under readthedocs is obsolete.
```

### Comparing `blacksmith-2.3.2/pyproject.toml` & `blacksmith-2.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,50 +11,50 @@
 description = "REST API Client designed for microservices"
 homepage = "https://github.com/mardiros/blacksmith"
 license = "BSD-derived"
 name = "blacksmith"
 
 readme = "README.rst"
 repository = "https://github.com/mardiros/blacksmith"
-version = "2.3.2"
+version = "2.3.3"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-aioredis = {version = "^2.0.0", optional = true}
-httpx = "^0.24.0"
-prometheus-client = {version = "^0.16.0", optional = true}
-purgatory = "^1.0.2"
+httpx = "^0.24.1"
+prometheus-client = {version = "^0.17.1", optional = true}
+purgatory = "^1.0.3"
 pydantic = "^1.10.7"
-typing-extensions = "^4.5.0"
-result = "^0.10.0"
+typing-extensions = "^4.7.0"
+result = "^0.11.0"
 
 [tool.poetry.extras]
 http_cache_async = ["redis"]
 http_cache_sync = ["redis"]
 prometheus = ["prometheus-client"]
 
 [tool.poetry.dev-dependencies]
-Sphinx = "^4.2.0"
-black = "^22.1.0"
-coverage = {version = "^6.2", extras = ["toml"]}
-esbonio = "^0.14.1"
-fastapi = "^0.85.0"
+black = "^22.3.0"
+coverage = {version = "^7.2.7", extras = ["toml"]}
+esbonio = "^0.16.1"
+fastapi = "^0.100.1"
 flake8 = "^5.0.4"
+furo = "^2022"
 isort = "^5.9.3"
-mypy = "^0.982"
-prometheus-client = "^0.16.0"
-pytest = "^7.1.3"
-pytest-asyncio = "^0.19.0"
-pytest-cov = "^4.0.0"
-redis = "^4.3.4"
-sphinx-rtd-theme = "^1.0.0"
+mypy = "^1.4.1"
+prometheus-client = "^0.17.1"
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.1.0"
+redis = "^4.6.0"
+sphinx = "^4.2.0"
+sphinx-autodoc-typehints = "^1.12.0"
 starlette-zipkin = "^0.3.0"
-tomlkit = "^0.11.5"
-types-redis = "^4.3.21"
-types-setuptools = "^65.4.0"
+tomlkit = "^0.12.1"
+types-redis = "^4.6.0"
+types-setuptools = "^68.0.0"
 unasync = "^0.5.0"
 uvicorn = "^0.18.3"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 norecursedirs = "tests/unittests/scanned_resources"
 testpaths = ["tests"]
@@ -79,13 +79,13 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "if TYPE_CHECKING:",
   "except ImportError:",
   "except pkg_resources.DistributionNotFound:",
   "\\s+\\.\\.\\.$",
-  "# coverage-ignore",
+  "# coverage: ignore",
 ]
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.2.0"]
```

### Comparing `blacksmith-2.3.2/src/blacksmith/__init__.py` & `blacksmith-2.3.3/src/blacksmith/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/error.py` & `blacksmith-2.3.3/src/blacksmith/domain/error.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/exceptions.py` & `blacksmith-2.3.3/src/blacksmith/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/model/__init__.py` & `blacksmith-2.3.3/src/blacksmith/domain/model/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/model/http.py` & `blacksmith-2.3.3/src/blacksmith/domain/model/http.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/model/middleware/circuit_breaker.py` & `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/model/middleware/http_cache.py` & `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/model/middleware/prometheus.py` & `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/model/middleware/zipkin.py` & `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/model/params.py` & `blacksmith-2.3.3/src/blacksmith/domain/model/params.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/registry.py` & `blacksmith-2.3.3/src/blacksmith/domain/registry.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/scanner.py` & `blacksmith-2.3.3/src/blacksmith/domain/scanner.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/domain/typing.py` & `blacksmith-2.3.3/src/blacksmith/domain/typing.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_async/__init__.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_async/auth.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_async/auth.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_async/base.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_async/base.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_async/circuit_breaker.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_async/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_async/http_cache.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_async/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_async/prometheus.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_async/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_async/zipkin.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_async/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_sync/__init__.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_sync/auth.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_sync/auth.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_sync/base.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_sync/base.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_sync/circuit_breaker.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_sync/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_sync/http_cache.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_sync/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_sync/prometheus.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_sync/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/middleware/_sync/zipkin.py` & `blacksmith-2.3.3/src/blacksmith/middleware/_sync/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/sd/_async/adapters/consul.py` & `blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/consul.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/sd/_async/adapters/router.py` & `blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/router.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/sd/_async/adapters/static.py` & `blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/static.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/sd/_sync/adapters/consul.py` & `blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/consul.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/sd/_sync/adapters/router.py` & `blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/router.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/sd/_sync/adapters/static.py` & `blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/static.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/service/_async/adapters/httpx.py` & `blacksmith-2.3.3/src/blacksmith/service/_async/adapters/httpx.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/service/_async/client.py` & `blacksmith-2.3.3/src/blacksmith/service/_async/client.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/service/_async/route_proxy.py` & `blacksmith-2.3.3/src/blacksmith/service/_async/route_proxy.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/service/_sync/adapters/httpx.py` & `blacksmith-2.3.3/src/blacksmith/service/_sync/adapters/httpx.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/service/_sync/client.py` & `blacksmith-2.3.3/src/blacksmith/service/_sync/client.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/src/blacksmith/service/_sync/route_proxy.py` & `blacksmith-2.3.3/src/blacksmith/service/_sync/route_proxy.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.2/PKG-INFO` & `blacksmith-2.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksmith
-Version: 2.3.2
+Version: 2.3.3
 Summary: REST API Client designed for microservices
 Home-page: https://github.com/mardiros/blacksmith
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,30 +19,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: http-cache-async
 Provides-Extra: http-cache-sync
 Provides-Extra: prometheus
-Requires-Dist: aioredis (>=2.0.0,<3.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: prometheus-client (>=0.16.0,<0.17.0) ; extra == "prometheus"
-Requires-Dist: purgatory (>=1.0.2,<2.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: prometheus-client (>=0.17.1,<0.18.0) ; extra == "prometheus"
+Requires-Dist: purgatory (>=1.0.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: result (>=0.10.0,<0.11.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: result (>=0.11.0,<0.12.0)
+Requires-Dist: typing-extensions (>=4.7.0,<5.0.0)
 Project-URL: Repository, https://github.com/mardiros/blacksmith
 Description-Content-Type: text/x-rst
 
 Blacksmith
 ==========
 
-.. image:: https://readthedocs.org/projects/python-blacksmith/badge/?version=latest
-   :target: https://python-blacksmith.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
+.. image:: https://github.com/mardiros/blacksmith/actions/workflows/gh-pages.yml/badge.svg
+   :target: https://mardiros.github.io/blacksmith/user/introduction.html
+   :alt: Documentation
 
 .. image:: https://github.com/mardiros/blacksmith/actions/workflows/main.yml/badge.svg
    :target: https://github.com/mardiros/blacksmith/actions/workflows/main.yml
    :alt: Continuous Integration
 
 .. image:: https://codecov.io/gh/mardiros/blacksmith/branch/master/graph/badge.svg?token=17KAC0LW9H
    :target: https://codecov.io/gh/mardiros/blacksmith
@@ -135,9 +134,14 @@
 
 
 Read More
 ---------
 
 You can read the `full documentation of this library here`_.
 
-.. _`full documentation of this library here`: https://python-blacksmith.readthedocs.io/en/latest/user/introduction.html
+.. _`full documentation of this library here`: https://mardiros.github.io/blacksmith/user/introduction.html
+
+.. important::
+
+   | The documentation has been moved to github pages.
+   | The documentation under readthedocs is obsolete.
```

