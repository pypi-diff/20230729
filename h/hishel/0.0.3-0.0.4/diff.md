# Comparing `tmp/hishel-0.0.3.tar.gz` & `tmp/hishel-0.0.4.tar.gz`

## Comparing `hishel-0.0.3.tar` & `hishel-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hishel-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 hishel-0.0.3/README.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/__about__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/__init__.py
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_controller.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_exceptions.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_files.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_serializers.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_synchronization.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/py.typed
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_client.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_mock.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_pool.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_storages.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_async/_transports.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_client.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_mock.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_pool.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_storages.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 hishel-0.0.3/hishel/_sync/_transports.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.3/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.3/LICENSE
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 hishel-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hishel-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 hishel-0.0.4/README.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/__about__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/__init__.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_controller.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_exceptions.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_files.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_serializers.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_synchronization.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/py.typed
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_client.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_mock.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_pool.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_storages.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_transports.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_client.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_mock.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_pool.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_storages.py
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_transports.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 hishel-0.0.4/PKG-INFO
```

### Comparing `hishel-0.0.3/README.md` & `hishel-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hishel.svg)](https://pypi.org/project/hishel)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hishel.svg)](https://pypi.org/project/hishel)
 ![PyPI - License](https://img.shields.io/pypi/l/hishel)
 ![Codecov](https://img.shields.io/codecov/c/github/karosis88/hishel)
 
-
 -----
 
 **Hishel (հիշել, remember)** is a library that implements HTTP Caching for [HTTPX](https://github.com/encode/httpx) and [HTTP Core](https://github.com/encode/httpcore) libraries in accordance with **RFC 9111**, the most recent caching specification.
 
 ## Features
 
 - 💾 Persistence: Responses are cached in the [**persistent memory**](https://en.m.wikipedia.org/wiki/Persistent_memory) for later use.
 - 🤲 Compatibility: It is completely compatible with your existing transports or connection pools, **whether they are default, custom, or provided by third-party libraries.**
 - 🤗 Easy to use: You continue to use the httpx and httpcore interfaces. **Can be integrated with no changes to the code.**
 - 🧠 Smart: Attempts to clearly implement RFC 9111, understands `Vary`, `Etag`, `Last-Modified`,  `Cache-Control`, and `Expires` headers, and **handles response re-validation automatically**.
-- ⚙️ Configurable: You can specify the **backend** where the responses should be stored, the **serializer**, and you can write your own **backends and serializers**. You can also specify which parts of RFC 9111 **should be ignored and which should not**, for example, you can explicitly disable stale responses for your safety or enable re-validation for each response before using it. 
-- 🚀 Very fast: When **IO is not required**, your requests are even faster.
+- ⚙️ Configurable: You have complete control over how the responses are stored and serialized, and there is built-in support for filesystem and redis backends.
+- 🚀 Very fast: Your requests will be even faster if there are **no IO operations**.
 
+## Documentation
+Go through the [Hishel documentation](https://karosis88.github.io/hishel/).
 
 ## QuickStart
 
 Install `Hishel` using pip:
 ``` shell
 $ pip install hishel
 ```
@@ -87,15 +88,16 @@
 pool.request("GET", "https://www.github.com")
 pool.request("GET", "https://www.github.com")  # takes from the cache
 
 ```
 
 ## How and where are the responses saved?
 
-The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a variety of built-in storage options, but the default storage is a [filesystem storage](TODO). You can switch the storage to another one that `Hishel` offers or, if necessary, write your own; for more information, see the storage documentation.
+The responses are stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/#storages).
+You have complete control over them; you can change storage or even write your own if necessary.
 
 
 ## Contributing
 
 `Hishel` is a powerful tool, but it is also a new project with potential flaws, so we welcome contributions!
 
 You can open the pull request by following these instructions if you want to improve `Hishel`. 💓
```

#### html2text {}

```diff
@@ -12,40 +12,38 @@
 memory**](https://en.m.wikipedia.org/wiki/Persistent_memory) for later use. -
 ð¤² Compatibility: It is completely compatible with your existing transports
 or connection pools, **whether they are default, custom, or provided by third-
 party libraries.** - ð¤ Easy to use: You continue to use the httpx and
 httpcore interfaces. **Can be integrated with no changes to the code.** - ð§ 
 Smart: Attempts to clearly implement RFC 9111, understands `Vary`, `Etag`,
 `Last-Modified`, `Cache-Control`, and `Expires` headers, and **handles response
-re-validation automatically**. - âï¸ Configurable: You can specify the
-**backend** where the responses should be stored, the **serializer**, and you
-can write your own **backends and serializers**. You can also specify which
-parts of RFC 9111 **should be ignored and which should not**, for example, you
-can explicitly disable stale responses for your safety or enable re-validation
-for each response before using it. - ð Very fast: When **IO is not
-required**, your requests are even faster. ## QuickStart Install `Hishel` using
-pip: ``` shell $ pip install hishel ``` Let's begin with an example of a httpx
-client. ```python import hishel with hishel.CacheClient() as client: client.get
-("https://www.github.com") client.get("https://www.github.com") # takes from
-the cache (very fast!) ``` or in asynchronous context ```python import hishel
-async with hishel.AsyncCacheClient() as client: await client.get("https://
-www.github.com") await client.get("https://www.github.com") # takes from the
-cache ``` ## HTTPX and HTTP Core `Hishel` also supports the transports of
-`HTTPX` and the connection pools of `HTTP Core`. `Hishel` respects existing
-**transports** and **connection pools** and can therefore work **on top of
-them**, making hishel a very **compatible and flexible library**.
-**Transports** example: ``` python import httpx import hishel transport =
-httpx.HTTPTransport() cache_transport = hishel.CacheTransport
-(transport=transport) req = httpx.Request("GET", "https://www.github.com")
-cache_transport.handle_request(req) cache_transport.handle_request(req) # takes
-from the cache ``` **Connection Pool** example: ```python import httpcore
-import hishel pool = hishel.CacheConnectionPool(pool=httpcore.ConnectionPool())
-pool.request("GET", "https://www.github.com") pool.request("GET", "https://
-www.github.com") # takes from the cache ``` ## How and where are the responses
-saved? The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a
-variety of built-in storage options, but the default storage is a [filesystem
-storage](TODO). You can switch the storage to another one that `Hishel` offers
-or, if necessary, write your own; for more information, see the storage
-documentation. ## Contributing `Hishel` is a powerful tool, but it is also a
-new project with potential flaws, so we welcome contributions! You can open the
-pull request by following these instructions if you want to improve `Hishel`.
-ð - Fork the project. - Make change. - Open the pull request.
+re-validation automatically**. - âï¸ Configurable: You have complete control
+over how the responses are stored and serialized, and there is built-in support
+for filesystem and redis backends. - ð Very fast: Your requests will be even
+faster if there are **no IO operations**. ## Documentation Go through the
+[Hishel documentation](https://karosis88.github.io/hishel/). ## QuickStart
+Install `Hishel` using pip: ``` shell $ pip install hishel ``` Let's begin with
+an example of a httpx client. ```python import hishel with hishel.CacheClient()
+as client: client.get("https://www.github.com") client.get("https://
+www.github.com") # takes from the cache (very fast!) ``` or in asynchronous
+context ```python import hishel async with hishel.AsyncCacheClient() as client:
+await client.get("https://www.github.com") await client.get("https://
+www.github.com") # takes from the cache ``` ## HTTPX and HTTP Core `Hishel`
+also supports the transports of `HTTPX` and the connection pools of `HTTP
+Core`. `Hishel` respects existing **transports** and **connection pools** and
+can therefore work **on top of them**, making hishel a very **compatible and
+flexible library**. **Transports** example: ``` python import httpx import
+hishel transport = httpx.HTTPTransport() cache_transport =
+hishel.CacheTransport(transport=transport) req = httpx.Request("GET", "https://
+www.github.com") cache_transport.handle_request(req)
+cache_transport.handle_request(req) # takes from the cache ``` **Connection
+Pool** example: ```python import httpcore import hishel pool =
+hishel.CacheConnectionPool(pool=httpcore.ConnectionPool()) pool.request("GET",
+"https://www.github.com") pool.request("GET", "https://www.github.com") # takes
+from the cache ``` ## How and where are the responses saved? The responses are
+stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/
+#storages). You have complete control over them; you can change storage or even
+write your own if necessary. ## Contributing `Hishel` is a powerful tool, but
+it is also a new project with potential flaws, so we welcome contributions! You
+can open the pull request by following these instructions if you want to
+improve `Hishel`. ð - Fork the project. - Make change. - Open the pull
+request.
```

### Comparing `hishel-0.0.3/hishel/_controller.py` & `hishel-0.0.4/hishel/_controller.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_files.py` & `hishel-0.0.4/hishel/_files.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_headers.py` & `hishel-0.0.4/hishel/_headers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_serializers.py` & `hishel-0.0.4/hishel/_serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import yaml
 from httpcore import Response
 
 HEADERS_ENCODING = "iso-8859-1"
 KNOWN_RESPONSE_EXTENSIONS = ("http_version", "reason_phrase")
 
-__all__ = ("PickleSerializer", "JSONSerializer", "YamlSerializer", "BaseSerializer")
+__all__ = ("PickleSerializer", "JSONSerializer", "YAMLSerializer", "BaseSerializer")
 
 
 class BaseSerializer:
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         raise NotImplementedError()
 
     def loads(self, data: tp.Union[str, bytes]) -> Response:
@@ -83,15 +83,15 @@
         )
 
     @property
     def is_binary(self) -> bool:
         return False
 
 
-class YamlSerializer(BaseSerializer):
+class YAMLSerializer(BaseSerializer):
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         response_dict = {
             "status": response.status,
             "headers": [
                 (key.decode(HEADERS_ENCODING), value.decode(HEADERS_ENCODING))
                 for key, value in response.headers
             ],
```

### Comparing `hishel-0.0.3/hishel/_synchronization.py` & `hishel-0.0.4/hishel/_synchronization.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_utils.py` & `hishel-0.0.4/hishel/_utils.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_async/_client.py` & `hishel-0.0.4/hishel/_async/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_async/_mock.py` & `hishel-0.0.4/hishel/_async/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_async/_pool.py` & `hishel-0.0.4/hishel/_async/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_async/_storages.py` & `hishel-0.0.4/hishel/_async/_storages.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 
 
 class AsyncFileStorage(AsyncBaseStorage):
     def __init__(
         self,
         serializer: tp.Optional[BaseSerializer] = None,
         base_path: tp.Optional[Path] = None,
-        max_cache_age: tp.Optional[int] = None,
+        ttl: tp.Optional[int] = None,
     ) -> None:
         super().__init__(serializer)
-        if base_path:  # pragma: no cover
-            self._base_path = base_path
-        else:
-            self._base_path = Path("./.cache/hishel")
+
+        self._base_path = (
+            Path(base_path) if base_path is not None else Path(".cache/hishel")
+        )
 
         if not self._base_path.is_dir():
             self._base_path.mkdir(parents=True)
 
         self._file_manager = AsyncFileManager(is_binary=self._serializer.is_binary)
-        self._max_cache_age = max_cache_age
+        self._ttl = ttl
         self._lock = AsyncLock()
 
     async def store(self, key: str, response: Response) -> None:
         response_path = self._base_path / key
 
         async with self._lock:
             await self._file_manager.write_to(
@@ -74,44 +74,42 @@
         await self._remove_expired_caches()
         return None
 
     async def aclose(self) -> None:
         return
 
     async def _remove_expired_caches(self) -> None:
-        if self._max_cache_age is None:
+        if self._ttl is None:
             return
 
         async with self._lock:
             for file in self._base_path.iterdir():
                 if file.is_file():
                     age = time.time() - file.stat().st_mtime
-                    if age > self._max_cache_age:
+                    if age > self._ttl:
                         file.unlink()
 
 
 class AsyncRedisStorage(AsyncBaseStorage):
     def __init__(
         self,
         serializer: tp.Optional[BaseSerializer] = None,
         client: tp.Optional[redis.Redis] = None,  # type: ignore
-        max_cache_age: tp.Optional[int] = None,
+        ttl: tp.Optional[int] = None,
     ) -> None:
         super().__init__(serializer)
 
         if client is None:
             self._client = redis.Redis()  # type: ignore
         else:  # pragma: no cover
             self._client = client
-        self._max_cache_age = max_cache_age
+        self._ttl = ttl
 
     async def store(self, key: str, response: Response) -> None:
-        await self._client.set(
-            key, self._serializer.dumps(response), ex=self._max_cache_age
-        )
+        await self._client.set(key, self._serializer.dumps(response), ex=self._ttl)
 
     async def retreive(self, key: str) -> tp.Optional[Response]:
         cached_response = await self._client.get(key)
         if cached_response is None:
             return None
 
         return self._serializer.loads(cached_response)
```

### Comparing `hishel-0.0.3/hishel/_async/_transports.py` & `hishel-0.0.4/hishel/_async/_transports.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_sync/_client.py` & `hishel-0.0.4/hishel/_sync/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_sync/_mock.py` & `hishel-0.0.4/hishel/_sync/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_sync/_pool.py` & `hishel-0.0.4/hishel/_sync/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/hishel/_sync/_storages.py` & `hishel-0.0.4/hishel/_sync/_storages.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 
 
 class FileStorage(BaseStorage):
     def __init__(
         self,
         serializer: tp.Optional[BaseSerializer] = None,
         base_path: tp.Optional[Path] = None,
-        max_cache_age: tp.Optional[int] = None,
+        ttl: tp.Optional[int] = None,
     ) -> None:
         super().__init__(serializer)
-        if base_path:  # pragma: no cover
-            self._base_path = base_path
-        else:
-            self._base_path = Path("./.cache/hishel")
+
+        self._base_path = (
+            Path(base_path) if base_path is not None else Path(".cache/hishel")
+        )
 
         if not self._base_path.is_dir():
             self._base_path.mkdir(parents=True)
 
         self._file_manager = FileManager(is_binary=self._serializer.is_binary)
-        self._max_cache_age = max_cache_age
+        self._ttl = ttl
         self._lock = Lock()
 
     def store(self, key: str, response: Response) -> None:
         response_path = self._base_path / key
 
         with self._lock:
             self._file_manager.write_to(
@@ -74,44 +74,42 @@
         self._remove_expired_caches()
         return None
 
     def close(self) -> None:
         return
 
     def _remove_expired_caches(self) -> None:
-        if self._max_cache_age is None:
+        if self._ttl is None:
             return
 
         with self._lock:
             for file in self._base_path.iterdir():
                 if file.is_file():
                     age = time.time() - file.stat().st_mtime
-                    if age > self._max_cache_age:
+                    if age > self._ttl:
                         file.unlink()
 
 
 class RedisStorage(BaseStorage):
     def __init__(
         self,
         serializer: tp.Optional[BaseSerializer] = None,
         client: tp.Optional[redis.Redis] = None,  # type: ignore
-        max_cache_age: tp.Optional[int] = None,
+        ttl: tp.Optional[int] = None,
     ) -> None:
         super().__init__(serializer)
 
         if client is None:
             self._client = redis.Redis()  # type: ignore
         else:  # pragma: no cover
             self._client = client
-        self._max_cache_age = max_cache_age
+        self._ttl = ttl
 
     def store(self, key: str, response: Response) -> None:
-        self._client.set(
-            key, self._serializer.dumps(response), ex=self._max_cache_age
-        )
+        self._client.set(key, self._serializer.dumps(response), ex=self._ttl)
 
     def retreive(self, key: str) -> tp.Optional[Response]:
         cached_response = self._client.get(key)
         if cached_response is None:
             return None
 
         return self._serializer.loads(cached_response)
```

### Comparing `hishel-0.0.3/hishel/_sync/_transports.py` & `hishel-0.0.4/hishel/_sync/_transports.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/LICENSE` & `hishel-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/pyproject.toml` & `hishel-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hishel-0.0.3/PKG-INFO` & `hishel-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hishel
-Version: 0.0.3
+Version: 0.0.4
 Summary: Persistant cache implementation for httpx and httpcore
 Project-URL: Homepage, https://github.com/karosis88/hishel
 Project-URL: Source, https://github.com/karosis88/hishel
 Author-email: Kar Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -38,28 +38,29 @@
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hishel.svg)](https://pypi.org/project/hishel)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hishel.svg)](https://pypi.org/project/hishel)
 ![PyPI - License](https://img.shields.io/pypi/l/hishel)
 ![Codecov](https://img.shields.io/codecov/c/github/karosis88/hishel)
 
-
 -----
 
 **Hishel (հիշել, remember)** is a library that implements HTTP Caching for [HTTPX](https://github.com/encode/httpx) and [HTTP Core](https://github.com/encode/httpcore) libraries in accordance with **RFC 9111**, the most recent caching specification.
 
 ## Features
 
 - 💾 Persistence: Responses are cached in the [**persistent memory**](https://en.m.wikipedia.org/wiki/Persistent_memory) for later use.
 - 🤲 Compatibility: It is completely compatible with your existing transports or connection pools, **whether they are default, custom, or provided by third-party libraries.**
 - 🤗 Easy to use: You continue to use the httpx and httpcore interfaces. **Can be integrated with no changes to the code.**
 - 🧠 Smart: Attempts to clearly implement RFC 9111, understands `Vary`, `Etag`, `Last-Modified`,  `Cache-Control`, and `Expires` headers, and **handles response re-validation automatically**.
-- ⚙️ Configurable: You can specify the **backend** where the responses should be stored, the **serializer**, and you can write your own **backends and serializers**. You can also specify which parts of RFC 9111 **should be ignored and which should not**, for example, you can explicitly disable stale responses for your safety or enable re-validation for each response before using it. 
-- 🚀 Very fast: When **IO is not required**, your requests are even faster.
+- ⚙️ Configurable: You have complete control over how the responses are stored and serialized, and there is built-in support for filesystem and redis backends.
+- 🚀 Very fast: Your requests will be even faster if there are **no IO operations**.
 
+## Documentation
+Go through the [Hishel documentation](https://karosis88.github.io/hishel/).
 
 ## QuickStart
 
 Install `Hishel` using pip:
 ``` shell
 $ pip install hishel
 ```
@@ -118,29 +119,34 @@
 pool.request("GET", "https://www.github.com")
 pool.request("GET", "https://www.github.com")  # takes from the cache
 
 ```
 
 ## How and where are the responses saved?
 
-The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a variety of built-in storage options, but the default storage is a [filesystem storage](TODO). You can switch the storage to another one that `Hishel` offers or, if necessary, write your own; for more information, see the storage documentation.
+The responses are stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/#storages).
+You have complete control over them; you can change storage or even write your own if necessary.
 
 
 ## Contributing
 
 `Hishel` is a powerful tool, but it is also a new project with potential flaws, so we welcome contributions!
 
 You can open the pull request by following these instructions if you want to improve `Hishel`. 💓
 
 - Fork the project.
 - Make change.
 - Open the pull request.
 
 # Changelog
 
+## 0.0.4 (7/29/2023)
+
+- Change `YamlSerializer` name to `YAMLSerializer`.
+
 ## 0.0.3 (7/28/2023)
 
 - Add `from_cache` response extension.
 - Add `typing_extensions` into the requirements.
 
 ## 0.0.2 (7/25/2023)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hishel Version: 0.0.3 Summary: Persistant cache
+Metadata-Version: 2.1 Name: hishel Version: 0.0.4 Summary: Persistant cache
 implementation for httpx and httpcore Project-URL: Homepage, https://
 github.com/karosis88/hishel Project-URL: Source, https://github.com/karosis88/
 hishel Author-email: Kar Petrosyan
 petrosyanpy@gmail.com> License-Expression: BSD-3-Clause License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Web
 Environment Classifier: Framework :: AsyncIO Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -29,44 +29,42 @@
 memory**](https://en.m.wikipedia.org/wiki/Persistent_memory) for later use. -
 ð¤² Compatibility: It is completely compatible with your existing transports
 or connection pools, **whether they are default, custom, or provided by third-
 party libraries.** - ð¤ Easy to use: You continue to use the httpx and
 httpcore interfaces. **Can be integrated with no changes to the code.** - ð§ 
 Smart: Attempts to clearly implement RFC 9111, understands `Vary`, `Etag`,
 `Last-Modified`, `Cache-Control`, and `Expires` headers, and **handles response
-re-validation automatically**. - âï¸ Configurable: You can specify the
-**backend** where the responses should be stored, the **serializer**, and you
-can write your own **backends and serializers**. You can also specify which
-parts of RFC 9111 **should be ignored and which should not**, for example, you
-can explicitly disable stale responses for your safety or enable re-validation
-for each response before using it. - ð Very fast: When **IO is not
-required**, your requests are even faster. ## QuickStart Install `Hishel` using
-pip: ``` shell $ pip install hishel ``` Let's begin with an example of a httpx
-client. ```python import hishel with hishel.CacheClient() as client: client.get
-("https://www.github.com") client.get("https://www.github.com") # takes from
-the cache (very fast!) ``` or in asynchronous context ```python import hishel
-async with hishel.AsyncCacheClient() as client: await client.get("https://
-www.github.com") await client.get("https://www.github.com") # takes from the
-cache ``` ## HTTPX and HTTP Core `Hishel` also supports the transports of
-`HTTPX` and the connection pools of `HTTP Core`. `Hishel` respects existing
-**transports** and **connection pools** and can therefore work **on top of
-them**, making hishel a very **compatible and flexible library**.
-**Transports** example: ``` python import httpx import hishel transport =
-httpx.HTTPTransport() cache_transport = hishel.CacheTransport
-(transport=transport) req = httpx.Request("GET", "https://www.github.com")
-cache_transport.handle_request(req) cache_transport.handle_request(req) # takes
-from the cache ``` **Connection Pool** example: ```python import httpcore
-import hishel pool = hishel.CacheConnectionPool(pool=httpcore.ConnectionPool())
-pool.request("GET", "https://www.github.com") pool.request("GET", "https://
-www.github.com") # takes from the cache ``` ## How and where are the responses
-saved? The responses are stored by `Hishel` in [storages](TODO). `Hishel` has a
-variety of built-in storage options, but the default storage is a [filesystem
-storage](TODO). You can switch the storage to another one that `Hishel` offers
-or, if necessary, write your own; for more information, see the storage
-documentation. ## Contributing `Hishel` is a powerful tool, but it is also a
-new project with potential flaws, so we welcome contributions! You can open the
-pull request by following these instructions if you want to improve `Hishel`.
-ð - Fork the project. - Make change. - Open the pull request. # Changelog ##
-0.0.3 (7/28/2023) - Add `from_cache` response extension. - Add
-`typing_extensions` into the requirements. ## 0.0.2 (7/25/2023) - Add [redis]
-(https://redis.io/) support. - Make backends thread and task safe. - Add black
-as a new linter. - Add an expire time for cached responses.
+re-validation automatically**. - âï¸ Configurable: You have complete control
+over how the responses are stored and serialized, and there is built-in support
+for filesystem and redis backends. - ð Very fast: Your requests will be even
+faster if there are **no IO operations**. ## Documentation Go through the
+[Hishel documentation](https://karosis88.github.io/hishel/). ## QuickStart
+Install `Hishel` using pip: ``` shell $ pip install hishel ``` Let's begin with
+an example of a httpx client. ```python import hishel with hishel.CacheClient()
+as client: client.get("https://www.github.com") client.get("https://
+www.github.com") # takes from the cache (very fast!) ``` or in asynchronous
+context ```python import hishel async with hishel.AsyncCacheClient() as client:
+await client.get("https://www.github.com") await client.get("https://
+www.github.com") # takes from the cache ``` ## HTTPX and HTTP Core `Hishel`
+also supports the transports of `HTTPX` and the connection pools of `HTTP
+Core`. `Hishel` respects existing **transports** and **connection pools** and
+can therefore work **on top of them**, making hishel a very **compatible and
+flexible library**. **Transports** example: ``` python import httpx import
+hishel transport = httpx.HTTPTransport() cache_transport =
+hishel.CacheTransport(transport=transport) req = httpx.Request("GET", "https://
+www.github.com") cache_transport.handle_request(req)
+cache_transport.handle_request(req) # takes from the cache ``` **Connection
+Pool** example: ```python import httpcore import hishel pool =
+hishel.CacheConnectionPool(pool=httpcore.ConnectionPool()) pool.request("GET",
+"https://www.github.com") pool.request("GET", "https://www.github.com") # takes
+from the cache ``` ## How and where are the responses saved? The responses are
+stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/
+#storages). You have complete control over them; you can change storage or even
+write your own if necessary. ## Contributing `Hishel` is a powerful tool, but
+it is also a new project with potential flaws, so we welcome contributions! You
+can open the pull request by following these instructions if you want to
+improve `Hishel`. ð - Fork the project. - Make change. - Open the pull
+request. # Changelog ## 0.0.4 (7/29/2023) - Change `YamlSerializer` name to
+`YAMLSerializer`. ## 0.0.3 (7/28/2023) - Add `from_cache` response extension. -
+Add `typing_extensions` into the requirements. ## 0.0.2 (7/25/2023) - Add
+[redis](https://redis.io/) support. - Make backends thread and task safe. - Add
+black as a new linter. - Add an expire time for cached responses.
```

