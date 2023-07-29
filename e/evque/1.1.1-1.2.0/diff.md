# Comparing `tmp/evque-1.1.1.tar.gz` & `tmp/evque-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evque-1.1.1.tar", last modified: Sat Jul 29 00:06:29 2023, max compression
+gzip compressed data, was "evque-1.2.0.tar", last modified: Sat Jul 29 14:37:23 2023, max compression
```

## Comparing `evque-1.1.1.tar` & `evque-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:06:29.870113 evque-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-29 00:06:18.000000 evque-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-29 00:06:29.870113 evque-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-29 00:06:18.000000 evque-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:06:29.870113 evque-1.1.1/evque/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-29 00:06:18.000000 evque-1.1.1/evque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-29 00:06:18.000000 evque-1.1.1/evque/evque.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:06:29.870113 evque-1.1.1/evque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-29 00:06:29.000000 evque-1.1.1/evque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-29 00:06:29.000000 evque-1.1.1/evque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:06:29.000000 evque-1.1.1/evque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 00:06:29.000000 evque-1.1.1/evque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:06:29.870113 evque-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-29 00:06:18.000000 evque-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:37:23.453864 evque-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-29 14:37:08.000000 evque-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 14:37:23.453864 evque-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-29 14:37:08.000000 evque-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:37:23.453864 evque-1.2.0/evque/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-29 14:37:08.000000 evque-1.2.0/evque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-29 14:37:08.000000 evque-1.2.0/evque/evque.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:37:23.453864 evque-1.2.0/evque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:37:23.453864 evque-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-29 14:37:08.000000 evque-1.2.0/setup.py
```

### Comparing `evque-1.1.1/LICENSE.txt` & `evque-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evque-1.1.1/PKG-INFO` & `evque-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evque
-Version: 1.1.1
+Version: 1.2.0
 Summary: A simple event queue library with support for topics.
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,34 +31,30 @@
 pip install evque
 ```
 
 ## Features
 
 - **Event Queue:** Manage events and their delivery times in a priority queue.
 - **Topic Support:** Subscribe and publish events to different topics.
-- **Relative Event Publishing:** Publish events with a relative delay from the current time.
 - **Singleton Instance:** Share a single event queue instance across modules in your application.
 
 ## Usage
 
 ```python
-from evque import subscribe, publish, publish_relative, run_until, empty, increase_clock, reset_clock, now
+from evque import subscribe, publish, run_until, empty, increase_clock, reset_clock, now
 
 # Subscribe to a topic
 def event_handler(arg):
     print(f"Event received with argument: {arg}")
 
 subscribe('topic1', event_handler)
 
 # Publish an event to be delivered at time 10
 publish('topic1', 10, "Hello, World!")
 
-# Publish an event with a relative delay of 5 units
-publish_relative('topic1', 5, "Relative Event!")
-
 # Run events until time 15
 run_until(15)
 
 # Check if there are undelivered events in the queue
 if empty():
     print("No undelivered events in the queue.")
 ```
```

### Comparing `evque-1.1.1/README.md` & `evque-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,34 +13,30 @@
 pip install evque
 ```
 
 ## Features
 
 - **Event Queue:** Manage events and their delivery times in a priority queue.
 - **Topic Support:** Subscribe and publish events to different topics.
-- **Relative Event Publishing:** Publish events with a relative delay from the current time.
 - **Singleton Instance:** Share a single event queue instance across modules in your application.
 
 ## Usage
 
 ```python
-from evque import subscribe, publish, publish_relative, run_until, empty, increase_clock, reset_clock, now
+from evque import subscribe, publish, run_until, empty, increase_clock, reset_clock, now
 
 # Subscribe to a topic
 def event_handler(arg):
     print(f"Event received with argument: {arg}")
 
 subscribe('topic1', event_handler)
 
 # Publish an event to be delivered at time 10
 publish('topic1', 10, "Hello, World!")
 
-# Publish an event with a relative delay of 5 units
-publish_relative('topic1', 5, "Relative Event!")
-
 # Run events until time 15
 run_until(15)
 
 # Check if there are undelivered events in the queue
 if empty():
     print("No undelivered events in the queue.")
 ```
```

### Comparing `evque-1.1.1/evque/evque.py` & `evque-1.2.0/evque/evque.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 
     unsubscribe(topic: str, handler: Callable):
         Unsubscribe a handler function from a topic.
 
     publish(topic: str, delivery_time: int, *args, **kwargs):
         Publish an event to a topic with a specific delivery time.
 
-    publish_relative(topic: str, delay: int, *args, **kwargs):
-        Publish an event to a topic with a relative delay from the current time.
-
     run_until(target_time: int):
         Process events in the queue until the target time is reached.
 
     empty() -> bool:
         Check if there are any undelivered events in the queue.
 
     Notes
@@ -123,38 +120,14 @@
         """
         if topic not in self._topics:
             raise KeyError(f"Topic '{topic}' does not exist.")
 
         event = (delivery_time, topic, args, kwargs)
         heapq.heappush(self._events, event)
 
-    def publish_relative(self, topic: str, delay: int, *args, **kwargs):
-        """
-        Publish an event to a topic with a relative delay from the current time.
-
-        Parameters
-        ----------
-        topic : str
-            The topic to publish the event to.
-        delay : int
-            The delay (in time units) from the current time to publish the event.
-        *args : list
-            Variable-length argument list to be passed to the event handlers.
-        **kwargs : dict
-            Arbitrary keyword arguments to be passed to the event handlers.
-
-        Raises
-        ------
-        KeyError
-            If the specified topic does not exist.
-        """
-        current_time = self.now()
-        delivery_time = current_time + delay
-        self.publish(topic, delivery_time, *args, **kwargs)
-
     def run_until(self, target_time: int):
         """
         Process events in the queue until the target time is reached.
 
         Parameters
         ----------
         target_time : int
```

### Comparing `evque-1.1.1/evque.egg-info/PKG-INFO` & `evque-1.2.0/evque.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evque
-Version: 1.1.1
+Version: 1.2.0
 Summary: A simple event queue library with support for topics.
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,34 +31,30 @@
 pip install evque
 ```
 
 ## Features
 
 - **Event Queue:** Manage events and their delivery times in a priority queue.
 - **Topic Support:** Subscribe and publish events to different topics.
-- **Relative Event Publishing:** Publish events with a relative delay from the current time.
 - **Singleton Instance:** Share a single event queue instance across modules in your application.
 
 ## Usage
 
 ```python
-from evque import subscribe, publish, publish_relative, run_until, empty, increase_clock, reset_clock, now
+from evque import subscribe, publish, run_until, empty, increase_clock, reset_clock, now
 
 # Subscribe to a topic
 def event_handler(arg):
     print(f"Event received with argument: {arg}")
 
 subscribe('topic1', event_handler)
 
 # Publish an event to be delivered at time 10
 publish('topic1', 10, "Hello, World!")
 
-# Publish an event with a relative delay of 5 units
-publish_relative('topic1', 5, "Relative Event!")
-
 # Run events until time 15
 run_until(15)
 
 # Check if there are undelivered events in the queue
 if empty():
     print("No undelivered events in the queue.")
 ```
```

### Comparing `evque-1.1.1/setup.py` & `evque-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='evque',
-    version='1.1.1',
+    version='1.2.0',
     description='A simple event queue library with support for topics.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ahmad Siavashi',
     author_email='siavashi@aut.ac.ir',
     packages=find_packages(),
     install_requires=[],
```

