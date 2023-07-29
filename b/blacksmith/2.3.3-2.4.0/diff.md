# Comparing `tmp/blacksmith-2.3.3.tar.gz` & `tmp/blacksmith-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksmith-2.3.3.tar", max compression
+gzip compressed data, was "blacksmith-2.4.0.tar", max compression
```

## Comparing `blacksmith-2.3.3.tar` & `blacksmith-2.4.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1528 2022-01-06 07:33:14.770656 blacksmith-2.3.3/LICENSE
--rw-r--r--   0        0        0     3878 2023-07-23 15:11:35.288448 blacksmith-2.3.3/README.rst
--rw-r--r--   0        0        0     2209 2023-07-29 13:25:37.098513 blacksmith-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     4003 2022-10-11 10:09:17.048567 blacksmith-2.3.3/src/blacksmith/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 07:19:10.263612 blacksmith-2.3.3/src/blacksmith/adapters/__init__.py
--rw-r--r--   0        0        0        0 2021-10-23 20:54:22.320117 blacksmith-2.3.3/src/blacksmith/domain/__init__.py
--rw-r--r--   0        0        0      813 2022-10-11 10:09:17.048567 blacksmith-2.3.3/src/blacksmith/domain/error.py
--rw-r--r--   0        0        0     3665 2022-10-10 18:11:37.257590 blacksmith-2.3.3/src/blacksmith/domain/exceptions.py
--rw-r--r--   0        0        0     1043 2022-10-11 10:09:17.048567 blacksmith-2.3.3/src/blacksmith/domain/model/__init__.py
--rw-r--r--   0        0        0     3278 2022-10-09 05:40:41.790453 blacksmith-2.3.3/src/blacksmith/domain/model/http.py
--rw-r--r--   0        0        0        0 2022-01-20 21:42:27.593890 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/__init__.py
--rw-r--r--   0        0        0     1201 2022-02-04 22:04:27.203840 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/circuit_breaker.py
--rw-r--r--   0        0        0     4365 2022-01-20 21:42:27.593890 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/http_cache.py
--rw-r--r--   0        0        0     2993 2022-02-07 21:56:12.757093 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/prometheus.py
--rw-r--r--   0        0        0     1174 2022-01-24 20:07:20.433938 blacksmith-2.3.3/src/blacksmith/domain/model/middleware/zipkin.py
--rw-r--r--   0        0        0    14313 2023-05-10 11:48:05.014686 blacksmith-2.3.3/src/blacksmith/domain/model/params.py
--rw-r--r--   0        0        0     5095 2022-10-10 21:39:42.618378 blacksmith-2.3.3/src/blacksmith/domain/registry.py
--rw-r--r--   0        0        0      983 2022-01-18 22:18:53.863644 blacksmith-2.3.3/src/blacksmith/domain/scanner.py
--rw-r--r--   0        0        0      885 2022-10-07 21:02:49.023029 blacksmith-2.3.3/src/blacksmith/domain/typing.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/middleware/__init__.py
--rw-r--r--   0        0        0      716 2022-01-22 22:10:58.887280 blacksmith-2.3.3/src/blacksmith/middleware/_async/__init__.py
--rw-r--r--   0        0        0      802 2022-01-22 22:10:58.887280 blacksmith-2.3.3/src/blacksmith/middleware/_async/auth.py
--rw-r--r--   0        0        0     1472 2022-10-07 21:02:43.642963 blacksmith-2.3.3/src/blacksmith/middleware/_async/base.py
--rw-r--r--   0        0        0     2330 2022-01-22 22:10:58.887280 blacksmith-2.3.3/src/blacksmith/middleware/_async/circuit_breaker.py
--rw-r--r--   0        0        0     5933 2023-05-11 07:19:10.263612 blacksmith-2.3.3/src/blacksmith/middleware/_async/http_cache.py
--rw-r--r--   0        0        0     2436 2022-02-04 22:05:35.793843 blacksmith-2.3.3/src/blacksmith/middleware/_async/prometheus.py
--rw-r--r--   0        0        0     2869 2022-01-24 20:07:20.433938 blacksmith-2.3.3/src/blacksmith/middleware/_async/zipkin.py
--rw-r--r--   0        0        0      696 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/__init__.py
--rw-r--r--   0        0        0      797 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/auth.py
--rw-r--r--   0        0        0     1434 2023-07-29 13:25:25.858473 blacksmith-2.3.3/src/blacksmith/middleware/_sync/base.py
--rw-r--r--   0        0        0     2284 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/circuit_breaker.py
--rw-r--r--   0        0        0     5827 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/middleware/_sync/http_cache.py
--rw-r--r--   0        0        0     2418 2023-07-29 13:25:25.855140 blacksmith-2.3.3/src/blacksmith/middleware/_sync/prometheus.py
--rw-r--r--   0        0        0     2851 2023-07-29 13:25:25.858473 blacksmith-2.3.3/src/blacksmith/middleware/_sync/zipkin.py
--rw-r--r--   0        0        0        0 2022-01-18 22:18:53.866978 blacksmith-2.3.3/src/blacksmith/py.typed
--rw-r--r--   0        0        0       24 2021-10-24 11:21:34.426587 blacksmith-2.3.3/src/blacksmith/sd/__init__.py
--rw-r--r--   0        0        0      334 2022-01-25 07:30:46.663983 blacksmith-2.3.3/src/blacksmith/sd/_async/__init__.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/__init__.py
--rw-r--r--   0        0        0     5660 2022-11-15 09:34:44.244184 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/consul.py
--rw-r--r--   0        0        0     1693 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/router.py
--rw-r--r--   0        0        0     1010 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/static.py
--rw-r--r--   0        0        0      317 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/sd/_async/base.py
--rw-r--r--   0        0        0      326 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/__init__.py
--rw-r--r--   0        0        0     5614 2023-07-29 13:25:25.865140 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/consul.py
--rw-r--r--   0        0        0     1684 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/router.py
--rw-r--r--   0        0        0     1001 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/static.py
--rw-r--r--   0        0        0      310 2023-07-29 13:25:25.861807 blacksmith-2.3.3/src/blacksmith/sd/_sync/base.py
--rw-r--r--   0        0        0        0 2021-10-23 21:02:59.310144 blacksmith-2.3.3/src/blacksmith/service/__init__.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/service/_async/__init__.py
--rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/service/_async/adapters/__init__.py
--rw-r--r--   0        0        0     2391 2023-05-10 11:48:05.014686 blacksmith-2.3.3/src/blacksmith/service/_async/adapters/httpx.py
--rw-r--r--   0        0        0      420 2022-10-08 15:37:33.544758 blacksmith-2.3.3/src/blacksmith/service/_async/base.py
--rw-r--r--   0        0        0     5903 2022-10-11 05:00:19.426732 blacksmith-2.3.3/src/blacksmith/service/_async/client.py
--rw-r--r--   0        0        0    12871 2022-10-10 21:39:42.621711 blacksmith-2.3.3/src/blacksmith/service/_async/route_proxy.py
--rw-r--r--   0        0        0        0 2023-07-29 13:25:25.865140 blacksmith-2.3.3/src/blacksmith/service/_sync/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 13:25:25.875140 blacksmith-2.3.3/src/blacksmith/service/_sync/adapters/__init__.py
--rw-r--r--   0        0        0     2368 2023-07-29 13:25:25.875140 blacksmith-2.3.3/src/blacksmith/service/_sync/adapters/httpx.py
--rw-r--r--   0        0        0      417 2023-07-29 13:25:25.865140 blacksmith-2.3.3/src/blacksmith/service/_sync/base.py
--rw-r--r--   0        0        0     5837 2023-07-29 13:25:28.985151 blacksmith-2.3.3/src/blacksmith/service/_sync/client.py
--rw-r--r--   0        0        0    12490 2023-07-29 13:25:29.061818 blacksmith-2.3.3/src/blacksmith/service/_sync/route_proxy.py
--rw-r--r--   0        0        0      121 2022-01-06 07:13:35.813927 blacksmith-2.3.3/src/blacksmith/service/ports.py
--rw-r--r--   0        0        0      450 2022-01-19 08:38:32.683866 blacksmith-2.3.3/src/blacksmith/typing.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 blacksmith-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1528 2022-01-06 07:33:14.770656 blacksmith-2.4.0/LICENSE
+-rw-r--r--   0        0        0     3878 2023-07-23 15:11:35.288448 blacksmith-2.4.0/README.rst
+-rw-r--r--   0        0        0     2237 2023-07-29 17:19:30.890915 blacksmith-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4003 2022-10-11 10:09:17.048567 blacksmith-2.4.0/src/blacksmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 07:19:10.263612 blacksmith-2.4.0/src/blacksmith/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-23 20:54:22.320117 blacksmith-2.4.0/src/blacksmith/domain/__init__.py
+-rw-r--r--   0        0        0      813 2022-10-11 10:09:17.048567 blacksmith-2.4.0/src/blacksmith/domain/error.py
+-rw-r--r--   0        0        0     3665 2022-10-10 18:11:37.257590 blacksmith-2.4.0/src/blacksmith/domain/exceptions.py
+-rw-r--r--   0        0        0     1043 2022-10-11 10:09:17.048567 blacksmith-2.4.0/src/blacksmith/domain/model/__init__.py
+-rw-r--r--   0        0        0     3278 2022-10-09 05:40:41.790453 blacksmith-2.4.0/src/blacksmith/domain/model/http.py
+-rw-r--r--   0        0        0        0 2022-01-20 21:42:27.593890 blacksmith-2.4.0/src/blacksmith/domain/model/middleware/__init__.py
+-rw-r--r--   0        0        0     1201 2022-02-04 22:04:27.203840 blacksmith-2.4.0/src/blacksmith/domain/model/middleware/circuit_breaker.py
+-rw-r--r--   0        0        0     4365 2022-01-20 21:42:27.593890 blacksmith-2.4.0/src/blacksmith/domain/model/middleware/http_cache.py
+-rw-r--r--   0        0        0     2993 2022-02-07 21:56:12.757093 blacksmith-2.4.0/src/blacksmith/domain/model/middleware/prometheus.py
+-rw-r--r--   0        0        0     1174 2022-01-24 20:07:20.433938 blacksmith-2.4.0/src/blacksmith/domain/model/middleware/zipkin.py
+-rw-r--r--   0        0        0    14973 2023-07-29 16:55:21.828053 blacksmith-2.4.0/src/blacksmith/domain/model/params.py
+-rw-r--r--   0        0        0     5095 2022-10-10 21:39:42.618378 blacksmith-2.4.0/src/blacksmith/domain/registry.py
+-rw-r--r--   0        0        0      983 2022-01-18 22:18:53.863644 blacksmith-2.4.0/src/blacksmith/domain/scanner.py
+-rw-r--r--   0        0        0      885 2022-10-07 21:02:49.023029 blacksmith-2.4.0/src/blacksmith/domain/typing.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/middleware/__init__.py
+-rw-r--r--   0        0        0      716 2022-01-22 22:10:58.887280 blacksmith-2.4.0/src/blacksmith/middleware/_async/__init__.py
+-rw-r--r--   0        0        0      802 2022-01-22 22:10:58.887280 blacksmith-2.4.0/src/blacksmith/middleware/_async/auth.py
+-rw-r--r--   0        0        0     1472 2022-10-07 21:02:43.642963 blacksmith-2.4.0/src/blacksmith/middleware/_async/base.py
+-rw-r--r--   0        0        0     2330 2022-01-22 22:10:58.887280 blacksmith-2.4.0/src/blacksmith/middleware/_async/circuit_breaker.py
+-rw-r--r--   0        0        0     5933 2023-05-11 07:19:10.263612 blacksmith-2.4.0/src/blacksmith/middleware/_async/http_cache.py
+-rw-r--r--   0        0        0     2436 2022-02-04 22:05:35.793843 blacksmith-2.4.0/src/blacksmith/middleware/_async/prometheus.py
+-rw-r--r--   0        0        0     2869 2022-01-24 20:07:20.433938 blacksmith-2.4.0/src/blacksmith/middleware/_async/zipkin.py
+-rw-r--r--   0        0        0      696 2023-07-29 17:19:19.344202 blacksmith-2.4.0/src/blacksmith/middleware/_sync/__init__.py
+-rw-r--r--   0        0        0      797 2023-07-29 17:19:19.347535 blacksmith-2.4.0/src/blacksmith/middleware/_sync/auth.py
+-rw-r--r--   0        0        0     1434 2023-07-29 17:19:19.347535 blacksmith-2.4.0/src/blacksmith/middleware/_sync/base.py
+-rw-r--r--   0        0        0     2284 2023-07-29 17:19:19.347535 blacksmith-2.4.0/src/blacksmith/middleware/_sync/circuit_breaker.py
+-rw-r--r--   0        0        0     5827 2023-07-29 17:19:19.350868 blacksmith-2.4.0/src/blacksmith/middleware/_sync/http_cache.py
+-rw-r--r--   0        0        0     2418 2023-07-29 17:19:19.344202 blacksmith-2.4.0/src/blacksmith/middleware/_sync/prometheus.py
+-rw-r--r--   0        0        0     2851 2023-07-29 17:19:19.347535 blacksmith-2.4.0/src/blacksmith/middleware/_sync/zipkin.py
+-rw-r--r--   0        0        0        0 2022-01-18 22:18:53.866978 blacksmith-2.4.0/src/blacksmith/py.typed
+-rw-r--r--   0        0        0       24 2021-10-24 11:21:34.426587 blacksmith-2.4.0/src/blacksmith/sd/__init__.py
+-rw-r--r--   0        0        0      334 2022-01-25 07:30:46.663983 blacksmith-2.4.0/src/blacksmith/sd/_async/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/sd/_async/adapters/__init__.py
+-rw-r--r--   0        0        0     5666 2023-07-29 16:55:21.828053 blacksmith-2.4.0/src/blacksmith/sd/_async/adapters/consul.py
+-rw-r--r--   0        0        0     1693 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/sd/_async/adapters/router.py
+-rw-r--r--   0        0        0     1010 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/sd/_async/adapters/static.py
+-rw-r--r--   0        0        0      317 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/sd/_async/base.py
+-rw-r--r--   0        0        0      326 2023-07-29 17:19:19.354202 blacksmith-2.4.0/src/blacksmith/sd/_sync/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:19:19.354202 blacksmith-2.4.0/src/blacksmith/sd/_sync/adapters/__init__.py
+-rw-r--r--   0        0        0     5620 2023-07-29 17:19:19.357535 blacksmith-2.4.0/src/blacksmith/sd/_sync/adapters/consul.py
+-rw-r--r--   0        0        0     1684 2023-07-29 17:19:19.354202 blacksmith-2.4.0/src/blacksmith/sd/_sync/adapters/router.py
+-rw-r--r--   0        0        0     1001 2023-07-29 17:19:19.354202 blacksmith-2.4.0/src/blacksmith/sd/_sync/adapters/static.py
+-rw-r--r--   0        0        0      310 2023-07-29 17:19:19.350868 blacksmith-2.4.0/src/blacksmith/sd/_sync/base.py
+-rw-r--r--   0        0        0        0 2021-10-23 21:02:59.310144 blacksmith-2.4.0/src/blacksmith/service/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/service/_async/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/service/_async/adapters/__init__.py
+-rw-r--r--   0        0        0     2391 2023-05-10 11:48:05.014686 blacksmith-2.4.0/src/blacksmith/service/_async/adapters/httpx.py
+-rw-r--r--   0        0        0      420 2022-10-08 15:37:33.544758 blacksmith-2.4.0/src/blacksmith/service/_async/base.py
+-rw-r--r--   0        0        0     5903 2022-10-11 05:00:19.426732 blacksmith-2.4.0/src/blacksmith/service/_async/client.py
+-rw-r--r--   0        0        0    12871 2022-10-10 21:39:42.621711 blacksmith-2.4.0/src/blacksmith/service/_async/route_proxy.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:19:19.357535 blacksmith-2.4.0/src/blacksmith/service/_sync/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:19:19.364202 blacksmith-2.4.0/src/blacksmith/service/_sync/adapters/__init__.py
+-rw-r--r--   0        0        0     2368 2023-07-29 17:19:19.367535 blacksmith-2.4.0/src/blacksmith/service/_sync/adapters/httpx.py
+-rw-r--r--   0        0        0      417 2023-07-29 17:19:19.357535 blacksmith-2.4.0/src/blacksmith/service/_sync/base.py
+-rw-r--r--   0        0        0     5837 2023-07-29 17:19:22.597548 blacksmith-2.4.0/src/blacksmith/service/_sync/client.py
+-rw-r--r--   0        0        0    12490 2023-07-29 17:19:22.744216 blacksmith-2.4.0/src/blacksmith/service/_sync/route_proxy.py
+-rw-r--r--   0        0        0      121 2022-01-06 07:13:35.813927 blacksmith-2.4.0/src/blacksmith/service/ports.py
+-rw-r--r--   0        0        0      450 2022-01-19 08:38:32.683866 blacksmith-2.4.0/src/blacksmith/typing.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 blacksmith-2.4.0/PKG-INFO
```

### Comparing `blacksmith-2.3.3/LICENSE` & `blacksmith-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/README.rst` & `blacksmith-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/pyproject.toml` & `blacksmith-2.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 description = "REST API Client designed for microservices"
 homepage = "https://github.com/mardiros/blacksmith"
 license = "BSD-derived"
 name = "blacksmith"
 
 readme = "README.rst"
 repository = "https://github.com/mardiros/blacksmith"
-version = "2.3.3"
+version = "2.4.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httpx = "^0.24.1"
 prometheus-client = {version = "^0.17.1", optional = true}
 purgatory = "^1.0.3"
-pydantic = "^1.10.7"
+pydantic = ">=1.10.12, <3"
 typing-extensions = "^4.7.0"
 result = "^0.11.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 http_cache_async = ["redis"]
 http_cache_sync = ["redis"]
 prometheus = ["prometheus-client"]
 
 [tool.poetry.dev-dependencies]
```

### Comparing `blacksmith-2.3.3/src/blacksmith/__init__.py` & `blacksmith-2.4.0/src/blacksmith/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/error.py` & `blacksmith-2.4.0/src/blacksmith/domain/error.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/exceptions.py` & `blacksmith-2.4.0/src/blacksmith/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/model/__init__.py` & `blacksmith-2.4.0/src/blacksmith/domain/model/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/model/http.py` & `blacksmith-2.4.0/src/blacksmith/domain/model/http.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/circuit_breaker.py` & `blacksmith-2.4.0/src/blacksmith/domain/model/middleware/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/http_cache.py` & `blacksmith-2.4.0/src/blacksmith/domain/model/middleware/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/prometheus.py` & `blacksmith-2.4.0/src/blacksmith/domain/model/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/model/middleware/zipkin.py` & `blacksmith-2.4.0/src/blacksmith/domain/model/middleware/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/model/params.py` & `blacksmith-2.4.0/src/blacksmith/domain/model/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,23 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from pydantic import BaseModel, Field
-from pydantic.json import ENCODERS_BY_TYPE
+
+# assume we can use deprecated stuff until we support both version
+try:
+    # pydantic 2
+    from pydantic.deprecated.json import ENCODERS_BY_TYPE  # type: ignore
+except ImportError:  # type: ignore # coverage: ignore
+    # pydantic 1
+    from pydantic.json import ENCODERS_BY_TYPE  # type: ignore  # coverage: ignore
+
 from result import Result
 from result.result import F, U
 
 from blacksmith.domain.error import AbstractErrorParser, TError_co
 
 if TYPE_CHECKING:
     from pydantic.typing import IntStr
@@ -44,24 +52,38 @@
 
 PATH: HttpLocation = "path"
 HEADER: HttpLocation = "headers"
 QUERY: HttpLocation = "querystring"
 BODY: HttpLocation = "body"
 
 
+# in pydantic 2, the extra keys for location is deprecated,
+# the json_schema_extra should be used.
+
 PathInfoField = partial(Field, location=PATH)
 """Declare field that are serialized to the path info."""
 HeaderField = partial(Field, location=HEADER)
 """Declare field that are serialized in http request header."""
 QueryStringField = partial(Field, location=QUERY)
 """Declare field that are serialized in the http querystring."""
 PostBodyField = partial(Field, location=BODY)
 """Declare field that are serialized in the json document."""
 
 
+def get_location(field: Any) -> HttpLocation:
+    # field is of type FieldInfo, which differ on pydantic 2 and pydantic 1
+    if hasattr(field, "json_schema_extra"):
+        extra = field.json_schema_extra
+    elif hasattr(field, "field_info"):
+        extra = field.field_info.extra
+    else:
+        raise ValueError(f"{field} is not a FieldInfo")
+    return extra["location"]
+
+
 class JSONEncoder(json.JSONEncoder):
     def default(self, o: Any) -> Any:
         for typ, serializer in ENCODERS_BY_TYPE.items():
             if isinstance(o, typ):
                 return serializer(o)
         return super(JSONEncoder, self).default(o)
 
@@ -106,20 +128,17 @@
         req = HTTPRequest(method=method, url_pattern=url_pattern)
         fields_by_loc: Dict[HttpLocation, Dict[IntStr, Any]] = {
             HEADER: {},
             PATH: {},
             QUERY: {},
             BODY: {},
         }
-        for field in self.__fields__.values():
-            loc = cast(
-                HttpLocation,
-                field.field_info.extra["location"],  # type: ignore
-            )
-            fields_by_loc[loc].update({field.name: ...})
+        for name, field in self.__fields__.items():
+            loc = get_location(field)
+            fields_by_loc[loc].update({name: ...})
 
         headers = serialize_part(self, fields_by_loc[HEADER])
         req.headers = {key: str(val) for key, val in headers.items()}
         req.path = serialize_part(self, fields_by_loc[PATH])
         req.querystring = cast(
             Dict[str, Union[simpletypes, List[simpletypes]]],
             serialize_part(self, fields_by_loc[QUERY]),
```

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/registry.py` & `blacksmith-2.4.0/src/blacksmith/domain/registry.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/scanner.py` & `blacksmith-2.4.0/src/blacksmith/domain/scanner.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/domain/typing.py` & `blacksmith-2.4.0/src/blacksmith/domain/typing.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_async/__init__.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_async/auth.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_async/auth.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_async/base.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_async/base.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_async/circuit_breaker.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_async/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_async/http_cache.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_async/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_async/prometheus.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_async/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_async/zipkin.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_async/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_sync/__init__.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_sync/auth.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_sync/auth.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_sync/base.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_sync/base.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_sync/circuit_breaker.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_sync/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_sync/http_cache.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_sync/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_sync/prometheus.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_sync/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/middleware/_sync/zipkin.py` & `blacksmith-2.4.0/src/blacksmith/middleware/_sync/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/consul.py` & `blacksmith-2.4.0/src/blacksmith/sd/_async/adapters/consul.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 class Service(Response):
     """Consul Service response."""
 
     node_address: str = Field(alias="Address")
     """IP address of the Consul node on which the service is registered."""
-    service_address: Optional[str] = Field(alias="ServiceAddress")
+    service_address: Optional[str] = Field(None, alias="ServiceAddress")
     """IP address of the service host. if empty, node address is used."""
     port: int = Field(alias="ServicePort")
     """TCP Port of an instance that host the service."""
 
     @property
     def address(self) -> str:
         return self.service_address or self.node_address
```

### Comparing `blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/router.py` & `blacksmith-2.4.0/src/blacksmith/sd/_async/adapters/router.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/sd/_async/adapters/static.py` & `blacksmith-2.4.0/src/blacksmith/sd/_async/adapters/static.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/consul.py` & `blacksmith-2.4.0/src/blacksmith/sd/_sync/adapters/consul.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 class Service(Response):
     """Consul Service response."""
 
     node_address: str = Field(alias="Address")
     """IP address of the Consul node on which the service is registered."""
-    service_address: Optional[str] = Field(alias="ServiceAddress")
+    service_address: Optional[str] = Field(None, alias="ServiceAddress")
     """IP address of the service host. if empty, node address is used."""
     port: int = Field(alias="ServicePort")
     """TCP Port of an instance that host the service."""
 
     @property
     def address(self) -> str:
         return self.service_address or self.node_address
```

### Comparing `blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/router.py` & `blacksmith-2.4.0/src/blacksmith/sd/_sync/adapters/router.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/sd/_sync/adapters/static.py` & `blacksmith-2.4.0/src/blacksmith/sd/_sync/adapters/static.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/service/_async/adapters/httpx.py` & `blacksmith-2.4.0/src/blacksmith/service/_async/adapters/httpx.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/service/_async/client.py` & `blacksmith-2.4.0/src/blacksmith/service/_async/client.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/service/_async/route_proxy.py` & `blacksmith-2.4.0/src/blacksmith/service/_async/route_proxy.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/service/_sync/adapters/httpx.py` & `blacksmith-2.4.0/src/blacksmith/service/_sync/adapters/httpx.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/service/_sync/client.py` & `blacksmith-2.4.0/src/blacksmith/service/_sync/client.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/src/blacksmith/service/_sync/route_proxy.py` & `blacksmith-2.4.0/src/blacksmith/service/_sync/route_proxy.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.3.3/PKG-INFO` & `blacksmith-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksmith
-Version: 2.3.3
+Version: 2.4.0
 Summary: REST API Client designed for microservices
 Home-page: https://github.com/mardiros/blacksmith
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -22,15 +22,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: http-cache-async
 Provides-Extra: http-cache-sync
 Provides-Extra: prometheus
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: prometheus-client (>=0.17.1,<0.18.0) ; extra == "prometheus"
 Requires-Dist: purgatory (>=1.0.3,<2.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=1.10.12,<3)
+Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: result (>=0.11.0,<0.12.0)
 Requires-Dist: typing-extensions (>=4.7.0,<5.0.0)
 Project-URL: Repository, https://github.com/mardiros/blacksmith
 Description-Content-Type: text/x-rst
 
 Blacksmith
 ==========
```

