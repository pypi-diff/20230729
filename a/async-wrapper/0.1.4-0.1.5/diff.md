# Comparing `tmp/async_wrapper-0.1.4.tar.gz` & `tmp/async_wrapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.1.4.tar", max compression
+gzip compressed data, was "async_wrapper-0.1.5.tar", max compression
```

## Comparing `async_wrapper-0.1.4.tar` & `async_wrapper-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-07-20 11:12:04.820027 async_wrapper-0.1.4/LICENSE
--rw-r--r--   0        0        0     1892 2023-07-20 11:12:04.820027 async_wrapper-0.1.4/README.md
--rw-r--r--   0        0        0     3648 2023-07-20 11:12:20.764335 async_wrapper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      419 2023-07-20 11:12:04.820027 async_wrapper-0.1.4/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-07-20 11:12:20.804336 async_wrapper-0.1.4/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0      896 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      706 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1217 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1581 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      209 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     3495 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     2960 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/_asyncio.py
--rw-r--r--   0        0        0     2491 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     2735 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 async_wrapper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-29 15:07:09.471177 async_wrapper-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1892 2023-07-29 15:07:09.471177 async_wrapper-0.1.5/README.md
+-rw-r--r--   0        0        0     3682 2023-07-29 15:07:28.700613 async_wrapper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      419 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-29 15:07:28.748615 async_wrapper-0.1.5/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0      896 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      706 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1217 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1581 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      209 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     4414 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/_anyio.py
+-rw-r--r--   0        0        0     3258 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/_asyncio.py
+-rw-r--r--   0        0        0     5558 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/base.py
+-rw-r--r--   0        0        0     2735 2023-07-29 15:07:09.475177 async_wrapper-0.1.5/src/async_wrapper/task_group/main.py
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 async_wrapper-0.1.5/PKG-INFO
```

### Comparing `async_wrapper-0.1.4/LICENSE` & `async_wrapper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/README.md` & `async_wrapper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/pyproject.toml` & `async_wrapper-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.1.4"
+version = "0.1.5"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
@@ -13,14 +13,15 @@
 python = ">=3.8"
 typing-extensions = "^4.6.3"
 anyio = { version = "^3.7.0", optional = true }
 aiotools = { version = "^1.6.1", python = "<3.11" }
 loky = { version = "^3.4.0", optional = true }
 cloudpickle = { version = "^2.2.1", optional = true }
 psutil = { version = "^5.9.5", optional = true }
+pyyaml = ">=6.0.1" # cython error
 
 [tool.poetry.extras]
 all = ['anyio', 'loky', "cloudpickle", "psutil"]
 anyio = ['anyio']
 loky = ['loky', "cloudpickle", "psutil"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/main.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.1.5/src/async_wrapper/convert/synclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.1.5/src/async_wrapper/task_group/_anyio.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,113 @@
 from __future__ import annotations
 
-from contextlib import AsyncExitStack
+from asyncio import create_task, wait
 from functools import partial, wraps
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
 
 from typing_extensions import ParamSpec, Self, override
 
-from async_wrapper.task_group.base import BaseSoonWrapper, Semaphore, SoonValue
+from async_wrapper.task_group.base import (
+    BaseSoonWrapper,
+    BaseTaskGroup,
+    Semaphore,
+    SoonValue,
+)
 
 try:
-    from anyio.abc import TaskGroup  # type: ignore
+    from anyio.abc import TaskGroup as _TaskGroup  # type: ignore
 except ImportError:
-    from typing import Any as TaskGroup
+    from typing import Any as _TaskGroup
 
 if TYPE_CHECKING:
+    from asyncio import Task
+    from types import TracebackType
+
     from anyio.abc import Semaphore as AnyioSemaphore  # type: ignore
 
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 __all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
 
 
+class TaskGroup(BaseTaskGroup):
+    def __init__(self) -> None:
+        self._task_group: _TaskGroup = _get_task_group()
+        self._tasks: WeakSet[Task[Any]] = WeakSet()
+
+    @override
+    def start_soon(
+        self,
+        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
+        *args: ParamT.args,
+        **kwargs: ParamT.kwargs,
+    ) -> SoonValue[ValueT_co]:
+        value = SoonValue()
+        wrapped = self._wrap_as_value(func, value)
+        self._task_group.start_soon(partial(wrapped, **kwargs), *args)
+        return value
+
+    def _wrap_as_value(
+        self,
+        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
+        value: SoonValue[ValueT_co],
+    ) -> Callable[ParamT, Coroutine[None, None, None]]:
+        @wraps(func)
+        async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> None:
+            coro = func(*args, **kwargs)
+            task = create_task(coro)
+            value._set_task_or_future(task)  # noqa: SLF001
+            self.tasks.add(task)
+            await task
+
+        return inner
+
+    @property
+    @override
+    def is_active(self) -> bool:
+        return self._task_group._active  # type: ignore # noqa: SLF001
+
+    @property
+    @override
+    def tasks(self) -> WeakSet[Task[Any]]:
+        return self._tasks
+
+    @override
+    async def __aenter__(self) -> Self:
+        await self._task_group.__aenter__()
+        return self
+
+    @override
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> Any:
+        tasks = tuple(self.tasks)
+        if tasks:
+            await wait(tasks)
+        return await self._task_group.__aexit__(exc_type, exc, traceback)
+
+
 @final
 class SoonWrapper(
     BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
     Generic[ParamT, ValueT_co],
 ):
     @override
     def __new__(
@@ -51,74 +120,40 @@
             import anyio  # type: ignore # noqa: F401
         except ImportError as exc:
             raise ImportError("install extas anyio first") from exc
 
         return super().__new__(cls, func, task_group, semaphore)  # type: ignore
 
     @override
-    def __init__(
-        self,
-        func: Callable[ParamT, Awaitable[ValueT_co]],
-        task_group: TaskGroup,
-        semaphore: Semaphore | None = None,
-    ) -> None:
-        super().__init__(func, task_group, semaphore)
-
-        def outer(
-            result: SoonValue[ValueT_co],
-        ) -> Callable[ParamT, None]:
-            @wraps(self.func)
-            def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> None:
-                partial_func = partial(self.func, *args, **kwargs)
-                set_value_func = partial(_set_value, partial_func, result, semaphore)
-                task_group.start_soon(set_value_func)
-
-            return inner
-
-        self._func = outer
-
-    @override
     def __call__(
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
-        result: SoonValue[ValueT_co] = SoonValue()
-        self._func(result)(*args, **kwargs)
-        return result
+        wrapped = self.task_group._wrap(self.func, self.semaphore)  # noqa: SLF001
+        return self.task_group.start_soon(wrapped, *args, **kwargs)
 
     @override
     def copy(self, semaphore: Semaphore | None = None) -> Self:
         if semaphore is None:
             semaphore = self.semaphore
         return SoonWrapper(self.func, self.task_group, semaphore)
 
 
-def get_task_group() -> TaskGroup:
-    try:
-        from anyio import create_task_group  # type: ignore
-    except ImportError as exc:
-        raise ImportError("install extas anyio first") from exc
-    return create_task_group()
-
-
 def get_semaphore_class() -> type[AnyioSemaphore]:
     try:
         from anyio import Semaphore as _Semaphore  # type: ignore
     except ImportError as exc:
         raise ImportError("install extas anyio first") from exc
     return _Semaphore
 
 
-async def _set_value(
-    func: Callable[[], Coroutine[Any, Any, ValueT]],
-    value: SoonValue[ValueT],
-    semaphore: Semaphore | None,
-) -> None:
-    async with AsyncExitStack() as stack:
-        if semaphore is not None:
-            await stack.enter_async_context(semaphore)
-        result = await func()
-    value.value = result
+def _get_task_group() -> _TaskGroup:
+    try:
+        from anyio import create_task_group  # type: ignore
+    except ImportError as exc:
+        raise ImportError("install extas anyio first") from exc
+    return create_task_group()
 
 
 wrap_soon = SoonWrapper
+get_task_group = TaskGroup
```

### Comparing `async_wrapper-0.1.4/src/async_wrapper/task_group/_asyncio.py` & `async_wrapper-0.1.5/src/async_wrapper/task_group/_asyncio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,95 @@
 from __future__ import annotations
 
 import sys
 from asyncio import Semaphore as AsyncioSemaphore
-from contextlib import AsyncExitStack
-from functools import partial, wraps
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
 
 from typing_extensions import ParamSpec, Self, override
 
-from async_wrapper.task_group.base import BaseSoonWrapper, Semaphore, SoonValue
+from async_wrapper.task_group.base import (
+    BaseSoonWrapper,
+    BaseTaskGroup,
+    Semaphore,
+    SoonValue,
+)
 
 if sys.version_info < (3, 11):
-    from aiotools.taskgroup import TaskGroup  # type: ignore
+    from aiotools.taskgroup import TaskGroup as _TaskGroup  # type: ignore
 else:
-    from asyncio.taskgroups import TaskGroup  # type: ignore
+    from asyncio.taskgroups import TaskGroup as _TaskGroup  # type: ignore
 
+if TYPE_CHECKING:
+    from asyncio import Task
+    from types import TracebackType
+    from weakref import WeakSet
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 __all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
 
 
+class TaskGroup(BaseTaskGroup):
+    def __init__(self) -> None:
+        self._task_group = _TaskGroup()
+        self._semaphore = None
+
+    @override
+    def start_soon(
+        self,
+        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
+        *args: ParamT.args,
+        **kwargs: ParamT.kwargs,
+    ) -> SoonValue[ValueT_co]:
+        coro = func(*args, **kwargs)
+        task = self._task_group.create_task(coro)
+        return SoonValue(task_or_future=task)
+
+    @property
+    @override
+    def is_active(self) -> bool:
+        return self._task_group._entered  # noqa: SLF001
+
+    @property
+    @override
+    def tasks(self) -> WeakSet[Task[Any]]:
+        return self._task_group._tasks  # noqa: SLF001
+
+    @override
+    async def __aenter__(self) -> Self:
+        await self._task_group.__aenter__()
+        return self
+
+    @override
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> Any:
+        tasks = tuple(self.tasks)
+        if tasks:
+            await wait(tasks)
+        return await self._task_group.__aexit__(exc_type, exc, traceback)
+
+
 @final
 class SoonWrapper(
     BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
     Generic[ParamT, ValueT_co],
 ):
     if TYPE_CHECKING:
 
@@ -47,63 +99,28 @@
             func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
             task_group: TaskGroup,
             semaphore: Semaphore | None = None,
         ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
             ...
 
     @override
-    def __init__(
-        self,
-        func: Callable[ParamT, Awaitable[ValueT_co]],
-        task_group: TaskGroup,
-        semaphore: Semaphore | None = None,
-    ) -> None:
-        super().__init__(func, task_group, semaphore)
-
-        def outer(
-            result: SoonValue[ValueT_co],
-        ) -> Callable[ParamT, None]:
-            @wraps(self.func)
-            def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> None:
-                partial_func = partial(self.func, *args, **kwargs)
-                set_value_func = partial(_set_value, partial_func, result, semaphore)
-                task_group.create_task(set_value_func())
-
-            return inner
-
-        self._func = outer
-
-    @override
     def __call__(
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
-        result: SoonValue[ValueT_co] = SoonValue()
-        self._func(result)(*args, **kwargs)
-        return result
+        wrapped = self.task_group._wrap(self.func, self.semaphore)  # noqa: SLF001
+        return self.task_group.start_soon(wrapped, *args, **kwargs)
 
     @override
     def copy(self, semaphore: Semaphore | None = None) -> Self:
         if semaphore is None:
             semaphore = self.semaphore
         return SoonWrapper(self.func, self.task_group, semaphore)
 
 
 def get_semaphore_class() -> type[AsyncioSemaphore]:
     return AsyncioSemaphore
 
 
-async def _set_value(
-    func: Callable[[], Coroutine[Any, Any, ValueT]],
-    value: SoonValue[ValueT],
-    semaphore: Semaphore | None,
-) -> None:
-    async with AsyncExitStack() as stack:
-        if semaphore is not None:
-            await stack.enter_async_context(semaphore)
-        result = await func()
-    value.value = result
-
-
 wrap_soon = SoonWrapper
 get_task_group = TaskGroup
```

### Comparing `async_wrapper-0.1.4/src/async_wrapper/task_group/main.py` & `async_wrapper-0.1.5/src/async_wrapper/task_group/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.4/PKG-INFO` & `async_wrapper-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.1.4
+Version: 0.1.5
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Provides-Extra: anyio
 Provides-Extra: loky
 Requires-Dist: aiotools (>=1.6.1,<2.0.0) ; python_version < "3.11"
 Requires-Dist: anyio (>=3.7.0,<4.0.0) ; extra == "all" or extra == "anyio"
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: loky (>=3.4.0,<4.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: psutil (>=5.9.5,<6.0.0) ; extra == "all" or extra == "loky"
+Requires-Dist: pyyaml (>=6.0.1)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

