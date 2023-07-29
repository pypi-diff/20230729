# Comparing `tmp/aiogram3_di-1.0.0.tar.gz` & `tmp/aiogram3_di-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_di-1.0.0.tar", last modified: Fri Jul 28 20:04:23 2023, max compression
+gzip compressed data, was "aiogram3_di-1.0.1.tar", last modified: Sat Jul 29 08:00:42 2023, max compression
```

## Comparing `aiogram3_di-1.0.0.tar` & `aiogram3_di-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 20:04:23.220456 aiogram3_di-1.0.0/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.0/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1285 2023-07-28 20:04:23.220456 aiogram3_di-1.0.0/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      997 2023-07-28 19:57:37.000000 aiogram3_di-1.0.0/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 20:04:23.220456 aiogram3_di-1.0.0/aiogram3_di/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.0/aiogram3_di/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-28 19:36:21.000000 aiogram3_di-1.0.0/aiogram3_di/_version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      289 2023-07-28 19:58:50.000000 aiogram3_di-1.0.0/aiogram3_di/depends.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      529 2023-07-28 19:02:18.000000 aiogram3_di-1.0.0/aiogram3_di/middleware.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     3714 2023-07-28 19:09:47.000000 aiogram3_di-1.0.0/aiogram3_di/utils.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 20:04:23.220456 aiogram3_di-1.0.0/aiogram3_di.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1285 2023-07-28 20:04:23.000000 aiogram3_di-1.0.0/aiogram3_di.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-28 20:04:23.000000 aiogram3_di-1.0.0/aiogram3_di.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-28 20:04:23.000000 aiogram3_di-1.0.0/aiogram3_di.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-28 20:04:23.000000 aiogram3_di-1.0.0/aiogram3_di.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-28 20:04:23.000000 aiogram3_di-1.0.0/aiogram3_di.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-28 20:04:23.220456 aiogram3_di-1.0.0/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      725 2023-07-28 20:04:06.000000 aiogram3_di-1.0.0/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.1/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1285 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      997 2023-07-28 19:57:37.000000 aiogram3_di-1.0.1/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/aiogram3_di/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.1/aiogram3_di/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-29 07:54:36.000000 aiogram3_di-1.0.1/aiogram3_di/_version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      289 2023-07-28 19:58:50.000000 aiogram3_di-1.0.1/aiogram3_di/depends.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      628 2023-07-29 07:32:25.000000 aiogram3_di-1.0.1/aiogram3_di/middleware.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3615 2023-07-29 07:46:05.000000 aiogram3_di-1.0.1/aiogram3_di/utils.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/aiogram3_di.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1285 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-29 08:00:42.000000 aiogram3_di-1.0.1/aiogram3_di.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-29 08:00:42.953884 aiogram3_di-1.0.1/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      725 2023-07-28 20:04:06.000000 aiogram3_di-1.0.1/setup.py
```

### Comparing `aiogram3_di-1.0.0/LICENSE` & `aiogram3_di-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.0/PKG-INFO` & `aiogram3_di-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3_di
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogram3_di-1.0.0/README.md` & `aiogram3_di-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.0/aiogram3_di/middleware.py` & `aiogram3_di-1.0.1/aiogram3_di/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import Callable, Awaitable
+from contextlib import AsyncExitStack
 from typing import Any
 
 from aiogram import BaseMiddleware
 from aiogram.types import TelegramObject
 
 from .utils import process_dependencies
 
@@ -10,9 +11,10 @@
 class DIMiddleware(BaseMiddleware):
     async def __call__(
             self,
             handler: Callable[[TelegramObject, dict[str, Any]], Awaitable[Any]],
             event: TelegramObject,
             data: dict[str, Any]
     ) -> Any:
-        data = await process_dependencies(data.copy())
-        return await handler(event, data)
+        async with AsyncExitStack() as stack:
+            data = await process_dependencies(stack, data.copy())
+            return await handler(event, data)
```

### Comparing `aiogram3_di-1.0.0/aiogram3_di/utils.py` & `aiogram3_di-1.0.1/aiogram3_di/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,38 +34,49 @@
         ok = bool(await asyncio.to_thread(cm.__exit__, type(e), e, None))
         if not ok:
             raise e
     else:
         await asyncio.to_thread(cm.__exit__, None, None, None)
 
 
-async def process_dependencies(data: dict[str, Any]) -> dict[str, Any]:
+def _extract_params(annotations: dict[str, Any], param_data: dict[tuple[int, str], Any]) -> dict[str, Any]:
+    dependencies: list[tuple[int, str]] = [(hash(value.__metadata__[0].func or value.__origin__), key) for key, value in annotations.items()
+                                            if isinstance(value, _AnnotatedAlias) and isinstance(value.__metadata__[0], Depends)]
+    return {param_name: param_data[(func_hash, param_name)] for func_hash, param_name in dependencies}
+
+
+async def _process_dependency(
+        cache: dict[int, Any],
+        call: Callable[..., Any],
+        use_cache: bool,
+        stack: AsyncExitStack,
+        data: dict[str, Any],
+        param_data: dict[tuple[int, str], Any]
+) -> Any:
+    if (cached_value := cache.get(hash(call))) and use_cache:
+        return cached_value
+
+    values = _get_valid_kwargs((data | _extract_params(inspect.getfullargspec(call).annotations, param_data)), call)
+
+    if inspect.isasyncgenfunction(call):
+        cm = asynccontextmanager(call)(**values)
+        return await stack.enter_async_context(cm)
+    elif inspect.isgeneratorfunction(call):
+        cm = _contextmanager_in_threadpool(contextmanager(call)(**values))
+        return await stack.enter_async_context(cm)
+    elif asyncio.iscoroutinefunction(call):
+        return await call(**values)
+    else:
+        return await asyncio.to_thread(call, **values)
+
+
+async def process_dependencies(stack: AsyncExitStack, data: dict[str, Any]) -> dict[str, Any]:
     param_data: dict[tuple[int, str], Any] = {}
     cache: dict[int, Any] = {}
 
-    async with AsyncExitStack() as stack:
-        for param_name, dependency, type_annotation in _get_dependencies(data['handler'].spec.annotations):
-            call = dependency.func or type_annotation
-
-            if (cached_value := cache.get(hash(call))) and dependency.use_cache:
-                result = cached_value
-            else:
-                func_dependencies: list[tuple[int, str]] = [(hash(value.__metadata__[0].func or value.__origin__), key) for key, value in inspect.getfullargspec(call).annotations.items()
-                                                             if isinstance(value, _AnnotatedAlias) and isinstance(value.__metadata__[0], Depends)]
-                values = _get_valid_kwargs(data | {param_name: param_data[(func_hash, param_name)] for func_hash, param_name in func_dependencies}, call)
-
-                if inspect.isasyncgenfunction(call):
-                    cm = asynccontextmanager(call)(**values)
-                    result = await stack.enter_async_context(cm)
-                elif inspect.isgeneratorfunction(call):
-                    cm = _contextmanager_in_threadpool(contextmanager(call)(**values))
-                    result = await stack.enter_async_context(cm)
-                elif asyncio.iscoroutinefunction(call):
-                    result = await call(**values)
-                else:
-                    result = await asyncio.to_thread(call, **values)
-
-            param_data[(hash(call)), param_name] = result
-            cache.setdefault(hash(call), result)
-    handler_dependencies: list[tuple[int, str]] = [(hash(value.__metadata__[0].func or value.__origin__), key) for key, value in data['handler'].spec.annotations.items()
-                                                    if isinstance(value, _AnnotatedAlias) and isinstance(value.__metadata__[0], Depends)]
-    return data | {param_name: param_data[(func_hash, param_name)] for func_hash, param_name in handler_dependencies}
+    for param_name, dependency, type_annotation in _get_dependencies(data['handler'].spec.annotations):
+        call = dependency.func or type_annotation
+        result = await _process_dependency(cache, call, dependency.use_cache, stack, data, param_data)
+        param_data[(hash(call)), param_name] = result
+        cache.setdefault(hash(call), result)
+
+    return data | _extract_params(data['handler'].spec.annotations, param_data)
```

### Comparing `aiogram3_di-1.0.0/aiogram3_di.egg-info/PKG-INFO` & `aiogram3_di-1.0.1/aiogram3_di.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-di
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogram3_di-1.0.0/setup.py` & `aiogram3_di-1.0.1/setup.py`

 * *Files identical despite different names*

