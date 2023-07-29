# Comparing `tmp/async_wrapper-0.1.5.tar.gz` & `tmp/async_wrapper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.1.5.tar", max compression
+gzip compressed data, was "async_wrapper-0.1.6.tar", max compression
```

## Comparing `async_wrapper-0.1.5.tar` & `async_wrapper-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-07-29 15:07:09.471177 async_wrapper-0.1.5/LICENSE
--rw-r--r--   0        0        0     1892 2023-07-29 15:07:09.471177 async_wrapper-0.1.5/README.md
--rw-r--r--   0        0        0     3682 2023-07-29 15:07:28.700613 async_wrapper-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      419 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-07-29 15:07:28.748615 async_wrapper-0.1.5/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0      896 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      706 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1217 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1581 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      209 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     4414 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     3258 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/_asyncio.py
--rw-r--r--   0        0        0     5558 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     2735 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 async_wrapper-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1892 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/README.md
+-rw-r--r--   0        0        0     3682 2023-07-29 15:55:30.585636 async_wrapper-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      419 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-29 15:55:30.617636 async_wrapper-0.1.6/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0      896 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      706 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1217 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1581 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      209 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     4745 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/_anyio.py
+-rw-r--r--   0        0        0     3258 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/_asyncio.py
+-rw-r--r--   0        0        0     5558 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/base.py
+-rw-r--r--   0        0        0     2735 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/main.py
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 async_wrapper-0.1.6/PKG-INFO
```

### Comparing `async_wrapper-0.1.5/LICENSE` & `async_wrapper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/README.md` & `async_wrapper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/pyproject.toml` & `async_wrapper-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.1.5"
+version = "0.1.6"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
```

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/main.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.1.6/src/async_wrapper/task_group/_anyio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
-from asyncio import create_task, wait
-from functools import partial, wraps
+from asyncio import create_task, ensure_future, wait
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Generic,
     TypeVar,
     final,
 )
-from weakref import WeakSet
+from weakref import WeakSet, WeakValueDictionary
 
 from typing_extensions import ParamSpec, Self, override
 
 from async_wrapper.task_group.base import (
     BaseSoonWrapper,
     BaseTaskGroup,
     Semaphore,
@@ -25,15 +24,15 @@
 
 try:
     from anyio.abc import TaskGroup as _TaskGroup  # type: ignore
 except ImportError:
     from typing import Any as _TaskGroup
 
 if TYPE_CHECKING:
-    from asyncio import Task
+    from asyncio import Future, Task
     from types import TracebackType
 
     from anyio.abc import Semaphore as AnyioSemaphore  # type: ignore
 
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
@@ -43,52 +42,62 @@
 
 __all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
 
 
 class TaskGroup(BaseTaskGroup):
     def __init__(self) -> None:
         self._task_group: _TaskGroup = _get_task_group()
-        self._tasks: WeakSet[Task[Any]] = WeakSet()
+        self._futures: WeakSet[Future[Any]] = WeakSet()
+        self._task_futures: WeakValueDictionary[
+            Task[Any],
+            Future[Any],
+        ] = WeakValueDictionary()
 
     @override
     def start_soon(
         self,
         func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
         value = SoonValue()
-        wrapped = self._wrap_as_value(func, value)
-        self._task_group.start_soon(partial(wrapped, **kwargs), *args)
+        future = self._as_future(func, *args, **kwargs)
+        value._set_task_or_future(future)  # noqa: SLF001
+        self._task_group.start_soon(self._as_task, future)
         return value
 
-    def _wrap_as_value(
+    def _as_future(
         self,
         func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
-        value: SoonValue[ValueT_co],
-    ) -> Callable[ParamT, Coroutine[None, None, None]]:
-        @wraps(func)
-        async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> None:
-            coro = func(*args, **kwargs)
-            task = create_task(coro)
-            value._set_task_or_future(task)  # noqa: SLF001
-            self.tasks.add(task)
-            await task
-
-        return inner
+        *args: ParamT.args,
+        **kwargs: ParamT.kwargs,
+    ) -> Future[ValueT_co]:
+        coro = func(*args, **kwargs)
+        future = ensure_future(coro)
+        self._futures.add(future)
+        return future
+
+    async def _as_coro(self, future: Future[ValueT_co]) -> ValueT_co:
+        return await future
+
+    async def _as_task(self, future: Future[ValueT_co]) -> ValueT_co:
+        coro = self._as_coro(future)
+        task = create_task(coro)
+        self._task_futures[task] = future
+        return await task
 
     @property
     @override
     def is_active(self) -> bool:
         return self._task_group._active  # type: ignore # noqa: SLF001
 
     @property
     @override
     def tasks(self) -> WeakSet[Task[Any]]:
-        return self._tasks
+        return WeakSet(self._task_futures.keys())
 
     @override
     async def __aenter__(self) -> Self:
         await self._task_group.__aenter__()
         return self
 
     @override
```

### Comparing `async_wrapper-0.1.5/src/async_wrapper/task_group/_asyncio.py` & `async_wrapper-0.1.6/src/async_wrapper/task_group/_asyncio.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/task_group/base.py` & `async_wrapper-0.1.6/src/async_wrapper/task_group/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/src/async_wrapper/task_group/main.py` & `async_wrapper-0.1.6/src/async_wrapper/task_group/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.5/PKG-INFO` & `async_wrapper-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.1.5
+Version: 0.1.6
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

