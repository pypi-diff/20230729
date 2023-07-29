# Comparing `tmp/deepchecks-llm-client-0.0.4.tar.gz` & `tmp/deepchecks-llm-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchecks-llm-client-0.0.4.tar", last modified: Sun Jul 16 11:08:51 2023, max compression
+gzip compressed data, was "deepchecks-llm-client-0.1.0.tar", last modified: Sat Jul 29 19:21:51 2023, max compression
```

## Comparing `deepchecks-llm-client-0.0.4.tar` & `deepchecks-llm-client-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.661552 deepchecks-llm-client-0.0.4/
--rw-r--r--   0 shay       (501) staff       (20)       18 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.4/MANIFEST.in
--rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-16 11:08:51.661449 deepchecks-llm-client-0.0.4/PKG-INFO
--rw-r--r--   0 shay       (501) staff       (20)      142 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/README.md
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.660498 deepchecks-llm-client-0.0.4/deepchecks_llm_client/
--rw-r--r--   0 shay       (501) staff       (20)       88 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/__init__.py
--rw-r--r--   0 shay       (501) staff       (20)     3847 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/api.py
--rw-r--r--   0 shay       (501) staff       (20)     3214 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/client.py
--rw-r--r--   0 shay       (501) staff       (20)     3682 2023-07-12 19:41:58.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/openai_instrumentor.py
--rw-r--r--   0 shay       (501) staff       (20)     2887 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client/utils.py
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.661007 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/
--rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/PKG-INFO
--rw-r--r--   0 shay       (501) staff       (20)      481 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/SOURCES.txt
--rw-r--r--   0 shay       (501) staff       (20)        1 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/dependency_links.txt
--rw-r--r--   0 shay       (501) staff       (20)       13 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/requires.txt
--rw-r--r--   0 shay       (501) staff       (20)       22 2023-07-16 11:08:51.000000 deepchecks-llm-client-0.0.4/deepchecks_llm_client.egg-info/top_level.txt
-drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-16 11:08:51.661189 deepchecks-llm-client-0.0.4/examples/
--rw-r--r--   0 shay       (501) staff       (20)        0 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.0.4/examples/__init__.py
--rw-r--r--   0 shay       (501) staff       (20)     2327 2023-07-16 10:23:12.000000 deepchecks-llm-client-0.0.4/examples/usage.py
--rw-r--r--   0 shay       (501) staff       (20)       13 2023-07-16 11:07:56.000000 deepchecks-llm-client-0.0.4/requirements.txt
--rw-r--r--   0 shay       (501) staff       (20)       38 2023-07-16 11:08:51.661582 deepchecks-llm-client-0.0.4/setup.cfg
--rw-r--r--   0 shay       (501) staff       (20)     3069 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.0.4/setup.py
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-29 19:21:51.261884 deepchecks-llm-client-0.1.0/
+-rw-r--r--   0 shay       (501) staff       (20)       18 2023-07-06 11:41:39.000000 deepchecks-llm-client-0.1.0/MANIFEST.in
+-rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-29 19:21:51.261784 deepchecks-llm-client-0.1.0/PKG-INFO
+-rw-r--r--   0 shay       (501) staff       (20)      142 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.1.0/README.md
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-29 19:21:51.260825 deepchecks-llm-client-0.1.0/deepchecks_llm_client/
+-rw-r--r--   0 shay       (501) staff       (20)       88 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client/__init__.py
+-rw-r--r--   0 shay       (501) staff       (20)     5012 2023-07-29 19:17:40.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client/api.py
+-rw-r--r--   0 shay       (501) staff       (20)     4786 2023-07-29 19:17:40.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client/client.py
+-rw-r--r--   0 shay       (501) staff       (20)     1132 2023-07-29 19:17:40.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client/data_types.py
+-rw-r--r--   0 shay       (501) staff       (20)     3333 2023-07-29 19:17:40.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client/openai_instrumentor.py
+-rw-r--r--   0 shay       (501) staff       (20)     3545 2023-07-29 19:17:40.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client/utils.py
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-29 19:21:51.261349 deepchecks-llm-client-0.1.0/deepchecks_llm_client.egg-info/
+-rw-r--r--   0 shay       (501) staff       (20)      211 2023-07-29 19:21:51.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client.egg-info/PKG-INFO
+-rw-r--r--   0 shay       (501) staff       (20)      517 2023-07-29 19:21:51.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shay       (501) staff       (20)        1 2023-07-29 19:21:51.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shay       (501) staff       (20)       13 2023-07-29 19:21:51.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client.egg-info/requires.txt
+-rw-r--r--   0 shay       (501) staff       (20)       22 2023-07-29 19:21:51.000000 deepchecks-llm-client-0.1.0/deepchecks_llm_client.egg-info/top_level.txt
+drwxr-xr-x   0 shay       (501) staff       (20)        0 2023-07-29 19:21:51.261519 deepchecks-llm-client-0.1.0/examples/
+-rw-r--r--   0 shay       (501) staff       (20)        0 2023-07-04 10:59:31.000000 deepchecks-llm-client-0.1.0/examples/__init__.py
+-rw-r--r--   0 shay       (501) staff       (20)     3692 2023-07-27 10:05:03.000000 deepchecks-llm-client-0.1.0/examples/usage.py
+-rw-r--r--   0 shay       (501) staff       (20)       13 2023-07-16 12:23:15.000000 deepchecks-llm-client-0.1.0/requirements.txt
+-rw-r--r--   0 shay       (501) staff       (20)       38 2023-07-29 19:21:51.261916 deepchecks-llm-client-0.1.0/setup.cfg
+-rw-r--r--   0 shay       (501) staff       (20)     3056 2023-07-29 19:21:50.000000 deepchecks-llm-client-0.1.0/setup.py
```

### Comparing `deepchecks-llm-client-0.0.4/deepchecks_llm_client/openai_instrumentor.py` & `deepchecks-llm-client-0.1.0/deepchecks_llm_client/openai_instrumentor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,37 @@
+import functools
 import logging
 import time
-import typing as t
 
 import openai
-from deepchecks_llm_client.api import API, EnvType
+from deepchecks_llm_client.api import API
+from deepchecks_llm_client.utils import handle_exceptions, set_verbosity
 
+logging.basicConfig()
 logger = logging.getLogger(__name__)
 
+
 class OpenAIInstrumentor:
 
-    def __init__(self, api: API, app_name: str, version_name: str,env_type: EnvType):
+    def __init__(self, api: API, verbose: bool = False, log_level: int = logging.WARNING):
         self.api = api
-        self.app_name = app_name
-        self.version_name = version_name
-        self.env_type = env_type
-        self._tags = dict()
+
+        logger.setLevel(log_level)
+        set_verbosity(verbose, logger)
 
         self.openai_version = "0.0.0"
         try:
             from importlib import metadata
             self.openai_version = metadata.version('openai')
         except Exception as ex:
             pass
 
-    def set_context(self, app_name, version_name, env_type):
-        self.app_name = app_name
-        self.version_name = version_name
-        self.env_type = env_type
-
-    @property
-    def tags(self) -> t.Dict[str, t.Any]:
-        return self._tags
-
-    @tags.setter
-    def tags(self, tags: t.Dict[str, t.Any]):
-        self._tags = tags
-
     @staticmethod
     def _patched_call(original_fn, patched_fn):
+        @functools.wraps(original_fn)
         def _inner_patch(*args, **kwargs):
             return patched_fn(original_fn, *args, **kwargs)
         return _inner_patch
 
     def patcher_create(self, original_fn, *args, **kwargs):
 
         self._before_run_log_print(args, kwargs, original_fn)
@@ -62,30 +52,30 @@
         result = await original_fn(*args, **kwargs)
         time_delta = time.time() - timestamp
 
         self._after_run_actions(args, kwargs, original_fn, result, time_delta)
 
         return result
 
+    @handle_exceptions(logger)
     def _after_run_actions(self, args, kwargs, original_fn, result, time_delta):
-        logger.debug(
-            f"Finished running function: '{original_fn.__qualname__}'. result: {result}, time delta: {time_delta}")
+        logger.info("Finished running function: %s, time delta: %s", original_fn.__qualname__, time_delta)
+        logger.debug("Function Response: %s", result)
         event_dict = {
             "request": {"func_name": original_fn.__qualname__, "args": args, "kwargs": kwargs},
             "response": result.to_dict_recursive(),
             "runtime_data": {"response_time": time_delta, "openai_version": self.openai_version},
-            "user_data": self.tags
         }
-        self.api.load_openai_data(data=[event_dict], app_name=self.app_name,
-                                  version_name=self.version_name, env_type=self.env_type)
-        logger.debug(f"Reported event dictionary:\n{event_dict}")
+        self.api.load_openai_data(data=[event_dict])
+
+        logger.debug("Reported this event to deepchecks server:\n%s", event_dict)
 
     @staticmethod
     def _before_run_log_print(args, kwargs, original_fn):
-        logger.debug(f"Running the original function: '{original_fn.__qualname__}'. args:{args}; kwargs: {kwargs}")
+        logger.info("Running the original function: %s. args: %s, kwargs: %s", original_fn.__qualname__, args, kwargs)
 
     def perform_patch(self):
         try:
             openai.ChatCompletion.acreate = self._patched_call(
                 openai.ChatCompletion.acreate, self.patcher_acreate
             )
         except AttributeError:
```

### Comparing `deepchecks-llm-client-0.0.4/setup.py` & `deepchecks-llm-client-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         else:
             dependencies.append(line)
     return dependencies, dependencies_links
 
 
 # ===============================================================
 
-version = get_version_string()
+version = "0.1.0"
 install_requires, dependency_links = read_requirements_file(ROOTDIR / 'requirements.txt')
 
 
 setuptools.setup(
     name="deepchecks-llm-client",
     version=version,
     author="deepchecks",
```

