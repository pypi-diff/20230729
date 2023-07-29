# Comparing `tmp/parallelism-0.0.2.tar.gz` & `tmp/parallelism-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallelism-0.0.2.tar", last modified: Fri Jul 28 19:21:41 2023, max compression
+gzip compressed data, was "parallelism-0.0.3.tar", last modified: Sat Jul 29 17:58:06 2023, max compression
```

## Comparing `parallelism-0.0.2.tar` & `parallelism-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.084377 parallelism-0.0.2/
--rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.0.2/.gitignore
--rw-rw-rw-   0        0        0       72 2023-07-28 18:43:52.000000 parallelism-0.0.2/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      674 2023-07-28 19:21:41.084377 parallelism-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.021891 parallelism-0.0.2/docs/
--rw-rw-rw-   0        0        0        2 2023-07-28 18:56:26.000000 parallelism-0.0.2/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.037513 parallelism-0.0.2/parallelism/
--rw-rw-rw-   0        0        0      296 2023-07-28 19:21:11.000000 parallelism-0.0.2/parallelism/__init__.py
--rw-rw-rw-   0        0        0     5367 2023-07-28 19:18:53.000000 parallelism-0.0.2/parallelism/api_reference.py
--rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.0.2/parallelism/config.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.068755 parallelism-0.0.2/parallelism/core/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.0.2/parallelism/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.068755 parallelism-0.0.2/parallelism/core/exceptions/
--rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.0.2/parallelism/core/exceptions/__init__.py
--rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.0.2/parallelism/core/exceptions/dependency_error.py
--rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.0.2/parallelism/core/exceptions/worker_error.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.068755 parallelism-0.0.2/parallelism/core/executors/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.0.2/parallelism/core/executors/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.0.2/parallelism/core/executors/process_executor.py
--rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.0.2/parallelism/core/executors/thread_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.084377 parallelism-0.0.2/parallelism/core/handlers/
--rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.0.2/parallelism/core/handlers/__init__.py
--rw-rw-rw-   0        0        0     3254 2023-07-28 11:30:13.000000 parallelism-0.0.2/parallelism/core/handlers/dependency_handler.py
--rw-rw-rw-   0        0        0      340 2023-07-18 13:08:21.000000 parallelism-0.0.2/parallelism/core/handlers/error_handler.py
--rw-rw-rw-   0        0        0     6888 2023-07-28 11:34:19.000000 parallelism-0.0.2/parallelism/core/handlers/function_handler.py
--rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.0.2/parallelism/core/handlers/parameters_handler.py
--rw-rw-rw-   0        0        0     2223 2023-07-27 17:39:03.000000 parallelism-0.0.2/parallelism/core/handlers/shared_memory_handler.py
--rw-rw-rw-   0        0        0     1388 2023-07-21 22:43:02.000000 parallelism-0.0.2/parallelism/core/return_value.py
--rw-rw-rw-   0        0        0     3122 2023-07-27 17:19:10.000000 parallelism-0.0.2/parallelism/core/scheduled_task.py
--rw-rw-rw-   0        0        0      399 2023-07-25 21:47:04.000000 parallelism-0.0.2/parallelism/core/scheduler_result.py
--rw-rw-rw-   0        0        0     7070 2023-07-28 11:30:13.000000 parallelism-0.0.2/parallelism/core/task_scheduler.py
--rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.0.2/parallelism/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.053136 parallelism-0.0.2/parallelism.egg-info/
--rw-rw-rw-   0        0        0      674 2023-07-28 19:21:40.000000 parallelism-0.0.2/parallelism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1020 2023-07-28 19:21:41.000000 parallelism-0.0.2/parallelism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 19:21:40.000000 parallelism-0.0.2/parallelism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-28 19:21:40.000000 parallelism-0.0.2/parallelism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 19:21:41.084377 parallelism-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.321160 parallelism-0.0.3/
+-rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.0.3/.gitignore
+-rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.0.3/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      674 2023-07-29 17:58:06.321160 parallelism-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.177020 parallelism-0.0.3/docs/
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.192642 parallelism-0.0.3/docs/api_reference/
+-rw-rw-rw-   0        0        0      249 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/api_reference/scheduled_task.rst
+-rw-rw-rw-   0        0        0      249 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/api_reference/task_scheduler.rst
+-rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/conf.py
+-rw-rw-rw-   0        0        0      986 2023-07-29 11:22:19.000000 parallelism-0.0.3/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.210966 parallelism-0.0.3/parallelism/
+-rw-rw-rw-   0        0        0      296 2023-07-29 17:56:59.000000 parallelism-0.0.3/parallelism/__init__.py
+-rw-rw-rw-   0        0        0     7123 2023-07-29 17:13:19.000000 parallelism-0.0.3/parallelism/api_reference.py
+-rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.0.3/parallelism/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.257831 parallelism-0.0.3/parallelism/core/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.0.3/parallelism/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.273483 parallelism-0.0.3/parallelism/core/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.0.3/parallelism/core/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.0.3/parallelism/core/exceptions/dependency_error.py
+-rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.0.3/parallelism/core/exceptions/worker_error.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.289074 parallelism-0.0.3/parallelism/core/executors/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.0.3/parallelism/core/executors/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.0.3/parallelism/core/executors/process_executor.py
+-rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.0.3/parallelism/core/executors/thread_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.321160 parallelism-0.0.3/parallelism/core/handlers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.0.3/parallelism/core/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.0.3/parallelism/core/handlers/dependency_handler.py
+-rw-rw-rw-   0        0        0      340 2023-07-18 13:08:21.000000 parallelism-0.0.3/parallelism/core/handlers/error_handler.py
+-rw-rw-rw-   0        0        0     6888 2023-07-28 11:34:19.000000 parallelism-0.0.3/parallelism/core/handlers/function_handler.py
+-rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.0.3/parallelism/core/handlers/parameters_handler.py
+-rw-rw-rw-   0        0        0     2718 2023-07-29 17:54:53.000000 parallelism-0.0.3/parallelism/core/handlers/shared_memory_handler.py
+-rw-rw-rw-   0        0        0     1388 2023-07-21 22:43:02.000000 parallelism-0.0.3/parallelism/core/return_value.py
+-rw-rw-rw-   0        0        0     3247 2023-07-29 17:19:03.000000 parallelism-0.0.3/parallelism/core/scheduled_task.py
+-rw-rw-rw-   0        0        0      399 2023-07-25 21:47:04.000000 parallelism-0.0.3/parallelism/core/scheduler_result.py
+-rw-rw-rw-   0        0        0     7102 2023-07-29 17:27:16.000000 parallelism-0.0.3/parallelism/core/task_scheduler.py
+-rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.0.3/parallelism/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:58:06.242210 parallelism-0.0.3/parallelism.egg-info/
+-rw-rw-rw-   0        0        0      674 2023-07-29 17:58:05.000000 parallelism-0.0.3/parallelism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1109 2023-07-29 17:58:06.000000 parallelism-0.0.3/parallelism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 17:58:05.000000 parallelism-0.0.3/parallelism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-29 17:58:05.000000 parallelism-0.0.3/parallelism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 17:58:06.321160 parallelism-0.0.3/setup.cfg
```

### Comparing `parallelism-0.0.2/.gitignore` & `parallelism-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.2/LICENSE` & `parallelism-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.2/PKG-INFO` & `parallelism-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.0.2
+Version: 0.0.3
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.0.2/parallelism/api_reference.py` & `parallelism-0.0.3/parallelism/api_reference.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,14 +28,40 @@
     *,
     dependencies: Tuple[ScheduledTask, ...] = None,
     priority: Union[int, float] = None,
     processes: int = 0,
     threads: int = 0,
     continual: bool = False,
 ) -> ScheduledTask:
+    """
+    Schedule a task to be executed at the right moment in the task scheduler
+
+    Parameters
+    ----------
+    executor : multiprocessing.Process or threading.Thread
+        | The execution unit of a task
+    name : str
+        | A unique identifier representing a task
+    target : callable
+        | A function to be invoked by a task scheduler
+    args : tuple, optional
+        | Positional arguments that are related to the target
+    kwargs : dict, optional
+        | Keyword arguments that are related to the target
+    dependencies : tuple of ScheduledTask, optional
+        | Certain tasks that create dependencies for the current task
+    priority : int or float, optional
+        | Priority level of task execution over others
+    processes : int, default 0
+        | The number of processes will be allocated retrospectively at runtime
+    threads : int, default 0
+        | The number of threads will be allocated retrospectively at runtime
+    continual : bool, default False
+        | An indicator to save the result after the task scheduler
+    """
     if args is None:
         args = ()
     if kwargs is None:
         kwargs = {}
     if dependencies is None:
         dependencies = ()
     if priority is None:
@@ -100,14 +126,26 @@
 
 def task_scheduler(
     tasks: Tuple[ScheduledTask, ...],
     *,
     processes: int = None,
     threads: int = None,
 ) -> SchedulerResult:
+    """
+    Schedule multiple tasks for execution
+
+    Parameters
+    ----------
+    tasks : tuple of ScheduledTask
+        | Tasks that need to be performed
+    processes : int, optional
+        | The number of processes assigned to perform the tasks
+    threads : int, optional
+        | The number of threads assigned to perform the tasks
+    """
     if processes is None:
         processes = processes or cpu_count() or 1
     if threads is None:
         threads = threads or cpu_count() or 1
     if not isinstance(tasks, tuple):
         pattern = 'The {!r} parameter should be of type {!r}'
         raise TypeError(pattern.format('tasks', 'tuple'))
@@ -119,12 +157,18 @@
         raise TypeError(pattern.format('name', 'tasks'))
     if not DependencyHandler.directed_acyclic_graph(tasks):
         pattern = 'Dependencies of the tasks contains cycles'
         raise TypeError(pattern)
     if not isinstance(processes, int):
         pattern = 'The {!r} parameter should be of type {!r}'
         raise TypeError(pattern.format('processes', 'int'))
+    if processes < 0:
+        pattern = 'The {!r} parameter should be an integer >= {!r}'
+        raise TypeError(pattern.format('processes', 0))
     if not isinstance(threads, int):
         pattern = 'The {!r} parameter should be of type {!r}'
         raise TypeError(pattern.format('threads', 'int'))
+    if threads < 0:
+        pattern = 'The {!r} parameter should be an integer >= {!r}'
+        raise TypeError(pattern.format('threads', 0))
     scheduler = TaskScheduler(tasks, processes, threads)
     return scheduler.execute()
```

### Comparing `parallelism-0.0.2/parallelism/core/executors/process_executor.py` & `parallelism-0.0.3/parallelism/core/executors/process_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.2/parallelism/core/executors/thread_executor.py` & `parallelism-0.0.3/parallelism/core/executors/thread_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.2/parallelism/core/handlers/dependency_handler.py` & `parallelism-0.0.3/parallelism/core/handlers/dependency_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,28 +27,28 @@
         return prerequisite
 
     def is_blocked(
         self,
         task: ScheduledTask,
         status: Literal['finish', 'complete'],
     ) -> bool:
-        task_names = tuple(task.name for task in self.depends_on(task))
-        return len(task_names) != sum(
+        tasks = tuple(task for task in self.depends_on(task))
+        return len(tasks) != sum(
             task.initialized and
             self.proxy.get(task.name).get(status)
             for task in self.tasks
-            if task.name in task_names
+            if task in tasks
         )
 
     def blocking_tasks(self, task: ScheduledTask) -> Tuple[str, ...]:
-        task_names = tuple(task.name for task in self.depends_on(task))
+        tasks = tuple(task for task in self.depends_on(task))
         return tuple(
             task.name for task in self.tasks
             if (
-                task.name in task_names and
+                task in tasks and
                 task.initialized and not
                 self.proxy.get(task.name).get('complete')
             )
         )
 
     @staticmethod
     def depends_on(task: ScheduledTask) -> Set[ScheduledTask]:
```

### Comparing `parallelism-0.0.2/parallelism/core/handlers/function_handler.py` & `parallelism-0.0.3/parallelism/core/handlers/function_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.2/parallelism/core/handlers/parameters_handler.py` & `parallelism-0.0.3/parallelism/core/handlers/parameters_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.2/parallelism/core/handlers/shared_memory_handler.py` & `parallelism-0.0.3/parallelism/core/handlers/shared_memory_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+from parallelism.core.scheduled_task import ScheduledTask
 
 if TYPE_CHECKING:
     from multiprocessing.managers import DictProxy
     from typing import Dict, List, Tuple
 
-    from parallelism.core.scheduled_task import ScheduledTask
-
 __all__ = ('SharedMemoryHandler',)
 
 
 class SharedMemoryHandler:
     __slots__ = (
         'tasks',
         'proxy',
@@ -30,39 +29,52 @@
         self.tasks = tasks
         self.proxy = proxy
         self.prerequisites = prerequisites
         self.elapsed_time = {}
         self.error_handler = {}
         self.return_value = {}
 
-    def free(self, task: ScheduledTask) -> None:
+    def free(self, index: int, task: ScheduledTask) -> None:
         proxy = self.proxy.get(task.name)
         if (
             proxy.get('finish') and
             self.has_shared_memory(task) and
             self.prerequisites_been_initialized(task)
         ):
             if proxy.get('elapsed_time'):
                 self.elapsed_time[task.name] = proxy.get('elapsed_time')
             if proxy.get('error_handler'):
                 self.error_handler[task.name] = proxy.get('error_handler')
             elif task.continual:
                 self.return_value[task.name] = proxy.get('return_value')
+            self.tasks[index] = ScheduledTask(
+                executor=task.executor.__class__.__base__,
+                name=task.name,
+                target=task.target,
+                args=(),
+                kwargs={},
+                dependencies=task.dependencies,
+                priority=task.priority,
+                processes=task.processes,
+                threads=task.threads,
+                continual=task.continual,
+                initialized=task.initialized,
+            )
             del self.proxy[task.name]['elapsed_time']
             del self.proxy[task.name]['error_handler']
             del self.proxy[task.name]['return_value']
 
     def has_shared_memory(self, task: ScheduledTask) -> bool:
         proxy = self.proxy.get(task.name)
         return (
             'elapsed_time' in proxy or
             'error_handler' in proxy or
             'return_value' in proxy
         )
 
     def prerequisites_been_initialized(self, task: ScheduledTask) -> bool:
         task_prerequisites = self.prerequisites.get(task.name)
-        task_names = tuple(task.name for task in task_prerequisites)
+        tasks = tuple(task for task in task_prerequisites)
         return all(
             task.initialized for task in self.tasks
-            if task.name in task_names
+            if task in tasks
         )
```

### Comparing `parallelism-0.0.2/parallelism/core/return_value.py` & `parallelism-0.0.3/parallelism/core/return_value.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.2/parallelism/core/scheduled_task.py` & `parallelism-0.0.3/parallelism/core/scheduled_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     threads: int
     continual: bool
     initialized: bool
 
     def __hash__(self) -> int:
         return hash(self.name)
 
+    def __eq__(self, other: ScheduledTask) -> bool:
+        return type(self) is type(other) and self.name == other.name
+
     def __repr__(self) -> str:
         parameters = (
             'executor={!r}'.format(self.reformat_executor),
             'name={!r}'.format(self.name),
             'target={!r}'.format(self.reformat_target),
             'args={!r}'.format(self.amount_of_args),
             'kwargs={!r}'.format(self.amount_of_kwargs),
```

### Comparing `parallelism-0.0.2/parallelism/core/task_scheduler.py` & `parallelism-0.0.3/parallelism/core/task_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             if not self.enough_workers(task):
                 self.proxy[task.name] = self.manager.dict()
                 task = self.initialize(task, blocked='worker')
                 self.tasks[index] = task
         while not self.finished:
             for index, task in enumerate(self.tasks):
                 if task.initialized:
-                    self.shared_memory_handler.free(task)
+                    self.shared_memory_handler.free(index, task)
                     continue
                 if not self.available_worker(task):
                     continue
                 if self.dependency_handler.is_blocked(task, status='finish'):
                     continue
                 if self.dependency_handler.is_blocked(task, status='complete'):
                     self.proxy[task.name] = self.manager.dict()
@@ -108,16 +108,16 @@
                     self.tasks[index] = task
                     continue
                 self.proxy[task.name] = self.manager.dict()
                 task = self.initialize(task)
                 self.tasks[index] = task
                 task.executor.start()
                 break
-        for task in self.tasks:
-            self.shared_memory_handler.free(task)
+        for index, task in enumerate(self.tasks):
+            self.shared_memory_handler.free(index, task)
         self.manager.shutdown()
         return SchedulerResult(
             self.shared_memory_handler.elapsed_time,
             self.shared_memory_handler.error_handler,
             self.shared_memory_handler.return_value,
         )
```

### Comparing `parallelism-0.0.2/parallelism.egg-info/PKG-INFO` & `parallelism-0.0.3/parallelism.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.0.2
+Version: 0.0.3
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.0.2/parallelism.egg-info/SOURCES.txt` & `parallelism-0.0.3/parallelism.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
+docs/conf.py
 docs/index.rst
+docs/api_reference/scheduled_task.rst
+docs/api_reference/task_scheduler.rst
 parallelism/__init__.py
 parallelism/api_reference.py
 parallelism/config.py
 parallelism/logger.py
 parallelism.egg-info/PKG-INFO
 parallelism.egg-info/SOURCES.txt
 parallelism.egg-info/dependency_links.txt
```

### Comparing `parallelism-0.0.2/pyproject.toml` & `parallelism-0.0.3/pyproject.toml`

 * *Files identical despite different names*

