# Comparing `tmp/parallelism-0.0.1.tar.gz` & `tmp/parallelism-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallelism-0.0.1.tar", last modified: Fri Jul 28 19:17:09 2023, max compression
+gzip compressed data, was "parallelism-0.0.2.tar", last modified: Fri Jul 28 19:21:41 2023, max compression
```

## Comparing `parallelism-0.0.1.tar` & `parallelism-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.916064 parallelism-0.0.1/
--rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.0.1/.gitignore
--rw-rw-rw-   0        0        0       72 2023-07-28 18:43:52.000000 parallelism-0.0.1/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      674 2023-07-28 19:17:09.915067 parallelism-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.850602 parallelism-0.0.1/docs/
--rw-rw-rw-   0        0        0        2 2023-07-28 18:56:26.000000 parallelism-0.0.1/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.859578 parallelism-0.0.1/parallelism/
--rw-rw-rw-   0        0        0      296 2023-07-28 18:36:41.000000 parallelism-0.0.1/parallelism/__init__.py
--rw-rw-rw-   0        0        0     5446 2023-07-28 17:09:04.000000 parallelism-0.0.1/parallelism/api_reference.py
--rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.0.1/parallelism/config.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.894486 parallelism-0.0.1/parallelism/core/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.0.1/parallelism/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.897483 parallelism-0.0.1/parallelism/core/exceptions/
--rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.0.1/parallelism/core/exceptions/__init__.py
--rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.0.1/parallelism/core/exceptions/dependency_error.py
--rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.0.1/parallelism/core/exceptions/worker_error.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.903462 parallelism-0.0.1/parallelism/core/executors/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.0.1/parallelism/core/executors/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.0.1/parallelism/core/executors/process_executor.py
--rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.0.1/parallelism/core/executors/thread_executor.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.913071 parallelism-0.0.1/parallelism/core/handlers/
--rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.0.1/parallelism/core/handlers/__init__.py
--rw-rw-rw-   0        0        0     3254 2023-07-28 11:30:13.000000 parallelism-0.0.1/parallelism/core/handlers/dependency_handler.py
--rw-rw-rw-   0        0        0      340 2023-07-18 13:08:21.000000 parallelism-0.0.1/parallelism/core/handlers/error_handler.py
--rw-rw-rw-   0        0        0     6888 2023-07-28 11:34:19.000000 parallelism-0.0.1/parallelism/core/handlers/function_handler.py
--rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.0.1/parallelism/core/handlers/parameters_handler.py
--rw-rw-rw-   0        0        0     2223 2023-07-27 17:39:03.000000 parallelism-0.0.1/parallelism/core/handlers/shared_memory_handler.py
--rw-rw-rw-   0        0        0     1388 2023-07-21 22:43:02.000000 parallelism-0.0.1/parallelism/core/return_value.py
--rw-rw-rw-   0        0        0     3122 2023-07-27 17:19:10.000000 parallelism-0.0.1/parallelism/core/scheduled_task.py
--rw-rw-rw-   0        0        0      399 2023-07-25 21:47:04.000000 parallelism-0.0.1/parallelism/core/scheduler_result.py
--rw-rw-rw-   0        0        0     7070 2023-07-28 11:30:13.000000 parallelism-0.0.1/parallelism/core/task_scheduler.py
--rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.0.1/parallelism/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-28 19:17:09.884513 parallelism-0.0.1/parallelism.egg-info/
--rw-rw-rw-   0        0        0      674 2023-07-28 19:17:09.000000 parallelism-0.0.1/parallelism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1020 2023-07-28 19:17:09.000000 parallelism-0.0.1/parallelism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 19:17:09.000000 parallelism-0.0.1/parallelism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-28 19:17:09.000000 parallelism-0.0.1/parallelism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 19:17:09.917063 parallelism-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.084377 parallelism-0.0.2/
+-rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0       72 2023-07-28 18:43:52.000000 parallelism-0.0.2/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      674 2023-07-28 19:21:41.084377 parallelism-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.021891 parallelism-0.0.2/docs/
+-rw-rw-rw-   0        0        0        2 2023-07-28 18:56:26.000000 parallelism-0.0.2/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.037513 parallelism-0.0.2/parallelism/
+-rw-rw-rw-   0        0        0      296 2023-07-28 19:21:11.000000 parallelism-0.0.2/parallelism/__init__.py
+-rw-rw-rw-   0        0        0     5367 2023-07-28 19:18:53.000000 parallelism-0.0.2/parallelism/api_reference.py
+-rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.0.2/parallelism/config.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.068755 parallelism-0.0.2/parallelism/core/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.0.2/parallelism/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.068755 parallelism-0.0.2/parallelism/core/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.0.2/parallelism/core/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.0.2/parallelism/core/exceptions/dependency_error.py
+-rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.0.2/parallelism/core/exceptions/worker_error.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.068755 parallelism-0.0.2/parallelism/core/executors/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.0.2/parallelism/core/executors/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.0.2/parallelism/core/executors/process_executor.py
+-rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.0.2/parallelism/core/executors/thread_executor.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.084377 parallelism-0.0.2/parallelism/core/handlers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.0.2/parallelism/core/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3254 2023-07-28 11:30:13.000000 parallelism-0.0.2/parallelism/core/handlers/dependency_handler.py
+-rw-rw-rw-   0        0        0      340 2023-07-18 13:08:21.000000 parallelism-0.0.2/parallelism/core/handlers/error_handler.py
+-rw-rw-rw-   0        0        0     6888 2023-07-28 11:34:19.000000 parallelism-0.0.2/parallelism/core/handlers/function_handler.py
+-rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.0.2/parallelism/core/handlers/parameters_handler.py
+-rw-rw-rw-   0        0        0     2223 2023-07-27 17:39:03.000000 parallelism-0.0.2/parallelism/core/handlers/shared_memory_handler.py
+-rw-rw-rw-   0        0        0     1388 2023-07-21 22:43:02.000000 parallelism-0.0.2/parallelism/core/return_value.py
+-rw-rw-rw-   0        0        0     3122 2023-07-27 17:19:10.000000 parallelism-0.0.2/parallelism/core/scheduled_task.py
+-rw-rw-rw-   0        0        0      399 2023-07-25 21:47:04.000000 parallelism-0.0.2/parallelism/core/scheduler_result.py
+-rw-rw-rw-   0        0        0     7070 2023-07-28 11:30:13.000000 parallelism-0.0.2/parallelism/core/task_scheduler.py
+-rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.0.2/parallelism/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:21:41.053136 parallelism-0.0.2/parallelism.egg-info/
+-rw-rw-rw-   0        0        0      674 2023-07-28 19:21:40.000000 parallelism-0.0.2/parallelism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1020 2023-07-28 19:21:41.000000 parallelism-0.0.2/parallelism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 19:21:40.000000 parallelism-0.0.2/parallelism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-28 19:21:40.000000 parallelism-0.0.2/parallelism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-28 19:21:41.084377 parallelism-0.0.2/setup.cfg
```

### Comparing `parallelism-0.0.1/.gitignore` & `parallelism-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/LICENSE` & `parallelism-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/PKG-INFO` & `parallelism-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.0.1
+Version: 0.0.2
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.0.1/parallelism/api_reference.py` & `parallelism-0.0.2/parallelism/api_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,14 @@
     from typing import Any, Callable, Dict, Tuple, Type, Union
 
     from parallelism.core.scheduler_result import SchedulerResult
 
 __all__ = ('scheduled_task', 'task_scheduler')
 
 
-Union[List[ScheduledTask], Set[ScheduledTask], Tuple[ScheduledTask, ...]]
-
-
 def scheduled_task(
     executor: Type[Union[Process, Thread]],
     name: str,
     target: Callable[..., Any],
     args: Tuple[Any, ...] = None,
     kwargs: Dict[str, Any] = None,
     *,
```

### Comparing `parallelism-0.0.1/parallelism/core/executors/process_executor.py` & `parallelism-0.0.2/parallelism/core/executors/process_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/executors/thread_executor.py` & `parallelism-0.0.2/parallelism/core/executors/thread_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/handlers/dependency_handler.py` & `parallelism-0.0.2/parallelism/core/handlers/dependency_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/handlers/function_handler.py` & `parallelism-0.0.2/parallelism/core/handlers/function_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/handlers/parameters_handler.py` & `parallelism-0.0.2/parallelism/core/handlers/parameters_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/handlers/shared_memory_handler.py` & `parallelism-0.0.2/parallelism/core/handlers/shared_memory_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/return_value.py` & `parallelism-0.0.2/parallelism/core/return_value.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/scheduled_task.py` & `parallelism-0.0.2/parallelism/core/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism/core/task_scheduler.py` & `parallelism-0.0.2/parallelism/core/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/parallelism.egg-info/PKG-INFO` & `parallelism-0.0.2/parallelism.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.0.1
+Version: 0.0.2
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.0.1/parallelism.egg-info/SOURCES.txt` & `parallelism-0.0.2/parallelism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallelism-0.0.1/pyproject.toml` & `parallelism-0.0.2/pyproject.toml`

 * *Files identical despite different names*

