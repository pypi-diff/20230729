# Comparing `tmp/plux-1.3.4.tar.gz` & `tmp/plux-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plux-1.3.4.tar", last modified: Sat Jul 29 02:02:18 2023, max compression
+gzip compressed data, was "plux-1.4.0.tar", last modified: Sat Jul 29 16:15:13 2023, max compression
```

## Comparing `plux-1.3.4.tar` & `plux-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 02:02:18.499237 plux-1.3.4/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11358 2023-07-29 01:51:57.000000 plux-1.3.4/LICENSE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-07-29 02:02:18.499237 plux-1.3.4/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8421 2023-07-29 01:51:57.000000 plux-1.3.4/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 02:02:18.499237 plux-1.3.4/plugin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      525 2023-07-29 02:02:07.000000 plux-1.3.4/plugin/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7213 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/core.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2802 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/discovery.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1778 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/entrypoint.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12564 2023-07-29 02:01:44.000000 plux-1.3.4/plugin/manager.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6904 2023-07-29 01:51:57.000000 plux-1.3.4/plugin/setuptools.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 02:02:18.499237 plux-1.3.4/plux.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      362 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      129 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 01:52:34.000000 plux-1.3.4/plux.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       63 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        7 2023-07-29 02:02:18.000000 plux-1.3.4/plux.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      197 2023-07-29 01:51:57.000000 plux-1.3.4/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1296 2023-07-29 02:02:18.499237 plux-1.3.4/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       60 2023-07-29 01:51:57.000000 plux-1.3.4/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 16:15:13.485162 plux-1.4.0/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11358 2023-07-29 01:51:57.000000 plux-1.4.0/LICENSE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11024 2023-07-29 16:15:13.485162 plux-1.4.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8421 2023-07-29 01:51:57.000000 plux-1.4.0/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 16:15:13.481161 plux-1.4.0/plugin/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      544 2023-07-29 16:14:39.000000 plux-1.4.0/plugin/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7054 2023-07-29 16:02:49.000000 plux-1.4.0/plugin/core.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2802 2023-07-29 01:51:57.000000 plux-1.4.0/plugin/discovery.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1778 2023-07-29 01:51:57.000000 plux-1.4.0/plugin/entrypoint.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12907 2023-07-29 16:02:42.000000 plux-1.4.0/plugin/manager.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1904 2023-07-29 16:02:42.000000 plux-1.4.0/plugin/metadata.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6904 2023-07-29 01:51:57.000000 plux-1.4.0/plugin/setuptools.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 16:15:13.481161 plux-1.4.0/plux/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      650 2023-07-29 16:07:42.000000 plux-1.4.0/plux/__init__.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 16:15:13.485162 plux-1.4.0/plux.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11024 2023-07-29 16:15:13.000000 plux-1.4.0/plux.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      398 2023-07-29 16:15:13.000000 plux-1.4.0/plux.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 16:15:13.000000 plux-1.4.0/plux.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      130 2023-07-29 16:15:13.000000 plux-1.4.0/plux.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 12:50:58.000000 plux-1.4.0/plux.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       63 2023-07-29 16:15:13.000000 plux-1.4.0/plux.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       12 2023-07-29 16:15:13.000000 plux-1.4.0/plux.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      197 2023-07-29 01:51:57.000000 plux-1.4.0/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1296 2023-07-29 16:15:13.485162 plux-1.4.0/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       60 2023-07-29 01:51:57.000000 plux-1.4.0/setup.py
```

### Comparing `plux-1.3.4/LICENSE` & `plux-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plux-1.3.4/PKG-INFO` & `plux-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: plux
-Version: 1.3.4
-Summary: A dynamic code loading framework for building pluggable Python distributions
-Home-page: https://github.com/localstack/plux
-Author: Thomas Rausch
-Author-email: thomas@localstack.cloud
-License: Apache License 2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: dev
-License-File: LICENSE
-
 Plux
 ====
 
 <p>
   <a href="https://github.com/localstack/plux/actions/workflows/build.yml"><img alt="CI badge" src="https://github.com/localstack/plux/actions/workflows/build.yml/badge.svg"></img></a>
   <a href="https://pypi.org/project/plux/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/plux?color=blue"></a>
   <a href="https://img.shields.io/pypi/l/plux.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/plux.svg"></a>
```

### Comparing `plux-1.3.4/plugin/__init__.py` & `plux-1.4.0/plugin/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     PluginType,
     plugin,
 )
 from .manager import PluginManager, PluginSpecResolver
 
 name = "plugin"
 
-__version__ = "1.3.4"
+__version__ = "1.4.0"
 
 __all__ = [
+    "__version__",
     "FunctionPlugin",
     "Plugin",
     "PluginSpec",
     "PluginType",
     "PluginLifecycleListener",
     "PluginFinder",
     "PluginManager",
```

### Comparing `plux-1.3.4/plugin/core.py` & `plux-1.4.0/plugin/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,14 @@
     particular Plugin have an informal contracts to use the same argument types when load is invoked.
     """
 
     namespace: str
     name: str
     requirements: List[str]
 
-    def is_active(self) -> bool:
-        # FIXME: remove after release (would currently break localstack-ext)
-        return self.should_load()
-
     def should_load(self) -> bool:
         return True
 
     def load(self, *args, **kwargs):
         """
         Called by a PluginLoader when it loads the Plugin.
         """
@@ -52,17 +48,17 @@
 class PluginSpec:
     """
     A PluginSpec describes a plugin through a namespace and its unique name within in that namespace, and holds the
     imported code that can instantiate the plugin (a PluginFactory). In the simplest case, the PluginFactory that can
     just be the Plugin's class.
 
     Internally a PluginSpec is essentially a wrapper around an importlib EntryPoint. An entrypoint is a tuple: (
-    "name", "module:object") inside a namespace that can be loaded. The entrypoint object of a LocalStack Plugin can
-    point to to a PluginSpec, or a Plugin that defines it's own namespace and name, in which case the PluginSpec will
-    be instantiated dynamically by, e.g., a PluginSpecResolver.
+    "name", "module:object") inside a namespace that can be loaded. The entrypoint object of a Plugin can point to a
+    PluginSpec, or a Plugin that defines its own namespace and name, in which case the PluginSpec will be instantiated
+    dynamically by, e.g., a PluginSpecResolver.
     """
 
     namespace: str
     name: str
     factory: PluginFactory
 
     def __init__(
@@ -104,14 +100,15 @@
     """
     A PluginSpecResolver finds or creates PluginSpec instances from sources, e.g., from analyzing a Plugin class.
     """
 
     def resolve(self, source: Any) -> PluginSpec:
         """
         Tries to create a PluginSpec from the given source.
+
         :param source: anything that can produce a PluginSpec (Plugin class, ...)
         :return: a PluginSpec instance
         """
         if isinstance(source, PluginSpec):
             return source
 
         if inspect.isclass(source):
```

### Comparing `plux-1.3.4/plugin/discovery.py` & `plux-1.4.0/plugin/discovery.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.4/plugin/entrypoint.py` & `plux-1.4.0/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.4/plugin/manager.py` & `plux-1.4.0/plugin/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     PluginDisabled,
     PluginException,
     PluginFinder,
     PluginLifecycleListener,
     PluginSpec,
     PluginSpecResolver,
 )
+from .metadata import resolve_distribution_information
 
 LOG = logging.getLogger(__name__)
 
 P = TypeVar("P", bound=Plugin)
 
 
 def _call_safe(func: Callable, args: Tuple, exception_message: str):
@@ -110,14 +111,23 @@
 
     is_init: bool = False
     is_loaded: bool = False
 
     init_error: Exception = None
     load_error: Exception = None
 
+    @property
+    def distribution(self):
+        """
+        Uses metadata from importlib to resolve the distribution information for this plugin.
+
+        :return: the importlib.metadata.Distribution object
+        """
+        return resolve_distribution_information(self.plugin_spec)
+
 
 class PluginManager(PluginLifecycleNotifierMixin, Generic[P]):
     """
     Manages Plugins within a namespace discovered by a PluginFinder. The default mechanism is to resolve plugins from
     entry points using a StevedorePluginFinder.
 
     A Plugin that is managed by a PluginManager can be in three states:
```

### Comparing `plux-1.3.4/plugin/setuptools.py` & `plux-1.4.0/plugin/setuptools.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.4/plux.egg-info/PKG-INFO` & `plux-1.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,238 +1,238 @@
 Metadata-Version: 2.1
 Name: plux
-Version: 1.3.4
+Version: 1.4.0
 Summary: A dynamic code loading framework for building pluggable Python distributions
 Home-page: https://github.com/localstack/plux
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 License: Apache License 2.0
+Description: Plux
+        ====
+        
+        <p>
+          <a href="https://github.com/localstack/plux/actions/workflows/build.yml"><img alt="CI badge" src="https://github.com/localstack/plux/actions/workflows/build.yml/badge.svg"></img></a>
+          <a href="https://pypi.org/project/plux/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/plux?color=blue"></a>
+          <a href="https://img.shields.io/pypi/l/plux.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/plux.svg"></a>
+          <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+        </p>
+        
+        plux is the dynamic code loading framework used in [LocalStack](https://github.com/localstack/localstack).
+        
+        
+        Overview
+        --------
+        
+        Plux builds a higher-level plugin mechanism around [Python's entry point mechanism](https://packaging.python.org/specifications/entry-points/).
+        It provides tools to load plugins from entry points at run time, and to discover entry points from plugins at build time (so you don't have to declare entry points statically in your `setup.py`).
+        
+        ### Core concepts
+        
+        * `PluginSpec`: describes a `Plugin`. Each plugin has a namespace, a unique name in that namespace, and a `PluginFactory` (something that creates `Plugin` the spec is describing.
+          In the simplest case, that can just be the Plugin's class).
+        * `Plugin`: an object that exposes a `should_load` and `load` method.
+          Note that it does not function as a domain object (it does not hold the plugins lifecycle state, like initialized, loaded, etc..., or other metadata of the Plugin)
+        * `PluginFinder`: finds plugins, either at build time (by scanning the modules using `pkgutil` and `setuptools`) or at run time (reading entrypoints of the distribution using [stevedore](https://docs.openstack.org/stevedore/latest/))
+        * `PluginManager`: manages the run time lifecycle of a Plugin, which has three states:
+          * resolved: the entrypoint pointing to the PluginSpec was imported and the `PluginSpec` instance was created
+          * init: the `PluginFactory` of the `PluginSpec` was successfully invoked
+          * loaded: the `load` method of the `Plugin` was successfully invoked
+        
+        ![architecture](https://raw.githubusercontent.com/localstack/plux/main/docs/plux-architecture.png)
+        
+        ### Loading Plugins
+        
+        At run time, a `PluginManager` uses a `PluginFinder` that in turn uses stevedore to scan the available entrypoints for things that look like a `PluginSpec`.
+        With `PluginManager.load(name: str)` or `PluginManager.load_all()`, plugins within the namespace that are discoverable in entrypoints can be loaded.
+        If an error occurs at any state of the lifecycle, the `PluginManager` informs the `PluginLifecycleListener` about it, but continues operating.
+        
+        ### Discovering entrypoints
+        
+        To build a source distribution and a wheel of your code with your plugins as entrypoints, simply run `python setup.py plugins sdist bdist_wheel`.
+        
+        How it works:
+        For discovering plugins at build time, plux provides a custom setuptools command `plugins`, invoked via `python setup.py plugins`.
+        The command uses a special `PluginFinder` that collects from the codebase anything that can be interpreted as a `PluginSpec`, and creates from it a plugin index file `plux.json`, that is placed into the `.egg-info` distribution metadata directory.
+        When a setuptools command is used to create the distribution (e.g., `python setup.py sdist/bdist_wheel/...`), plux finds the `plux.json` plugin index and extends automatically the list of entry points (collected into `.egg-info/entry_points.txt`).
+        The `plux.json` file becomes a part of the distribution, s.t., the plugins do not have to be discovered every time your distribution is installed elsewhere.
+        
+        
+        
+        Examples
+        --------
+        
+        To build something using the plugin framework, you will first want to introduce a Plugin that does something when it is loaded.
+        And then, at runtime, you need a component that uses the `PluginManager` to get those plugins.
+        
+        ### One class per plugin
+        
+        This is the way we went with `LocalstackCliPlugin`. Every plugin class (e.g., `ProCliPlugin`) is essentially a singleton.
+        This is easy, as the classes are discoverable as plugins.
+        Simply create a Plugin class with a name and namespace and it will be discovered by the build time `PluginFinder`.
+        
+        ```python
+        
+        # abstract case (not discovered at build time, missing name)
+        class CliPlugin(Plugin):
+            namespace = "my.plugins.cli"
+        
+            def load(self, cli):
+                self.attach(cli)
+        
+            def attach(self, cli):
+                raise NotImplementedError
+        
+        # discovered at build time (has a namespace, name, and is a Plugin)
+        class MyCliPlugin(CliPlugin):
+            name = "my"
+        
+            def attach(self, cli):
+                # ... attach commands to cli object
+        
+        ```
+        
+        now we need a `PluginManager` (which has a generic type) to load the plugins for us:
+        
+        ```python
+        cli = # ... needs to come from somewhere
+        
+        manager: PluginManager[CliPlugin] = PluginManager("my.plugins.cli", load_args=(cli,))
+        
+        plugins: List[CliPlugin] = manager.load_all()
+        
+        # todo: do stuff with the plugins, if you want/need
+        #  in this example, we simply use the plugin mechanism to run a one-shot function (attach) on a load argument
+        
+        ```
+        
+        ### Re-usable plugins
+        
+        When you have lots of plugins that are structured in a similar way, we may not want to create a separate Plugin class
+        for each plugin. Instead we want to use the same `Plugin` class to do the same thing, but use several instances of it.
+        The `PluginFactory`, and the fact that `PluginSpec` instances defined at module level are discoverable (inpired
+        by [pluggy](https://github.com/pytest-dev/pluggy)), can be used to achieve that.
+        
+        ```python
+        
+        class ServicePlugin(Plugin):
+        
+            def __init__(self, service_name):
+                self.service_name = service_name
+                self.service = None
+        
+            def should_load(self):
+                return self.service_name in config.SERVICES
+        
+            def load(self):
+                module = importlib.import_module("localstack.services.%s" % self.service_name)
+                # suppose we define a convention that each service module has a Service class, like moto's `Backend`
+                self.service = module.Service()
+        
+        def service_plugin_factory(name) -> PluginFactory:
+            def create():
+                return ServicePlugin(name)
+        
+            return create
+        
+        # discoverable
+        s3 = PluginSpec("localstack.plugins.services", "s3", service_plugin_factory("s3"))
+        
+        # discoverable
+        dynamodb = PluginSpec("localstack.plugins.services", "dynamodb", service_plugin_factory("dynamodb"))
+        
+        # ... could be simplified with convenience framework code, but the principle will stay the same
+        
+        ```
+        
+        Then we could use the `PluginManager` to build a Supervisor
+        
+        ```python
+        
+        class Supervisor:
+            manager: PluginManager[ServicePlugin]
+        
+            def start(self, service_name):
+                plugin = manager.load(service_name)
+                service = plugin.service
+                service.start()
+        
+        ```
+        
+        ### Functions as plugins
+        
+        with the `@plugin` decorator, you can expose functions as plugins. They will be wrapped by the framework
+        into `FunctionPlugin` instances, which satisfy both the contract of a Plugin, and that of the function.
+        
+        ```python
+        from plugin import plugin
+        
+        
+        @plugin(namespace="localstack.configurators")
+        def configure_logging(runtime):
+            logging.basicConfig(level=runtime.config.loglevel)
+        
+            
+        @plugin(namespace="localstack.configurators")
+        def configure_somethingelse(runtime):
+            # do other stuff with the runtime object
+            pass
+        ```
+        
+        With a PluginManager via `load_all`, you receive the `FunctionPlugin` instances, that you can call like the functions
+        
+        ```python
+        
+        runtime = LocalstackRuntime()
+        
+        for configurator in PluginManager("localstack.configurators").load_all():
+            configurator(runtime)
+        ```
+        
+        Configuring your distribution
+        -----------------------------
+        
+        If you are building a python distribution that exposes plugins discovered by plux, you need to configure your projects build system so other dependencies creates the `entry_points.txt` file when installing your distribution.
+        
+        For a [`pyproject.toml`](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) template this involves adding the `build-system` section:
+        
+        ```toml
+        [build-system]
+        requires = ['setuptools', 'wheel', 'plux>=1.3.1']
+        build-backend = "setuptools.build_meta"
+        
+        # ...
+        ```
+        
+        Install
+        -------
+        
+            pip install plux
+        
+        Develop
+        -------
+        
+        Create the virtual environment, install dependencies, and run tests
+        
+            make venv
+            make test
+        
+        Run the code formatter
+        
+            make format
+        
+        Upload the pypi package using twine
+        
+            make upload
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
-License-File: LICENSE
-
-Plux
-====
-
-<p>
-  <a href="https://github.com/localstack/plux/actions/workflows/build.yml"><img alt="CI badge" src="https://github.com/localstack/plux/actions/workflows/build.yml/badge.svg"></img></a>
-  <a href="https://pypi.org/project/plux/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/plux?color=blue"></a>
-  <a href="https://img.shields.io/pypi/l/plux.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/plux.svg"></a>
-  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-</p>
-
-plux is the dynamic code loading framework used in [LocalStack](https://github.com/localstack/localstack).
-
-
-Overview
---------
-
-Plux builds a higher-level plugin mechanism around [Python's entry point mechanism](https://packaging.python.org/specifications/entry-points/).
-It provides tools to load plugins from entry points at run time, and to discover entry points from plugins at build time (so you don't have to declare entry points statically in your `setup.py`).
-
-### Core concepts
-
-* `PluginSpec`: describes a `Plugin`. Each plugin has a namespace, a unique name in that namespace, and a `PluginFactory` (something that creates `Plugin` the spec is describing.
-  In the simplest case, that can just be the Plugin's class).
-* `Plugin`: an object that exposes a `should_load` and `load` method.
-  Note that it does not function as a domain object (it does not hold the plugins lifecycle state, like initialized, loaded, etc..., or other metadata of the Plugin)
-* `PluginFinder`: finds plugins, either at build time (by scanning the modules using `pkgutil` and `setuptools`) or at run time (reading entrypoints of the distribution using [stevedore](https://docs.openstack.org/stevedore/latest/))
-* `PluginManager`: manages the run time lifecycle of a Plugin, which has three states:
-  * resolved: the entrypoint pointing to the PluginSpec was imported and the `PluginSpec` instance was created
-  * init: the `PluginFactory` of the `PluginSpec` was successfully invoked
-  * loaded: the `load` method of the `Plugin` was successfully invoked
-
-![architecture](https://raw.githubusercontent.com/localstack/plux/main/docs/plux-architecture.png)
-
-### Loading Plugins
-
-At run time, a `PluginManager` uses a `PluginFinder` that in turn uses stevedore to scan the available entrypoints for things that look like a `PluginSpec`.
-With `PluginManager.load(name: str)` or `PluginManager.load_all()`, plugins within the namespace that are discoverable in entrypoints can be loaded.
-If an error occurs at any state of the lifecycle, the `PluginManager` informs the `PluginLifecycleListener` about it, but continues operating.
-
-### Discovering entrypoints
-
-To build a source distribution and a wheel of your code with your plugins as entrypoints, simply run `python setup.py plugins sdist bdist_wheel`.
-
-How it works:
-For discovering plugins at build time, plux provides a custom setuptools command `plugins`, invoked via `python setup.py plugins`.
-The command uses a special `PluginFinder` that collects from the codebase anything that can be interpreted as a `PluginSpec`, and creates from it a plugin index file `plux.json`, that is placed into the `.egg-info` distribution metadata directory.
-When a setuptools command is used to create the distribution (e.g., `python setup.py sdist/bdist_wheel/...`), plux finds the `plux.json` plugin index and extends automatically the list of entry points (collected into `.egg-info/entry_points.txt`).
-The `plux.json` file becomes a part of the distribution, s.t., the plugins do not have to be discovered every time your distribution is installed elsewhere.
-
-
-
-Examples
---------
-
-To build something using the plugin framework, you will first want to introduce a Plugin that does something when it is loaded.
-And then, at runtime, you need a component that uses the `PluginManager` to get those plugins.
-
-### One class per plugin
-
-This is the way we went with `LocalstackCliPlugin`. Every plugin class (e.g., `ProCliPlugin`) is essentially a singleton.
-This is easy, as the classes are discoverable as plugins.
-Simply create a Plugin class with a name and namespace and it will be discovered by the build time `PluginFinder`.
-
-```python
-
-# abstract case (not discovered at build time, missing name)
-class CliPlugin(Plugin):
-    namespace = "my.plugins.cli"
-
-    def load(self, cli):
-        self.attach(cli)
-
-    def attach(self, cli):
-        raise NotImplementedError
-
-# discovered at build time (has a namespace, name, and is a Plugin)
-class MyCliPlugin(CliPlugin):
-    name = "my"
-
-    def attach(self, cli):
-        # ... attach commands to cli object
-
-```
-
-now we need a `PluginManager` (which has a generic type) to load the plugins for us:
-
-```python
-cli = # ... needs to come from somewhere
-
-manager: PluginManager[CliPlugin] = PluginManager("my.plugins.cli", load_args=(cli,))
-
-plugins: List[CliPlugin] = manager.load_all()
-
-# todo: do stuff with the plugins, if you want/need
-#  in this example, we simply use the plugin mechanism to run a one-shot function (attach) on a load argument
-
-```
-
-### Re-usable plugins
-
-When you have lots of plugins that are structured in a similar way, we may not want to create a separate Plugin class
-for each plugin. Instead we want to use the same `Plugin` class to do the same thing, but use several instances of it.
-The `PluginFactory`, and the fact that `PluginSpec` instances defined at module level are discoverable (inpired
-by [pluggy](https://github.com/pytest-dev/pluggy)), can be used to achieve that.
-
-```python
-
-class ServicePlugin(Plugin):
-
-    def __init__(self, service_name):
-        self.service_name = service_name
-        self.service = None
-
-    def should_load(self):
-        return self.service_name in config.SERVICES
-
-    def load(self):
-        module = importlib.import_module("localstack.services.%s" % self.service_name)
-        # suppose we define a convention that each service module has a Service class, like moto's `Backend`
-        self.service = module.Service()
-
-def service_plugin_factory(name) -> PluginFactory:
-    def create():
-        return ServicePlugin(name)
-
-    return create
-
-# discoverable
-s3 = PluginSpec("localstack.plugins.services", "s3", service_plugin_factory("s3"))
-
-# discoverable
-dynamodb = PluginSpec("localstack.plugins.services", "dynamodb", service_plugin_factory("dynamodb"))
-
-# ... could be simplified with convenience framework code, but the principle will stay the same
-
-```
-
-Then we could use the `PluginManager` to build a Supervisor
-
-```python
-
-class Supervisor:
-    manager: PluginManager[ServicePlugin]
-
-    def start(self, service_name):
-        plugin = manager.load(service_name)
-        service = plugin.service
-        service.start()
-
-```
-
-### Functions as plugins
-
-with the `@plugin` decorator, you can expose functions as plugins. They will be wrapped by the framework
-into `FunctionPlugin` instances, which satisfy both the contract of a Plugin, and that of the function.
-
-```python
-from plugin import plugin
-
-
-@plugin(namespace="localstack.configurators")
-def configure_logging(runtime):
-    logging.basicConfig(level=runtime.config.loglevel)
-
-    
-@plugin(namespace="localstack.configurators")
-def configure_somethingelse(runtime):
-    # do other stuff with the runtime object
-    pass
-```
-
-With a PluginManager via `load_all`, you receive the `FunctionPlugin` instances, that you can call like the functions
-
-```python
-
-runtime = LocalstackRuntime()
-
-for configurator in PluginManager("localstack.configurators").load_all():
-    configurator(runtime)
-```
-
-Configuring your distribution
------------------------------
-
-If you are building a python distribution that exposes plugins discovered by plux, you need to configure your projects build system so other dependencies creates the `entry_points.txt` file when installing your distribution.
-
-For a [`pyproject.toml`](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) template this involves adding the `build-system` section:
-
-```toml
-[build-system]
-requires = ['setuptools', 'wheel', 'plux>=1.3.1']
-build-backend = "setuptools.build_meta"
-
-# ...
-```
-
-Install
--------
-
-    pip install plux
-
-Develop
--------
-
-Create the virtual environment, install dependencies, and run tests
-
-    make venv
-    make test
-
-Run the code formatter
-
-    make format
-
-Upload the pypi package using twine
-
-    make upload
```

### Comparing `plux-1.3.4/setup.cfg` & `plux-1.4.0/setup.cfg`

 * *Files identical despite different names*

