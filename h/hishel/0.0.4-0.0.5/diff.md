# Comparing `tmp/hishel-0.0.4.tar.gz` & `tmp/hishel-0.0.5.tar.gz`

## Comparing `hishel-0.0.4.tar` & `hishel-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hishel-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 hishel-0.0.4/README.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/__about__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/__init__.py
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_controller.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_exceptions.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_files.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_serializers.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_synchronization.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/py.typed
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_client.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_mock.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_pool.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_storages.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_async/_transports.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_client.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_mock.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_pool.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_storages.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 hishel-0.0.4/hishel/_sync/_transports.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.4/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.4/LICENSE
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 hishel-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hishel-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 hishel-0.0.5/README.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/__about__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/__init__.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_controller.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_exceptions.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_files.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_serializers.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_synchronization.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/py.typed
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_client.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_mock.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_pool.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_storages.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_transports.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_client.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_mock.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_pool.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_storages.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_transports.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 hishel-0.0.5/PKG-INFO
```

### Comparing `hishel-0.0.4/README.md` & `hishel-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_controller.py` & `hishel-0.0.5/hishel/_controller.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_files.py` & `hishel-0.0.5/hishel/_files.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_headers.py` & `hishel-0.0.5/hishel/_headers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_serializers.py` & `hishel-0.0.5/hishel/_serializers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_synchronization.py` & `hishel-0.0.5/hishel/_synchronization.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_utils.py` & `hishel-0.0.5/hishel/_utils.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_async/_client.py` & `hishel-0.0.5/hishel/_async/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_async/_mock.py` & `hishel-0.0.5/hishel/_async/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_async/_pool.py` & `hishel-0.0.5/hishel/_async/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_async/_storages.py` & `hishel-0.0.5/hishel/_async/_storages.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_async/_transports.py` & `hishel-0.0.5/hishel/_async/_transports.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 if tp.TYPE_CHECKING:  # pragma: no cover
     from typing_extensions import Self
 
 __all__ = ("AsyncCacheTransport",)
 
 
+async def fake_stream(content: bytes) -> tp.AsyncIterable[bytes]:
+    yield content
+
+
 class AsyncCacheTransport(httpx.AsyncBaseTransport):
     def __init__(
         self,
         transport: httpx.AsyncBaseTransport,
         storage: tp.Optional[AsyncBaseStorage] = None,
         controller: tp.Optional[Controller] = None,
     ) -> None:
@@ -42,15 +46,14 @@
                 port=request.url.port,
                 target=request.url.raw_path,
             ),
             headers=request.headers.raw,
             content=request.stream,
             extensions=request.extensions,
         )
-
         key = generate_key(httpcore_request)
         stored_resposne = await self._storage.retreive(key)
 
         if stored_resposne:
             # Try using the stored response if it was discovered.
 
             res = self._controller.construct_response_from_cache(
@@ -99,35 +102,40 @@
                 assert isinstance(full_response.stream, tp.AsyncIterable)
                 full_response.extensions["from_cache"] = (  # type: ignore[index]
                     httpcore_response.status == 304
                 )
                 return Response(
                     status_code=full_response.status,
                     headers=full_response.headers,
-                    stream=AsyncResponseStream(full_response.stream),
+                    stream=AsyncResponseStream(fake_stream(full_response.content)),
                     extensions=full_response.extensions,
                 )
 
         response = await self._transport.handle_async_request(request)
         assert isinstance(response.stream, tp.AsyncIterable)
         httpcore_response = httpcore.Response(
             status=response.status_code,
             headers=response.headers.raw,
             content=AsyncResponseStream(response.stream),
             extensions=response.extensions,
         )
+        await httpcore_response.aread()
 
         if self._controller.is_cachable(
             request=httpcore_request, response=httpcore_response
         ):
-            await httpcore_response.aread()
             await self._storage.store(key, httpcore_response)
 
         response.extensions["from_cache"] = False  # type: ignore[index]
-        return response
+        return Response(
+            status_code=httpcore_response.status,
+            headers=httpcore_response.headers,
+            stream=AsyncResponseStream(fake_stream(httpcore_response.content)),
+            extensions=httpcore_response.extensions,
+        )
 
     async def aclose(self) -> None:
         await self._storage.aclose()
 
     async def __aenter__(self) -> "Self":
         return self
```

### Comparing `hishel-0.0.4/hishel/_sync/_client.py` & `hishel-0.0.5/hishel/_sync/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_sync/_mock.py` & `hishel-0.0.5/hishel/_sync/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_sync/_pool.py` & `hishel-0.0.5/hishel/_sync/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_sync/_storages.py` & `hishel-0.0.5/hishel/_sync/_storages.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/hishel/_sync/_transports.py` & `hishel-0.0.5/hishel/_sync/_transports.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 if tp.TYPE_CHECKING:  # pragma: no cover
     from typing_extensions import Self
 
 __all__ = ("CacheTransport",)
 
 
+def fake_stream(content: bytes) -> tp.Iterable[bytes]:
+    yield content
+
+
 class CacheTransport(httpx.BaseTransport):
     def __init__(
         self,
         transport: httpx.BaseTransport,
         storage: tp.Optional[BaseStorage] = None,
         controller: tp.Optional[Controller] = None,
     ) -> None:
@@ -42,15 +46,14 @@
                 port=request.url.port,
                 target=request.url.raw_path,
             ),
             headers=request.headers.raw,
             content=request.stream,
             extensions=request.extensions,
         )
-
         key = generate_key(httpcore_request)
         stored_resposne = self._storage.retreive(key)
 
         if stored_resposne:
             # Try using the stored response if it was discovered.
 
             res = self._controller.construct_response_from_cache(
@@ -99,35 +102,40 @@
                 assert isinstance(full_response.stream, tp.Iterable)
                 full_response.extensions["from_cache"] = (  # type: ignore[index]
                     httpcore_response.status == 304
                 )
                 return Response(
                     status_code=full_response.status,
                     headers=full_response.headers,
-                    stream=ResponseStream(full_response.stream),
+                    stream=ResponseStream(fake_stream(full_response.content)),
                     extensions=full_response.extensions,
                 )
 
         response = self._transport.handle_request(request)
         assert isinstance(response.stream, tp.Iterable)
         httpcore_response = httpcore.Response(
             status=response.status_code,
             headers=response.headers.raw,
             content=ResponseStream(response.stream),
             extensions=response.extensions,
         )
+        httpcore_response.read()
 
         if self._controller.is_cachable(
             request=httpcore_request, response=httpcore_response
         ):
-            httpcore_response.read()
             self._storage.store(key, httpcore_response)
 
         response.extensions["from_cache"] = False  # type: ignore[index]
-        return response
+        return Response(
+            status_code=httpcore_response.status,
+            headers=httpcore_response.headers,
+            stream=ResponseStream(fake_stream(httpcore_response.content)),
+            extensions=httpcore_response.extensions,
+        )
 
     def close(self) -> None:
         self._storage.close()
 
     def __enter__(self) -> "Self":
         return self
```

### Comparing `hishel-0.0.4/LICENSE` & `hishel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/pyproject.toml` & `hishel-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hishel-0.0.4/PKG-INFO` & `hishel-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hishel
-Version: 0.0.4
+Version: 0.0.5
 Summary: Persistant cache implementation for httpx and httpcore
 Project-URL: Homepage, https://github.com/karosis88/hishel
 Project-URL: Source, https://github.com/karosis88/hishel
 Author-email: Kar Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -135,14 +135,18 @@
 
 - Fork the project.
 - Make change.
 - Open the pull request.
 
 # Changelog
 
+## 0.0.5 (7/29/2023)
+
+- Fix httpx response streaming.
+
 ## 0.0.4 (7/29/2023)
 
 - Change `YamlSerializer` name to `YAMLSerializer`.
 
 ## 0.0.3 (7/28/2023)
 
 - Add `from_cache` response extension.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hishel Version: 0.0.4 Summary: Persistant cache
+Metadata-Version: 2.1 Name: hishel Version: 0.0.5 Summary: Persistant cache
 implementation for httpx and httpcore Project-URL: Homepage, https://
 github.com/karosis88/hishel Project-URL: Source, https://github.com/karosis88/
 hishel Author-email: Kar Petrosyan
 petrosyanpy@gmail.com> License-Expression: BSD-3-Clause License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Web
 Environment Classifier: Framework :: AsyncIO Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -59,12 +59,13 @@
 from the cache ``` ## How and where are the responses saved? The responses are
 stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/
 #storages). You have complete control over them; you can change storage or even
 write your own if necessary. ## Contributing `Hishel` is a powerful tool, but
 it is also a new project with potential flaws, so we welcome contributions! You
 can open the pull request by following these instructions if you want to
 improve `Hishel`. ð - Fork the project. - Make change. - Open the pull
-request. # Changelog ## 0.0.4 (7/29/2023) - Change `YamlSerializer` name to
-`YAMLSerializer`. ## 0.0.3 (7/28/2023) - Add `from_cache` response extension. -
-Add `typing_extensions` into the requirements. ## 0.0.2 (7/25/2023) - Add
-[redis](https://redis.io/) support. - Make backends thread and task safe. - Add
-black as a new linter. - Add an expire time for cached responses.
+request. # Changelog ## 0.0.5 (7/29/2023) - Fix httpx response streaming. ##
+0.0.4 (7/29/2023) - Change `YamlSerializer` name to `YAMLSerializer`. ## 0.0.3
+(7/28/2023) - Add `from_cache` response extension. - Add `typing_extensions`
+into the requirements. ## 0.0.2 (7/25/2023) - Add [redis](https://redis.io/
+) support. - Make backends thread and task safe. - Add black as a new linter. -
+Add an expire time for cached responses.
```

