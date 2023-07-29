# Comparing `tmp/brewblox_service-3.0.1.tar.gz` & `tmp/brewblox_service-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brewblox_service-3.0.1.tar", max compression
+gzip compressed data, was "brewblox_service-3.0.2.tar", max compression
```

## Comparing `brewblox_service-3.0.1.tar` & `brewblox_service-3.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35140 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/LICENSE.md
--rw-r--r--   0        0        0     3759 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/README.md
--rw-r--r--   0        0        0     1147 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/__init__.py
--rw-r--r--   0        0        0     1503 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/cors.py
--rw-r--r--   0        0        0     9701 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/features.py
--rw-r--r--   0        0        0     1153 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/http.py
--rw-r--r--   0        0        0      362 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/models.py
--rw-r--r--   0        0        0    14610 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/mqtt.py
--rw-r--r--   0        0        0     5382 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/repeater.py
--rw-r--r--   0        0        0     5687 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/scheduler.py
--rw-r--r--   0        0        0     7358 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/service.py
--rw-r--r--   0        0        0     2805 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/brewblox_service/testing.py
--rw-r--r--   0        0        0      681 2023-07-29 10:44:18.642517 brewblox_service-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 brewblox_service-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35140 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/LICENSE.md
+-rw-r--r--   0        0        0     3759 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/README.md
+-rw-r--r--   0        0        0     1147 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/__init__.py
+-rw-r--r--   0        0        0     1503 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/cors.py
+-rw-r--r--   0        0        0     9701 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/features.py
+-rw-r--r--   0        0        0     1153 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/http.py
+-rw-r--r--   0        0        0      362 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/models.py
+-rw-r--r--   0        0        0    14239 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/mqtt.py
+-rw-r--r--   0        0        0     5382 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/repeater.py
+-rw-r--r--   0        0        0     5687 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/scheduler.py
+-rw-r--r--   0        0        0     7358 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/service.py
+-rw-r--r--   0        0        0     2805 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/brewblox_service/testing.py
+-rw-r--r--   0        0        0      681 2023-07-29 11:06:38.889748 brewblox_service-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 brewblox_service-3.0.2/PKG-INFO
```

### Comparing `brewblox_service-3.0.1/LICENSE.md` & `brewblox_service-3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/README.md` & `brewblox_service-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/__init__.py` & `brewblox_service-3.0.2/brewblox_service/__init__.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/cors.py` & `brewblox_service-3.0.2/brewblox_service/cors.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/features.py` & `brewblox_service-3.0.2/brewblox_service/features.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/http.py` & `brewblox_service-3.0.2/brewblox_service/http.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/mqtt.py` & `brewblox_service-3.0.2/brewblox_service/mqtt.py`

 * *Files 6% similar despite different names*

```diff
@@ -291,28 +291,14 @@
     Args:
         app (web.Application):
             The Aiohttp Application object.
     """
     return features.get(app, EventHandler)
 
 
-def handler(app: web.Application) -> EventHandler:  # pragma: no cover
-    """
-    Deprecated: use fget() instead
-
-    Get registered EventHandler.
-    Requires setup(app) to have been called first.
-
-    Args:
-        app (web.Application):
-            The Aiohttp Application object.
-    """
-    return features.get(app, EventHandler)
-
-
 def set_client_will(app: web.Application,
                     topic: str,
                     message: PayloadType = None,
                     **kwargs):
     """
     Set MQTT Last Will and Testament for client.
     Requires setup(app) to have been called first.
@@ -324,15 +310,15 @@
 
         topic (str):
             The MQTT message topic. Cannot include wildcards.
 
         message (str, bytes, None):
             The payload that will be published by the broker on our behalf after disconnecting.
     """
-    handler(app).set_client_will(topic, message, **kwargs)
+    fget(app).set_client_will(topic, message, **kwargs)
 
 
 async def publish(app: web.Application,
                   topic: str,
                   message: PayloadType,
                   retain=False,
                   qos=0,
@@ -363,20 +349,20 @@
             The MQTT quality-of-service flag.
             Must be 0, 1, or 2.
 
         err (bool):
             Local flag to determine error handling.
             If set to `False`, no exception is raised when the message could not be published.
     """
-    await handler(app).publish(topic,
-                               message,
-                               retain,
-                               qos,
-                               err,
-                               **kwargs)
+    await fget(app).publish(topic,
+                            message,
+                            retain,
+                            qos,
+                            err,
+                            **kwargs)
 
 
 async def subscribe(app: web.Application, topic: str):
     """
     Subscribe to event messages.
     Requires setup(app) to have been called first.
 
@@ -389,15 +375,15 @@
         app (web.Application):
             The Aiohttp Application object.
 
         topic (str):
             A filter for message topics.
             Can include the '+' and '#' wildcards.
     """
-    await handler(app).subscribe(topic)
+    await fget(app).subscribe(topic)
 
 
 async def listen(app: web.Application, topic: str, callback: ListenerCallback_):
     """
     Set a listener for event messages.
     Requires setup(app) to have been called first.
 
@@ -415,15 +401,15 @@
             Can include the '+' and '#' wildcards.
 
         callback (Callable[[str, str], Awaitable[None]]):
             The callback that will be invoked if a message is received.
             It is expected to be an async function that takes two arguments: topic and payload.
 
     """
-    await handler(app).listen(topic, callback)
+    await fget(app).listen(topic, callback)
 
 
 async def unsubscribe(app: web.Application, topic: str):
     """
     Unsubscribe to event messages.
     Requires setup(app) to have been called first.
 
@@ -433,15 +419,15 @@
     Args:
         app (web.Application):
             The Aiohttp Application object.
 
         topic (str):
             Must match the `topic` argument earlier used in `subscribe(topic)`.
     """
-    await handler(app).unsubscribe(topic)
+    await fget(app).unsubscribe(topic)
 
 
 async def unlisten(app: web.Application, topic: str, callback: ListenerCallback_):
     """
     Remove a callback for received event messages.
     Requires setup(app) to have been called first.
 
@@ -455,8 +441,8 @@
 
         topic (str):
             Must match the `topic` argument earlier used in `listen(topic, callback)`.
 
         callback (Callable[[str, str], Awaitable[None]]):
             Must match the `callback` argument earlier used in `listen(topic, callback)`.
     """
-    await handler(app).unlisten(topic, callback)
+    await fget(app).unlisten(topic, callback)
```

### Comparing `brewblox_service-3.0.1/brewblox_service/repeater.py` & `brewblox_service-3.0.2/brewblox_service/repeater.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/scheduler.py` & `brewblox_service-3.0.2/brewblox_service/scheduler.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/service.py` & `brewblox_service-3.0.2/brewblox_service/service.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/brewblox_service/testing.py` & `brewblox_service-3.0.2/brewblox_service/testing.py`

 * *Files identical despite different names*

### Comparing `brewblox_service-3.0.1/pyproject.toml` & `brewblox_service-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brewblox-service"
-version = "3.0.1"
+version = "3.0.2"
 description = "Scaffolding for Brewblox backend services"
 authors = ["BrewPi <development@brewpi.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.pyright]
 include = ["brewblox_service"]
```

### Comparing `brewblox_service-3.0.1/PKG-INFO` & `brewblox_service-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brewblox-service
-Version: 3.0.1
+Version: 3.0.2
 Summary: Scaffolding for Brewblox backend services
 License: GPL-3.0
 Author: BrewPi
 Author-email: development@brewpi.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

