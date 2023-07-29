# Comparing `tmp/plux-1.3.3.tar.gz` & `tmp/plux-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plux-1.3.3.tar", last modified: Fri Jul 28 17:27:10 2023, max compression
+gzip compressed data, was "plux-1.3.4.tar", last modified: Sat Jul 29 02:02:18 2023, max compression
```

## Comparing `plux-1.3.3.tar` & `plux-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 17:27:10.342421 plux-1.3.3/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11358 2023-02-17 21:14:38.000000 plux-1.3.3/LICENSE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-07-28 17:27:10.342421 plux-1.3.3/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8421 2023-05-15 20:31:40.000000 plux-1.3.3/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 17:27:10.342421 plux-1.3.3/plugin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      525 2023-07-28 17:26:50.000000 plux-1.3.3/plugin/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7213 2023-02-17 21:14:38.000000 plux-1.3.3/plugin/core.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2802 2023-02-17 21:14:38.000000 plux-1.3.3/plugin/discovery.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1778 2023-02-17 21:14:38.000000 plux-1.3.3/plugin/entrypoint.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12907 2023-07-28 17:26:43.000000 plux-1.3.3/plugin/manager.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1282 2023-07-28 17:26:43.000000 plux-1.3.3/plugin/metadata.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6904 2023-02-17 21:14:38.000000 plux-1.3.3/plugin/setuptools.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-28 17:27:10.342421 plux-1.3.3/plux.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-07-28 17:27:10.000000 plux-1.3.3/plux.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      381 2023-07-28 17:27:10.000000 plux-1.3.3/plux.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 17:27:10.000000 plux-1.3.3/plux.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      129 2023-07-28 17:27:10.000000 plux-1.3.3/plux.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-28 17:27:10.000000 plux-1.3.3/plux.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       63 2023-07-28 17:27:10.000000 plux-1.3.3/plux.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        7 2023-07-28 17:27:10.000000 plux-1.3.3/plux.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      197 2023-02-17 21:14:38.000000 plux-1.3.3/pyproject.toml
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1296 2023-07-28 17:27:10.342421 plux-1.3.3/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)       60 2023-02-17 21:14:38.000000 plux-1.3.3/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 02:02:18.499237 plux-1.3.4/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11358 2023-07-29 01:51:57.000000 plux-1.3.4/LICENSE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-07-29 02:02:18.499237 plux-1.3.4/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8421 2023-07-29 01:51:57.000000 plux-1.3.4/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 02:02:18.499237 plux-1.3.4/plugin/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      525 2023-07-29 02:02:07.000000 plux-1.3.4/plugin/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7213 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/core.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2802 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/discovery.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1778 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/entrypoint.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12564 2023-07-29 02:01:44.000000 plux-1.3.4/plugin/manager.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6904 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/setuptools.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 02:02:18.499237 plux-1.3.4/plux.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      362 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      129 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 01:52:34.000000 plux-1.3.4/plux.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       63 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        7 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      197 2023-07-29 01:51:57.000000 plux-1.3.4/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1296 2023-07-29 02:02:18.499237 plux-1.3.4/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       60 2023-07-29 01:51:57.000000 plux-1.3.4/setup.py
```

### Comparing `plux-1.3.3/LICENSE` & `plux-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plux-1.3.3/PKG-INFO` & `plux-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plux
-Version: 1.3.3
+Version: 1.3.4
 Summary: A dynamic code loading framework for building pluggable Python distributions
 Home-page: https://github.com/localstack/plux
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `plux-1.3.3/README.md` & `plux-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `plux-1.3.3/plugin/__init__.py` & `plux-1.3.4/plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     PluginType,
     plugin,
 )
 from .manager import PluginManager, PluginSpecResolver
 
 name = "plugin"
 
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 
 __all__ = [
     "FunctionPlugin",
     "Plugin",
     "PluginSpec",
     "PluginType",
     "PluginLifecycleListener",
```

### Comparing `plux-1.3.3/plugin/core.py` & `plux-1.3.4/plugin/core.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.3/plugin/discovery.py` & `plux-1.3.4/plugin/discovery.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.3/plugin/entrypoint.py` & `plux-1.3.4/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.3/plugin/manager.py` & `plux-1.3.4/plugin/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     PluginDisabled,
     PluginException,
     PluginFinder,
     PluginLifecycleListener,
     PluginSpec,
     PluginSpecResolver,
 )
-from .metadata import resolve_distribution_information
 
 LOG = logging.getLogger(__name__)
 
 P = TypeVar("P", bound=Plugin)
 
 
 def _call_safe(func: Callable, args: Tuple, exception_message: str):
@@ -111,23 +110,14 @@
 
     is_init: bool = False
     is_loaded: bool = False
 
     init_error: Exception = None
     load_error: Exception = None
 
-    @property
-    def distribution(self):
-        """
-        Uses metadata from importlib to resolve the distribution information for this plugin.
-
-        :return: the importlib.metadata.Distribution object
-        """
-        return resolve_distribution_information(self.plugin_spec)
-
 
 class PluginManager(PluginLifecycleNotifierMixin, Generic[P]):
     """
     Manages Plugins within a namespace discovered by a PluginFinder. The default mechanism is to resolve plugins from
     entry points using a StevedorePluginFinder.
 
     A Plugin that is managed by a PluginManager can be in three states:
```

### Comparing `plux-1.3.3/plugin/setuptools.py` & `plux-1.3.4/plugin/setuptools.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.3/plux.egg-info/PKG-INFO` & `plux-1.3.4/plux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plux
-Version: 1.3.3
+Version: 1.3.4
 Summary: A dynamic code loading framework for building pluggable Python distributions
 Home-page: https://github.com/localstack/plux
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `plux-1.3.3/setup.cfg` & `plux-1.3.4/setup.cfg`

 * *Files identical despite different names*

