# Comparing `tmp/async_wrapper-0.2.1.tar.gz` & `tmp/async_wrapper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.2.1.tar", max compression
+gzip compressed data, was "async_wrapper-0.2.2.tar", max compression
```

## Comparing `async_wrapper-0.2.1.tar` & `async_wrapper-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1070 2023-07-29 20:35:14.034783 async_wrapper-0.2.1/LICENSE
--rw-r--r--   0        0        0     1850 2023-07-29 20:35:14.034783 async_wrapper-0.2.1/README.md
--rw-r--r--   0        0        0     3649 2023-07-29 20:35:27.010767 async_wrapper-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      419 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-07-29 20:35:27.042766 async_wrapper-0.2.1/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0     1007 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      564 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1140 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1136 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      209 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     8669 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     3227 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/_asyncio.py
--rw-r--r--   0        0        0     6194 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     2733 2023-07-29 20:35:14.038784 async_wrapper-0.2.1/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     2936 1970-01-01 00:00:00.000000 async_wrapper-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1823 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/README.md
+-rw-r--r--   0        0        0     3565 2023-07-29 21:39:45.196393 async_wrapper-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      419 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-29 21:39:45.244394 async_wrapper-0.2.2/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0     1007 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      564 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1140 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1136 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      209 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     3707 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/_anyio.py
+-rw-r--r--   0        0        0     9566 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/base.py
+-rw-r--r--   0        0        0     1735 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/main.py
+-rw-r--r--   0        0        0     2810 1970-01-01 00:00:00.000000 async_wrapper-0.2.2/PKG-INFO
```

### Comparing `async_wrapper-0.2.1/LICENSE` & `async_wrapper-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/README.md` & `async_wrapper-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 
 async def sample_func_2(x: int) -> int:
     await asyncio.sleep(1)
     return x
 
 
 async def main():
-    wrapper = get_task_group_wrapper("asyncio")
-    factory = get_task_group_factory("asyncio")
-    Semaphore = get_semaphore_class("asyncio")
+    wrapper = get_task_group_wrapper()
+    factory = get_task_group_factory()
+    Semaphore = get_semaphore_class()
     semaphore = Semaphore(2)
 
     start = time.perf_counter()
     async with factory() as task_group:
         wrapped = wrapper(sample_func_2, task_group, semaphore)
         value_1 = wrapped(1)
         value_2 = wrapped(2)
```

### Comparing `async_wrapper-0.2.1/pyproject.toml` & `async_wrapper-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.2.1"
+version = "0.2.2"
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
 anyio = "^3.7.0"
-aiotools = { version = "^1.6.1", python = "<3.11" }
 loky = { version = "^3.4.0", optional = true }
 cloudpickle = { version = "^2.2.1", optional = true }
 psutil = { version = "^5.9.5", optional = true }
-pyyaml = ">=6.0.1"                                    # cython error
 
 [tool.poetry.extras]
 all = ['loky', "cloudpickle", "psutil"]
 loky = ['loky', "cloudpickle", "psutil"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.0.275"
 black = "23.3.0"
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 trio = "^0.22.2"
+pyyaml = ">=6.0.1"    # cython error
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py38"
```

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/main.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.1/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.2.2/src/async_wrapper/task_group/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,63 @@
 from __future__ import annotations
 
 import math
+from abc import ABC, abstractmethod
 from collections import deque
-from functools import partial
+from contextlib import AbstractAsyncContextManager
+from functools import partial, wraps
+from threading import local
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Generator,
     Generic,
     Iterable,
+    Protocol,
     TypeVar,
-    final,
 )
-from weakref import WeakSet
 
-from anyio import (
-    CancelScope,
-    create_memory_object_stream,
-    create_task_group,
-    fail_after,
-    maybe_async_cm,
-)
-from anyio import Event as _Event
-from anyio import Semaphore as _Semaphore
+import anyio
 from typing_extensions import ParamSpec, Self, override
 
-from async_wrapper.task_group.base import (
-    BaseSoonWrapper,
-    BaseTaskGroup,
-    Semaphore,
-    SoonValue,
-)
-
 if TYPE_CHECKING:
     from contextvars import Context
     from types import TracebackType
+    from weakref import WeakSet
 
     from anyio.abc import Event as AnyioEvent
-    from anyio.abc import Semaphore as AnyioSemaphore  # type: ignore
-    from anyio.abc import TaskGroup as _TaskGroup
     from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 
-    from async_wrapper.task_group.base import Futurelike
-
-
+TaskGroupT = TypeVar("TaskGroupT", bound="BaseTaskGroup")
+TaskGroupT_co = TypeVar("TaskGroupT_co", covariant=True, bound="BaseTaskGroup")
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
+Pending = local()
 
-__all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
+__all__ = ["PendingError", "BaseSoonWrapper", "SoonValue", "TaskGroupFactory"]
 
 
-class CancelError(Exception):
+class PendingError(Exception):
     ...
 
 
+class Semaphore(AbstractAsyncContextManager, Protocol):
+    async def acquire(self) -> Any:
+        ...
+
+
 class StreamQueue(Generic[ValueT]):
     def __init__(self, size: float = 0) -> None:
-        setter, getter = create_memory_object_stream(size)
+        setter, getter = anyio.create_memory_object_stream(size)
         self.getter: MemoryObjectReceiveStream[ValueT] = getter
         self.setter: MemoryObjectSendStream[ValueT] = setter
 
     def set(self, value: ValueT) -> None:  # noqa: A003
         self.setter.send_nowait(value)
 
     async def aset(self, value: ValueT) -> None:
@@ -173,148 +164,188 @@
     ) -> None:
         self.callbacks.append((__fn, context))
 
     def add_final_callback(self, func: Callable[[Self], Any]) -> None:
         self.final_callbacks.set(func)
 
 
-class TaskGroup(BaseTaskGroup):
-    def __init__(self) -> None:
-        self._task_group: _TaskGroup = create_task_group()
-        self._futures: WeakSet[Future[Any]] = WeakSet()
-
-    @override
+class BaseTaskGroup(ABC):
+    @abstractmethod
     def start_soon(
         self,
         func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
-        value = SoonValue()
-        future = self._as_future(func, *args, **kwargs)
-        value._set_task_or_future(future)  # noqa: SLF001
-        self._task_group.start_soon(_as_coro, future)
-        return value
-
-    def _as_future(
-        self,
-        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
-        *args: ParamT.args,
-        **kwargs: ParamT.kwargs,
-    ) -> Futurelike[ValueT_co]:
-        coro = func(*args, **kwargs)
-        future = Future(coro)
-        self._futures.add(future)
-        return future
+        ...
 
     @property
-    @override
+    @abstractmethod
     def is_active(self) -> bool:
-        return self._task_group._active  # type: ignore # noqa: SLF001
+        ...
 
     @property
-    @override
+    @abstractmethod
     def tasks(self) -> WeakSet[Future[Any]]:
-        return self._futures
+        ...
 
-    @override
+    @abstractmethod
     async def __aenter__(self) -> Self:
-        await self._task_group.__aenter__()
-        return self
+        ...
 
-    @override
+    @abstractmethod
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         traceback: TracebackType | None,
     ) -> Any:
-        tasks = tuple(self.tasks)
-        if tasks:
-            await _wait(tasks)
-        return await self._task_group.__aexit__(exc_type, exc, traceback)
-
-
-@final
-class SoonWrapper(
-    BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
-    Generic[ParamT, ValueT_co],
-):
-    if TYPE_CHECKING:
-
-        @override
-        def __new__(
-            cls,
-            func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
-            task_group: TaskGroup,
-            semaphore: Semaphore | None = None,
-        ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
-            ...
+        ...
+
+    async def wait(self, tasks: tuple[Future[Any], ...]) -> None:
+        await _wait(tasks)
+
+    @staticmethod
+    def _wrap(
+        func: Callable[ParamT, Awaitable[ValueT_co]],
+        semaphore: Semaphore | None = None,
+    ) -> Callable[ParamT, Coroutine[Any, Any, ValueT_co]]:
+        @wraps(func)
+        async def wrapped(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
+            if semaphore is None:
+                return await func(*args, **kwargs)
+            async with semaphore:
+                return await func(*args, **kwargs)
+
+        return wrapped
+
+
+class BaseSoonWrapper(ABC, Generic[TaskGroupT, ParamT, ValueT_co]):
+    def __init__(
+        self,
+        func: Callable[ParamT, Awaitable[ValueT_co]],
+        task_group: TaskGroupT,
+        semaphore: Semaphore | None = None,
+    ) -> None:
+        self.func = func
+        self.task_group = task_group
+        self.semaphore = semaphore
 
     @override
-    def __call__(
+    def __new__(
+        cls,
+        func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
+        task_group: TaskGroupT,
+        semaphore: Semaphore | None = None,
+    ) -> BaseSoonWrapper[TaskGroupT, OtherParamT, OtherValueT_co]:
+        return super().__new__(cls)  # type: ignore
+
+    @abstractmethod
+    def __call__(  # noqa: D102
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
-        wrapped = self.task_group._wrap(self.func, self.semaphore)  # noqa: SLF001
-        return self.task_group.start_soon(wrapped, *args, **kwargs)
+        ...
 
-    @override
-    def copy(self, semaphore: Semaphore | None = None) -> Self:
-        if semaphore is None:
-            semaphore = self.semaphore
-        return SoonWrapper(self.func, self.task_group, semaphore)
+    @abstractmethod
+    def copy(self, semaphore: Semaphore | None = None) -> Self:  # noqa: D102
+        ...
+
+
+class SoonValue(Generic[ValueT_co]):
+    def __init__(
+        self,
+        future: Future[ValueT_co] | None = None,
+    ) -> None:
+        self._value = Pending
+        if future is None:
+            self._future = None
+        else:
+            self._set_future(future)
 
+    def __repr__(self) -> str:
+        status = "pending" if self._value is Pending else "done"
+        return f"<SoonValue: status={status}>"
 
-def get_semaphore_class() -> type[AnyioSemaphore]:
-    return _Semaphore
+    @property
+    def value(self) -> ValueT_co:  # noqa: D102
+        if self._value is Pending:
+            raise PendingError
+        return self._value  # type: ignore
+
+    @value.setter
+    def value(self, value: Any) -> None:
+        self._value = value
+
+    @value.deleter
+    def value(self) -> None:
+        raise NotImplementedError
+
+    @property
+    def is_ready(self) -> bool:  # noqa: D102
+        return self._value is not Pending
+
+    def _set_future(
+        self,
+        future: Future[ValueT_co],
+    ) -> None:
+        if self._value is not Pending:
+            raise AttributeError("value is already setted")
+        future.add_done_callback(self._set_from_future)
+        self._future = future
+
+    def _set_from_future(
+        self,
+        future: Future[ValueT_co],
+    ) -> None:
+        if future.exception() is None:
+            self.value = future.result()
+        if self._future is not None:
+            self._future = None
+
+
+class TaskGroupFactory(Protocol[TaskGroupT_co]):
+    def __call__(self) -> TaskGroupT_co:  # noqa: D102
+        ...
 
 
 async def _wait(
     futures: Iterable[Future[Any]],
     timeout: float | None = None,
 ) -> None:
     futures = set(futures)
     if not futures:
         return
 
-    async with create_task_group() as task_group:
+    async with anyio.create_task_group() as task_group:
         for future in futures:
             task_group.start_soon(_await, future, timeout)
 
 
 async def _await(future: Future[Any], timeout: float | None) -> None:
     if future.done:
         return
 
-    event = _Event()
+    event = anyio.Event()
     waiter = Future.new(event)
-    scope = CancelScope(shield=True, deadline=timeout or math.inf)
+    scope = anyio.CancelScope(shield=True, deadline=timeout or math.inf)
     callback = partial(_release, waiter=waiter, event=event, scope=scope)
     future.add_final_callback(callback)
 
-    async with maybe_async_cm(fail_after(timeout)):
+    async with anyio.maybe_async_cm(anyio.fail_after(timeout)):
         await waiter
 
 
-async def _as_coro(future: Futurelike[ValueT_co]) -> ValueT_co:
-    return await future
-
-
 def _release(
     future: Future[Any],  # noqa: ARG001
     waiter: Future[Any],
     event: AnyioEvent,
-    scope: CancelScope,
+    scope: anyio.CancelScope,
 ) -> None:
     with scope:
         if not waiter.done:
             event.set()
 
 
 async def _dummy(event: AnyioEvent) -> None:
     await event.wait()
-
-
-wrap_soon = SoonWrapper
-get_task_group = TaskGroup
```

### Comparing `async_wrapper-0.2.1/src/async_wrapper/task_group/_asyncio.py` & `async_wrapper-0.2.2/src/async_wrapper/task_group/_anyio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,91 @@
 from __future__ import annotations
 
-import sys
-from asyncio import Semaphore as AsyncioSemaphore
-from asyncio import wait
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
+from weakref import WeakSet
 
+from anyio import Semaphore as _Semaphore
+from anyio import create_task_group
 from typing_extensions import ParamSpec, Self, override
 
 from async_wrapper.task_group.base import (
     BaseSoonWrapper,
     BaseTaskGroup,
+    Future,
     Semaphore,
     SoonValue,
 )
 
-if sys.version_info < (3, 11):
-    from aiotools.taskgroup import TaskGroup as _TaskGroup  # type: ignore
-else:
-    from asyncio.taskgroups import TaskGroup as _TaskGroup  # type: ignore
-
 if TYPE_CHECKING:
-    from asyncio import Task
     from types import TracebackType
-    from weakref import WeakSet
+
+    from anyio.abc import Semaphore as AnyioSemaphore  # type: ignore
+    from anyio.abc import TaskGroup as _TaskGroup
+
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 __all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
 
 
+class CancelError(Exception):
+    ...
+
+
 class TaskGroup(BaseTaskGroup):
     def __init__(self) -> None:
-        self._task_group = _TaskGroup()
+        self._task_group: _TaskGroup = create_task_group()
+        self._futures: WeakSet[Future[Any]] = WeakSet()
 
     @override
     def start_soon(
         self,
         func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
+        value = SoonValue()
+        future = self._as_future(func, *args, **kwargs)
+        value._set_future(future)  # noqa: SLF001
+        self._task_group.start_soon(_as_coro, future)
+        return value
+
+    def _as_future(
+        self,
+        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
+        *args: ParamT.args,
+        **kwargs: ParamT.kwargs,
+    ) -> Future[ValueT_co]:
         coro = func(*args, **kwargs)
-        task = self._task_group.create_task(coro)
-        return SoonValue(task_or_future=task)
+        future = Future(coro)
+        self._futures.add(future)
+        return future
 
     @property
     @override
     def is_active(self) -> bool:
-        return self._task_group._entered  # noqa: SLF001
+        return self._task_group._active  # type: ignore # noqa: SLF001
 
     @property
     @override
-    def tasks(self) -> WeakSet[Task[Any]]:
-        return self._task_group._tasks  # noqa: SLF001
+    def tasks(self) -> WeakSet[Future[Any]]:
+        return self._futures
 
     @override
     async def __aenter__(self) -> Self:
         await self._task_group.__aenter__()
         return self
 
     @override
@@ -77,15 +93,15 @@
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         traceback: TracebackType | None,
     ) -> Any:
         tasks = tuple(self.tasks)
         if tasks:
-            await wait(tasks)
+            await self.wait(tasks)
         return await self._task_group.__aexit__(exc_type, exc, traceback)
 
 
 @final
 class SoonWrapper(
     BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
     Generic[ParamT, ValueT_co],
@@ -113,13 +129,17 @@
     @override
     def copy(self, semaphore: Semaphore | None = None) -> Self:
         if semaphore is None:
             semaphore = self.semaphore
         return SoonWrapper(self.func, self.task_group, semaphore)
 
 
-def get_semaphore_class() -> type[AsyncioSemaphore]:
-    return AsyncioSemaphore
+def get_semaphore_class() -> type[AnyioSemaphore]:
+    return _Semaphore
+
+
+async def _as_coro(future: Future[ValueT_co]) -> ValueT_co:
+    return await future
 
 
 wrap_soon = SoonWrapper
 get_task_group = TaskGroup
```

### Comparing `async_wrapper-0.2.1/src/async_wrapper/task_group/main.py` & `async_wrapper-0.2.2/src/async_wrapper/task_group/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,67 @@
 from __future__ import annotations
 
 import importlib
-from typing import TYPE_CHECKING, Literal, overload
+from typing import TYPE_CHECKING, Literal
 
 if TYPE_CHECKING:
     from async_wrapper.task_group import _anyio as anyio_task_group
-    from async_wrapper.task_group import _asyncio as asyncio_task_group
     from async_wrapper.task_group.base import TaskGroupFactory
 
 __all__ = ["get_task_group_wrapper", "get_task_group_factory", "get_semaphore_class"]
 
 DEFAULT_BACKEND = "anyio"
-TaskGroupBackendType = Literal["asyncio", "anyio"]
-
-
-@overload
-def get_task_group_wrapper(
-    backend: Literal["anyio"] | None = ...,
-) -> type[anyio_task_group.SoonWrapper]:
-    ...
-
-
-@overload
-def get_task_group_wrapper(
-    backend: Literal["asyncio"] = ...,
-) -> type[asyncio_task_group.SoonWrapper]:
-    ...
+TaskGroupBackendType = Literal["anyio", "asyncio"]
 
 
 def get_task_group_wrapper(
     backend: TaskGroupBackendType | None = None,
-) -> type[anyio_task_group.SoonWrapper] | type[asyncio_task_group.SoonWrapper]:
+) -> type[anyio_task_group.SoonWrapper]:
     """get task group wrapper
 
     Args:
-        backend: anyio or asyncio. Defaults to None.
+        backend: anyio. Defaults to None.
 
     Returns:
         task group soon wrapper
     """
-    if not backend:
+    if not backend or backend == "asyncio":
         backend = DEFAULT_BACKEND
 
     module = importlib.import_module(f"._{backend}", __package__)
     return module.wrap_soon
 
 
-@overload
-def get_task_group_factory(
-    backend: Literal["anyio"] | None = ...,
-) -> TaskGroupFactory[anyio_task_group.TaskGroup]:
-    ...
-
-
-@overload
-def get_task_group_factory(
-    backend: Literal["asyncio"] = ...,
-) -> TaskGroupFactory[asyncio_task_group.TaskGroup]:
-    ...
-
-
 def get_task_group_factory(
     backend: TaskGroupBackendType | None = None,
-) -> (
-    TaskGroupFactory[asyncio_task_group.TaskGroup]
-    | TaskGroupFactory[anyio_task_group.TaskGroup]
-):
+) -> TaskGroupFactory[anyio_task_group.TaskGroup]:
     """get task group factory func
 
     Args:
-        backend: asyncio or anyio. Defaults to None.
+        backend: anyio. Defaults to None.
 
     Returns:
         task group factory
     """
-    if not backend:
+    if not backend or backend == "asyncio":
         backend = DEFAULT_BACKEND
 
     module = importlib.import_module(f"._{backend}", __package__)
     return module.get_task_group
 
 
-@overload
-def get_semaphore_class(
-    backend: Literal["anyio"] | None = ...,
-) -> type[anyio_task_group.AnyioSemaphore]:
-    ...
-
-
-@overload
-def get_semaphore_class(
-    backend: Literal["asyncio"] = ...,
-) -> type[asyncio_task_group.AsyncioSemaphore]:
-    ...
-
-
 def get_semaphore_class(
     backend: TaskGroupBackendType | None = None,
-) -> type[asyncio_task_group.AsyncioSemaphore] | type[anyio_task_group.AnyioSemaphore]:
+) -> type[anyio_task_group.AnyioSemaphore]:
     """get semaphore class using in wrap func
 
     Args:
-        backend: asyncio or anyio. Defaults to None.
+        backend: anyio. Defaults to None.
 
     Returns:
         semaphore class
     """
-    if not backend:
+    if not backend or backend == "asyncio":
         backend = DEFAULT_BACKEND
 
     module = importlib.import_module(f"._{backend}", __package__)
     return module.get_semaphore_class()
```

### Comparing `async_wrapper-0.2.1/PKG-INFO` & `async_wrapper-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.2.1
+Version: 0.2.2
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
 Provides-Extra: loky
-Requires-Dist: aiotools (>=1.6.1,<2.0.0) ; python_version < "3.11"
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: loky (>=3.4.0,<4.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: psutil (>=5.9.5,<6.0.0) ; extra == "all" or extra == "loky"
-Requires-Dist: pyyaml (>=6.0.1)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -69,17 +67,17 @@
 
 async def sample_func_2(x: int) -> int:
     await asyncio.sleep(1)
     return x
 
 
 async def main():
-    wrapper = get_task_group_wrapper("asyncio")
-    factory = get_task_group_factory("asyncio")
-    Semaphore = get_semaphore_class("asyncio")
+    wrapper = get_task_group_wrapper()
+    factory = get_task_group_factory()
+    Semaphore = get_semaphore_class()
     semaphore = Semaphore(2)
 
     start = time.perf_counter()
     async with factory() as task_group:
         wrapped = wrapper(sample_func_2, task_group, semaphore)
         value_1 = wrapped(1)
         value_2 = wrapped(2)
```

