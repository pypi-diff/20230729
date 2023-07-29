# Comparing `tmp/async_wrapper-0.1.6.tar.gz` & `tmp/async_wrapper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.1.6.tar", max compression
+gzip compressed data, was "async_wrapper-0.2.1.tar", max compression
```

## Comparing `async_wrapper-0.1.6.tar` & `async_wrapper-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/LICENSE
--rw-r--r--   0        0        0     1892 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/README.md
--rw-r--r--   0        0        0     3682 2023-07-29 15:55:30.585636 async_wrapper-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      419 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-07-29 15:55:30.617636 async_wrapper-0.1.6/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0      896 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      706 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1217 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1581 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      209 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     4745 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     3258 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/_asyncio.py
--rw-r--r--   0        0        0     5558 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     2735 2023-07-29 15:55:18.137599 async_wrapper-0.1.6/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 async_wrapper-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-29 20:35:14.034783 async_wrapper-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1850 2023-07-29 20:35:14.034783 async_wrapper-0.2.1/README.md
+-rw-r--r--   0        0        0     3649 2023-07-29 20:35:27.010767 async_wrapper-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      419 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-29 20:35:27.042766 async_wrapper-0.2.1/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0     1007 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      564 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1140 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1136 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      209 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     8669 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/_anyio.py
+-rw-r--r--   0        0        0     3227 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/_asyncio.py
+-rw-r--r--   0        0        0     6194 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/base.py
+-rw-r--r--   0        0        0     2733 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/main.py
+-rw-r--r--   0        0        0     2936 1970-01-01 00:00:00.000000 async_wrapper-0.2.1/PKG-INFO
```

### Comparing `async_wrapper-0.1.6/LICENSE` & `async_wrapper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.6/README.md` & `async_wrapper-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 ## how to install
 ```shell
 $ pip install async_wrapper
 # or
 $ pip install "async_wrapper[all]"
 # or
-$ pip install "async_wrapper[anyio]"
-# or
 $ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
 from __future__ import annotations
```

### Comparing `async_wrapper-0.1.6/pyproject.toml` & `async_wrapper-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.1.6"
+version = "0.2.1"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = "^4.6.3"
-anyio = { version = "^3.7.0", optional = true }
+anyio = "^3.7.0"
 aiotools = { version = "^1.6.1", python = "<3.11" }
 loky = { version = "^3.4.0", optional = true }
 cloudpickle = { version = "^2.2.1", optional = true }
 psutil = { version = "^5.9.5", optional = true }
-pyyaml = ">=6.0.1" # cython error
+pyyaml = ">=6.0.1"                                    # cython error
 
 [tool.poetry.extras]
-all = ['anyio', 'loky', "cloudpickle", "psutil"]
-anyio = ['anyio']
+all = ['loky', "cloudpickle", "psutil"]
 loky = ['loky', "cloudpickle", "psutil"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.0.275"
 black = "23.3.0"
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
-pytest-asyncio = "^0.21.0"
 pre-commit = "^3.3.3"
+trio = "^0.22.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py38"
```

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-import asyncio
-from functools import wraps
+from functools import partial, wraps
 from typing import Any, Callable, Coroutine, TypeVar
 
+import anyio
 from typing_extensions import ParamSpec
 
 ValueT = TypeVar("ValueT")
 ParamT = ParamSpec("ParamT")
 
 __all__ = ["sync_to_async"]
 
@@ -18,15 +18,17 @@
     try:
         from loky.process_executor import (  # type: ignore
             ProcessPoolExecutor,  # type: ignore
         )
     except ImportError as exc:
         raise ImportError("install extas loky first") from exc
 
-    @wraps(func)
-    async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
+    def new(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
         with ProcessPoolExecutor(1) as pool:
             future = pool.submit(func, *args, **kwargs)  # type: ignore
-            coro = asyncio.wrap_future(future)
-            return await coro
+            return future.result()
+
+    @wraps(func)
+    async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
+        return await anyio.to_thread.run_sync(partial(new, *args, **kwargs))
 
     return inner
```

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from __future__ import annotations
 
-import asyncio
-from concurrent.futures import ThreadPoolExecutor
-from functools import wraps
+from functools import partial, wraps
 from typing import Any, Callable, Coroutine, TypeVar
 
+import anyio
 from typing_extensions import ParamSpec
 
 ValueT = TypeVar("ValueT")
 ParamT = ParamSpec("ParamT")
 
 __all__ = ["sync_to_async"]
 
 
 def sync_to_async(
     func: Callable[ParamT, ValueT],
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     @wraps(func)
     async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
-        with ThreadPoolExecutor(1) as pool:
-            future = pool.submit(func, *args, **kwargs)
-            coro = asyncio.wrap_future(future)
-            return await coro
+        return await anyio.to_thread.run_sync(partial(func, *args, **kwargs))
 
     return inner
```

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/main.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
-import asyncio
 from concurrent.futures import ThreadPoolExecutor, wait
-from functools import wraps
+from functools import partial, wraps
 from typing import Awaitable, Callable, TypeVar
 
+import anyio
 from typing_extensions import ParamSpec
 
-from async_wrapper.convert.synclib.base import as_coro_func
-
 ValueT = TypeVar("ValueT")
 ParamT = ParamSpec("ParamT")
 
 __all__ = ["async_to_sync"]
 
 
 def async_to_sync(
@@ -41,9 +39,8 @@
 
 
 def _run(
     func: Callable[ParamT, Awaitable[ValueT]],
     *args: ParamT.args,
     **kwargs: ParamT.kwargs,
 ) -> ValueT:
-    func = as_coro_func(func)
-    return asyncio.run(func(*args, **kwargs))
+    return anyio.run(partial(func, *args, **kwargs))
```

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,29 @@
 from __future__ import annotations
 
-import asyncio
-from functools import wraps
-from typing import Any, Awaitable, Callable, Coroutine, Protocol, TypeVar
+from functools import partial, wraps
+from typing import Awaitable, Callable, Protocol, TypeVar
 
+import anyio
 from typing_extensions import ParamSpec
 
 ValueT = TypeVar("ValueT")
 ParamT = ParamSpec("ParamT")
 
-__all__ = ["as_coro_func", "as_sync_func", "AsyncToSync"]
+__all__ = ["as_sync_func", "AsyncToSync"]
 
 
 class AsyncToSync(Protocol):
     def __call__(  # noqa: D102
         self,
         func: Callable[ParamT, Awaitable[ValueT]],
     ) -> Callable[ParamT, ValueT]:
         ...
 
 
-def as_coro_func(
-    func: Callable[ParamT, Awaitable[ValueT]],
-) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
-    """awaitable func to corotine func
-
-    Args:
-        func: awaitable func
-
-    Returns:
-        corotine func
-    """
-
-    @wraps(func)
-    async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
-        return await func(*args, **kwargs)
-
-    return inner
-
-
 def as_sync_func(
     func: Callable[ParamT, Awaitable[ValueT]],
 ) -> Callable[ParamT, ValueT]:
     """awaitable func to sync func
 
     Args:
         func: awaitable func
@@ -67,9 +48,8 @@
 
     Args:
         func: awaitable func
 
     Returns:
         func result
     """
-    func = as_coro_func(func)
-    return asyncio.run(func(*args, **kwargs))
+    return anyio.run(partial(func, *args, **kwargs))
```

### Comparing `async_wrapper-0.1.6/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.6/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.2.1/src/async_wrapper/task_group/_asyncio.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,75 @@
 from __future__ import annotations
 
-from asyncio import create_task, ensure_future, wait
+import sys
+from asyncio import Semaphore as AsyncioSemaphore
+from asyncio import wait
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
-from weakref import WeakSet, WeakValueDictionary
 
 from typing_extensions import ParamSpec, Self, override
 
 from async_wrapper.task_group.base import (
     BaseSoonWrapper,
     BaseTaskGroup,
     Semaphore,
     SoonValue,
 )
 
-try:
-    from anyio.abc import TaskGroup as _TaskGroup  # type: ignore
-except ImportError:
-    from typing import Any as _TaskGroup
+if sys.version_info < (3, 11):
+    from aiotools.taskgroup import TaskGroup as _TaskGroup  # type: ignore
+else:
+    from asyncio.taskgroups import TaskGroup as _TaskGroup  # type: ignore
 
 if TYPE_CHECKING:
-    from asyncio import Future, Task
+    from asyncio import Task
     from types import TracebackType
-
-    from anyio.abc import Semaphore as AnyioSemaphore  # type: ignore
-
+    from weakref import WeakSet
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 __all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
 
 
 class TaskGroup(BaseTaskGroup):
     def __init__(self) -> None:
-        self._task_group: _TaskGroup = _get_task_group()
-        self._futures: WeakSet[Future[Any]] = WeakSet()
-        self._task_futures: WeakValueDictionary[
-            Task[Any],
-            Future[Any],
-        ] = WeakValueDictionary()
+        self._task_group = _TaskGroup()
 
     @override
     def start_soon(
         self,
         func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
-        value = SoonValue()
-        future = self._as_future(func, *args, **kwargs)
-        value._set_task_or_future(future)  # noqa: SLF001
-        self._task_group.start_soon(self._as_task, future)
-        return value
-
-    def _as_future(
-        self,
-        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
-        *args: ParamT.args,
-        **kwargs: ParamT.kwargs,
-    ) -> Future[ValueT_co]:
         coro = func(*args, **kwargs)
-        future = ensure_future(coro)
-        self._futures.add(future)
-        return future
-
-    async def _as_coro(self, future: Future[ValueT_co]) -> ValueT_co:
-        return await future
-
-    async def _as_task(self, future: Future[ValueT_co]) -> ValueT_co:
-        coro = self._as_coro(future)
-        task = create_task(coro)
-        self._task_futures[task] = future
-        return await task
+        task = self._task_group.create_task(coro)
+        return SoonValue(task_or_future=task)
 
     @property
     @override
     def is_active(self) -> bool:
-        return self._task_group._active  # type: ignore # noqa: SLF001
+        return self._task_group._entered  # noqa: SLF001
 
     @property
     @override
     def tasks(self) -> WeakSet[Task[Any]]:
-        return WeakSet(self._task_futures.keys())
+        return self._task_group._tasks  # noqa: SLF001
 
     @override
     async def __aenter__(self) -> Self:
         await self._task_group.__aenter__()
         return self
 
     @override
@@ -114,27 +86,24 @@
 
 
 @final
 class SoonWrapper(
     BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
     Generic[ParamT, ValueT_co],
 ):
-    @override
-    def __new__(
-        cls,
-        func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
-        task_group: TaskGroup,
-        semaphore: Semaphore | None = None,
-    ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
-        try:
-            import anyio  # type: ignore # noqa: F401
-        except ImportError as exc:
-            raise ImportError("install extas anyio first") from exc
+    if TYPE_CHECKING:
 
-        return super().__new__(cls, func, task_group, semaphore)  # type: ignore
+        @override
+        def __new__(
+            cls,
+            func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
+            task_group: TaskGroup,
+            semaphore: Semaphore | None = None,
+        ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
+            ...
 
     @override
     def __call__(
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
@@ -144,25 +113,13 @@
     @override
     def copy(self, semaphore: Semaphore | None = None) -> Self:
         if semaphore is None:
             semaphore = self.semaphore
         return SoonWrapper(self.func, self.task_group, semaphore)
 
 
-def get_semaphore_class() -> type[AnyioSemaphore]:
-    try:
-        from anyio import Semaphore as _Semaphore  # type: ignore
-    except ImportError as exc:
-        raise ImportError("install extas anyio first") from exc
-    return _Semaphore
-
-
-def _get_task_group() -> _TaskGroup:
-    try:
-        from anyio import create_task_group  # type: ignore
-    except ImportError as exc:
-        raise ImportError("install extas anyio first") from exc
-    return create_task_group()
+def get_semaphore_class() -> type[AsyncioSemaphore]:
+    return AsyncioSemaphore
 
 
 wrap_soon = SoonWrapper
 get_task_group = TaskGroup
```

### Comparing `async_wrapper-0.1.6/src/async_wrapper/task_group/base.py` & `async_wrapper-0.2.1/src/async_wrapper/task_group/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from asyncio import run_coroutine_threadsafe
 from contextlib import AbstractAsyncContextManager, suppress
 from functools import wraps
 from threading import local
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Coroutine,
+    Generator,
     Generic,
     Protocol,
     TypeVar,
 )
 
+import anyio
 from typing_extensions import ParamSpec, Self, override
 
 if TYPE_CHECKING:
-    from asyncio import Future, Task
+    from contextvars import Context
     from types import TracebackType
     from weakref import WeakSet
 
 TaskGroupT = TypeVar("TaskGroupT", bound="BaseTaskGroup")
 TaskGroupT_co = TypeVar("TaskGroupT_co", covariant=True, bound="BaseTaskGroup")
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
@@ -40,14 +41,33 @@
 
 
 class Semaphore(AbstractAsyncContextManager, Protocol):
     async def acquire(self) -> Any:
         ...
 
 
+class Futurelike(Protocol, Generic[ValueT_co]):
+    def __await__(self) -> Generator[Any, None, ValueT_co]:
+        ...
+
+    def exception(self) -> BaseException | None:
+        ...
+
+    def result(self) -> ValueT_co:
+        ...
+
+    def add_done_callback(
+        self,
+        __fn: Callable[[Self], Any],
+        *,
+        context: Context | None = None,
+    ) -> None:
+        ...
+
+
 class BaseTaskGroup(ABC):
     @abstractmethod
     def start_soon(
         self,
         func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
@@ -57,15 +77,15 @@
     @property
     @abstractmethod
     def is_active(self) -> bool:
         ...
 
     @property
     @abstractmethod
-    def tasks(self) -> WeakSet[Task[Any]]:
+    def tasks(self) -> WeakSet[Futurelike[Any]]:
         ...
 
     @abstractmethod
     async def __aenter__(self) -> Self:
         ...
 
     @abstractmethod
@@ -124,15 +144,15 @@
     def copy(self, semaphore: Semaphore | None = None) -> Self:  # noqa: D102
         ...
 
 
 class SoonValue(Generic[ValueT_co]):
     def __init__(
         self,
-        task_or_future: Task[ValueT_co] | Future[ValueT_co] | None = None,
+        task_or_future: Futurelike[ValueT_co] | None = None,
     ) -> None:
         self._value = Pending
         if task_or_future is None:
             self._task_or_future = None
         else:
             self._set_task_or_future(task_or_future)
 
@@ -168,39 +188,47 @@
 
         task = self._task_or_future
         if task is None:
             with suppress(PendingError):
                 return self.value
             raise AttributeError("task is None")
 
-        coro = _as_coro(task)
-        future = run_coroutine_threadsafe(coro, loop=task.get_loop())
-        return future.result(timeout)
+        async def wrap_task() -> ValueT_co:
+            task = self._task_or_future
+            if task is None:
+                with suppress(PendingError):
+                    return self.value
+                raise AttributeError("task is None")
+            return await _wait_for(task, timeout)
+
+        return anyio.from_thread.run(wrap_task)
 
     def _set_task_or_future(
         self,
-        task_or_future: Task[ValueT_co] | Future[ValueT_co],
+        task_or_future: Futurelike[ValueT_co],
     ) -> None:
         if self._value is not Pending:
             raise AttributeError("value is already setted")
         task_or_future.add_done_callback(self._set_from_task_or_future)
         self._task_or_future = task_or_future
 
     def _set_from_task_or_future(
         self,
-        task_or_future: Task[ValueT_co] | Future[ValueT_co],
+        task_or_future: Futurelike[ValueT_co],
     ) -> None:
         if task_or_future.exception() is None:
             self.value = task_or_future.result()
         if self._task_or_future is not None:
             self._task_or_future = None
 
 
 class TaskGroupFactory(Protocol[TaskGroupT_co]):
     def __call__(self) -> TaskGroupT_co:  # noqa: D102
         ...
 
 
-async def _as_coro(
-    task_or_future: Task[Any] | Future[Any],
-) -> Any:
-    return await task_or_future
+async def _wait_for(
+    future: Futurelike[ValueT_co],
+    timeout: float | None = None,
+) -> ValueT_co:
+    async with anyio.maybe_async_cm(anyio.fail_after(timeout)):
+        return await future
```

### Comparing `async_wrapper-0.1.6/src/async_wrapper/task_group/main.py` & `async_wrapper-0.2.1/src/async_wrapper/task_group/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 if TYPE_CHECKING:
     from async_wrapper.task_group import _anyio as anyio_task_group
     from async_wrapper.task_group import _asyncio as asyncio_task_group
     from async_wrapper.task_group.base import TaskGroupFactory
 
 __all__ = ["get_task_group_wrapper", "get_task_group_factory", "get_semaphore_class"]
 
-DEFAULT_BACKEND = "asyncio"
+DEFAULT_BACKEND = "anyio"
 TaskGroupBackendType = Literal["asyncio", "anyio"]
 
 
 @overload
 def get_task_group_wrapper(
-    backend: Literal["asyncio"] | None = ...,
-) -> type[asyncio_task_group.SoonWrapper]:
+    backend: Literal["anyio"] | None = ...,
+) -> type[anyio_task_group.SoonWrapper]:
     ...
 
 
 @overload
 def get_task_group_wrapper(
-    backend: Literal["anyio"] = ...,
-) -> type[anyio_task_group.SoonWrapper]:
+    backend: Literal["asyncio"] = ...,
+) -> type[asyncio_task_group.SoonWrapper]:
     ...
 
 
 def get_task_group_wrapper(
     backend: TaskGroupBackendType | None = None,
 ) -> type[anyio_task_group.SoonWrapper] | type[asyncio_task_group.SoonWrapper]:
     """get task group wrapper
@@ -44,23 +44,23 @@
 
     module = importlib.import_module(f"._{backend}", __package__)
     return module.wrap_soon
 
 
 @overload
 def get_task_group_factory(
-    backend: Literal["asyncio"] | None = ...,
-) -> TaskGroupFactory[asyncio_task_group.TaskGroup]:
+    backend: Literal["anyio"] | None = ...,
+) -> TaskGroupFactory[anyio_task_group.TaskGroup]:
     ...
 
 
 @overload
 def get_task_group_factory(
-    backend: Literal["anyio"] = ...,
-) -> TaskGroupFactory[anyio_task_group.TaskGroup]:
+    backend: Literal["asyncio"] = ...,
+) -> TaskGroupFactory[asyncio_task_group.TaskGroup]:
     ...
 
 
 def get_task_group_factory(
     backend: TaskGroupBackendType | None = None,
 ) -> (
     TaskGroupFactory[asyncio_task_group.TaskGroup]
@@ -79,23 +79,23 @@
 
     module = importlib.import_module(f"._{backend}", __package__)
     return module.get_task_group
 
 
 @overload
 def get_semaphore_class(
-    backend: Literal["asyncio"] | None = ...,
-) -> type[asyncio_task_group.AsyncioSemaphore]:
+    backend: Literal["anyio"] | None = ...,
+) -> type[anyio_task_group.AnyioSemaphore]:
     ...
 
 
 @overload
 def get_semaphore_class(
-    backend: Literal["anyio"] = ...,
-) -> type[anyio_task_group.AnyioSemaphore]:
+    backend: Literal["asyncio"] = ...,
+) -> type[asyncio_task_group.AsyncioSemaphore]:
     ...
 
 
 def get_semaphore_class(
     backend: TaskGroupBackendType | None = None,
 ) -> type[asyncio_task_group.AsyncioSemaphore] | type[anyio_task_group.AnyioSemaphore]:
     """get semaphore class using in wrap func
```

### Comparing `async_wrapper-0.1.6/PKG-INFO` & `async_wrapper-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.1.6
+Version: 0.2.1
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
-Provides-Extra: anyio
 Provides-Extra: loky
 Requires-Dist: aiotools (>=1.6.1,<2.0.0) ; python_version < "3.11"
-Requires-Dist: anyio (>=3.7.0,<4.0.0) ; extra == "all" or extra == "anyio"
+Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: loky (>=3.4.0,<4.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: psutil (>=5.9.5,<6.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: pyyaml (>=6.0.1)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
@@ -35,16 +34,14 @@
 
 ## how to install
 ```shell
 $ pip install async_wrapper
 # or
 $ pip install "async_wrapper[all]"
 # or
-$ pip install "async_wrapper[anyio]"
-# or
 $ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
 from __future__ import annotations
```

