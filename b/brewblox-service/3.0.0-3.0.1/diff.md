# Comparing `tmp/brewblox_service-3.0.0.tar.gz` & `tmp/brewblox_service-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-3.0.0.tar", max compression
+gzip compressed data, was "brewblox_service-3.0.1.tar", max compression
```

## Comparing `brewblox_service-3.0.0.tar` & `brewblox_service-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35140 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/LICENSE.md
--rw-r--r--   0        0        0     3551 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/README.md
--rw-r--r--   0        0        0     1147 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/cors.py
--rw-r--r--   0        0        0     9617 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/http.py
--rw-r--r--   0        0        0      358 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/models.py
--rw-r--r--   0        0        0    14606 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5378 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5687 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7652 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/service.py
--rw-r--r--   0        0        0     2805 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/brewblox_service/testing.py
--rw-r--r--   0        0        0      681 2023-07-28 15:31:44.757140 brewblox_service-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 brewblox_service-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/LICENSE.md
+-rw-r--r--   0        0        0     3759 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/README.md
+-rw-r--r--   0        0        0     1147 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9701 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/http.py
+-rw-r--r--   0        0        0      362 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/models.py
+-rw-r--r--   0        0        0    14610 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5382 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5687 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7358 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/service.py
+-rw-r--r--   0        0        0     2805 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/testing.py
+-rw-r--r--   0        0        0      681 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 brewblox_service-3.0.1/PKG-INFO
```

### Comparing `brewblox_service-3.0.0/LICENSE.md` & `brewblox_service-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.0/README.md` & `brewblox_service-3.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,31 +22,39 @@
 ## [service.py](./brewblox_service/service.py)
 
 Parses commandline arguments, creates an `aiohttp` application object, and runs it.
 
 The shortest implementation is:
 
 ```python
-app = service.create_app(default_name='my_service')
+parser = service.create_parser('my_service')
+config = service.create_config(parser)
+app = service.create_app(config)
 service.run_app(app)
 ```
 
 This will get you a working web application, but it will not have any endpoints.
 
 Applications can configure their own features, and add new commandline arguments.
 
 Example:
 
 ```python
+class ExtendedConfig(models.BaseServiceConfig):
+    my_arg: str
+
 # Separately creating the parser allows adding arguments to the default set
-parser = service.create_parser(default_name='my_service')
+parser = service.create_parser('my_service')
 parser.add_argument('--my-arg')
 
+# Get a config object from the extended args
+config = service.create_config(parser, model=ExtendedConfig)
+
 # Now create the app
-app = service.create_app(parser=create_parser())
+app = service.create_app(config)
 
 async def setup():
     # Add features for this service
     # You can call async functions here
     device.setup(app)
     api.setup(app)
```

### Comparing `brewblox_service-3.0.0/brewblox_service/__init__.py` & `brewblox_service-3.0.1/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.0/brewblox_service/cors.py` & `brewblox_service-3.0.1/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.0/brewblox_service/features.py` & `brewblox_service-3.0.1/brewblox_service/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,17 @@
                         'Sentry mode activated',
                         'Is anyone there?',
                         'Could you come over here?',
                     ]))
 
     Example use:
 
-        app = service.create_app(default_name='example')
+        parser = service.create_parser('my_service')
+        config = service.create_config(parser)
+        app = service.create_app(config)
 
         async def setup():
             scheduler.setup(app)
             greeter = MyFeature(app)
 
         service.run_app(app, setup())
         # greeter.startup(app) is called now
```

### Comparing `brewblox_service-3.0.0/brewblox_service/http.py` & `brewblox_service-3.0.1/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.0/brewblox_service/mqtt.py` & `brewblox_service-3.0.1/brewblox_service/mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                  protocol: models.MqttProtocol = None,
                  host: str = None,
                  port: int = None,
                  path: str = None,
                  **kwargs):
         super().__init__(app, **kwargs)
 
-        config: models.ServiceConfig = app['config']
+        config: models.BaseServiceConfig = app['config']
         protocol = protocol or config.mqtt_protocol
         host = host or config.mqtt_host
         port = port or config.mqtt_port
         path = path or config.mqtt_path
         self.config = MQTTConfig(protocol, host, port, path)
         self.client: Client = None
```

### Comparing `brewblox_service-3.0.0/brewblox_service/repeater.py` & `brewblox_service-3.0.1/brewblox_service/repeater.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     - `run()` [repeated until shutdown]
     - `before_shutdown()`
     - `shutdown()`
     """
 
     def __init__(self, app: web.Application, autostart=True, **kwargs):
         super().__init__(app, **kwargs)
-        config: models.ServiceConfig = app['config']
+        config: models.BaseServiceConfig = app['config']
 
         self._autostart: bool = autostart
         self._task: Optional[asyncio.Task] = None
         self._debug: bool = config.debug
 
     async def _startup(self, app: web.Application):
         """
```

### Comparing `brewblox_service-3.0.0/brewblox_service/scheduler.py` & `brewblox_service-3.0.1/brewblox_service/scheduler.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.0/brewblox_service/service.py` & `brewblox_service-3.0.1/brewblox_service/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 """
 Generic startup functions for a brewblox application.
 
 Responsible for parsing user configuration, and creating top-level objects.
 This module provides the framework to which service implementations can attach their features.
 
 Example:
-    # Uses the default argument parser
-    # To add new commandline arguments, use create_parser()
-    app = service.create_app(default_name='my_service')
+    parser = service.create_parser('my_service')
+    config = service.create_config(parser)
+    app = service.create_app(config)
 
     async def setup():
-        # (Placeholder names)
-        # All features (endpoints and async handlers) must be created and added to the app here
-        # The Aiohttp Application will freeze functionality once it has been started
         feature_one.setup(app)
         feature_two.setup(app)
 
-    # Run the application
-    # This function blocks until the application is shut down
     service.run_app(app, setup())
 """
 
 import argparse
 import logging
 # The argumentparser can't fall back to the default sys.argv if sys is not imported
 import sys  # noqa
 import tempfile
-from typing import Awaitable, Optional
+from typing import Awaitable, Optional, TypeVar
 
 from aiohttp import web
 from aiohttp_pydantic import oas
 
 from brewblox_service import brewblox_logger, cors, features, models
 
 LOGGER = brewblox_logger(__name__)
@@ -97,58 +92,63 @@
                        default='brewcast/history')
     group.add_argument('--state-topic',
                        help='Eventbus topic to which volatile controller state is broadcast. [%(default)s]',
                        default='brewcast/state')
     return parser
 
 
-def create_app(
-        default_name: str = None,
-        parser: argparse.ArgumentParser = None,
-        raw_args: Optional[list[str]] = None,
-        config_cls: type[models.ServiceConfig] = models.ServiceConfig,
-) -> web.Application:
+ConfigT = TypeVar('ConfigT')
+
+
+def create_config(parser: argparse.ArgumentParser,
+                  model: type[ConfigT] = models.BaseServiceConfig,
+                  raw_args: Optional[list[str]] = None
+                  ) -> ConfigT:
     """
-    Creates and configures an Aiohttp application.
+    Parses arguments, and generates the Pydantic config object.
+    If you added arguments to the parser, you should provide
+    a matching Pydantic model that extends `models.BaseServiceConfig`
 
     Args:
-        default_name (str, optional):
-            Default value for the --name commandline argument.
-            This value is required if `parser` is not provided.
-            This value will be ignored if `parser` is provided.
-
-        parser (argparse.ArgumentParser, optional):
-            Application-specific parser.
-            If not provided, the return value of `create_parser()` will be used.
-
-        raw_args (list of str, optional):
-            Explicit commandline arguments.
-            Defaults to sys.argv[1:]
-
-        config_cls (type[models.ServiceConfig], optional):
-            The Pydantic model to load the parsed args.
-            This model should inherit from ServiceConfig.
+        parser (argparse.ArgumentParser):
+            The parser generated by `create_parser()`,
+            optionally extended by caller code.
 
-    Returns:
-        web.Application: A configured Aiohttp Application object.
-            This Application is not yet running.
+        model (type[ConfigT], optional):
+            The Pydantic model that matches `parser`.
 
-    """
-
-    if parser is None:
-        assert default_name, 'Default service name is required'
-        parser = create_parser(default_name)
+        raw_args (list[str], optional):
+            If not set, `sys.argv[1:]` will be used.
 
+    Returns:
+        ConfigT: `model` instantiated with the parsed arguments.
+    """
     args, unknown_args = parser.parse_known_args(raw_args)
     _init_logging(args)
 
     if unknown_args:
         LOGGER.error(f'Unknown arguments detected: {unknown_args}')
 
-    config: models.ServiceConfig = config_cls(**vars(args))
+    return model(**vars(args))
+
+
+def create_app(config: models.BaseServiceConfig) -> web.Application:
+    """
+    Creates and configures an Aiohttp application.
+
+    Args:
+        config (models.BaseServiceConfig):
+            Parsed configuration, generated by create_config().
+            This is inserted into the application as `app['config']`.
+
+    Returns:
+        web.Application: A configured Aiohttp Application object.
+            This Application is not yet running.
+
+    """
     app = web.Application()
     app['config'] = config
 
     app.middlewares.append(cors.cors_middleware)
     oas.setup(app, url_prefix='/api/doc', title_spec=config.name)
 
     return app
@@ -172,15 +172,15 @@
 
         listen_http (bool):
             Whether to open a port for the REST API.
             Set to False to disable all REST endpoints.
             This can be useful for services that use communication protocols
             other than REST (such as MQTT), or only have active functionality.
     """
-    config: models.ServiceConfig = app['config']
+    config: models.BaseServiceConfig = app['config']
 
     async def _factory() -> web.Application:
         if setup is not None:
             await setup
 
         prefix = '/' + config.name.lstrip('/')
         for resource in app.router.resources():
```

### Comparing `brewblox_service-3.0.0/brewblox_service/testing.py` & `brewblox_service-3.0.1/brewblox_service/testing.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.0/pyproject.toml` & `brewblox_service-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brewblox-service"
-version = "3.0.0"
+version = "3.0.1"
 description = "Scaffolding for Brewblox backend services"
 authors = ["BrewPi <development@brewpi.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.pyright]
 include = ["brewblox_service"]
```

### Comparing `brewblox_service-3.0.0/PKG-INFO` & `brewblox_service-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 3.0.0
+Version: 3.0.1
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -41,31 +41,39 @@
 ## [service.py](./brewblox_service/service.py)
 
 Parses commandline arguments, creates an `aiohttp` application object, and runs it.
 
 The shortest implementation is:
 
 ```python
-app = service.create_app(default_name='my_service')
+parser = service.create_parser('my_service')
+config = service.create_config(parser)
+app = service.create_app(config)
 service.run_app(app)
 ```
 
 This will get you a working web application, but it will not have any endpoints.
 
 Applications can configure their own features, and add new commandline arguments.
 
 Example:
 
 ```python
+class ExtendedConfig(models.BaseServiceConfig):
+    my_arg: str
+
 # Separately creating the parser allows adding arguments to the default set
-parser = service.create_parser(default_name='my_service')
+parser = service.create_parser('my_service')
 parser.add_argument('--my-arg')
 
+# Get a config object from the extended args
+config = service.create_config(parser, model=ExtendedConfig)
+
 # Now create the app
-app = service.create_app(parser=create_parser())
+app = service.create_app(config)
 
 async def setup():
     # Add features for this service
     # You can call async functions here
     device.setup(app)
     api.setup(app)
```

