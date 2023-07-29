# Comparing `tmp/abstract_gui-0.0.50.5.tar.gz` & `tmp/abstract_gui-0.0.50.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.50.5.tar", last modified: Sat Jul 29 02:23:37 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.50.6.tar", last modified: Sat Jul 29 04:23:06 2023, max compression
```

## Comparing `abstract_gui-0.0.50.5.tar` & `abstract_gui-0.0.50.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/
--rw-r--r--   0 root         (0) root         (0)     3833 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3086 2023-07-28 00:06:19.000000 abstract_gui-0.0.50.5/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.5/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1134 2023-07-29 02:23:24.000000 abstract_gui-0.0.50.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.5/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.5/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.5/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.5/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.5/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.5/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    12005 2023-07-29 02:23:05.000000 abstract_gui-0.0.50.5/src/abstract_gui/simple_gui/gui_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 02:23:37.177201 abstract_gui-0.0.50.5/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3833 2023-07-29 02:23:37.000000 abstract_gui-0.0.50.5/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      505 2023-07-29 02:23:37.000000 abstract_gui-0.0.50.5/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-29 02:23:37.000000 abstract_gui-0.0.50.5/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-29 02:23:37.000000 abstract_gui-0.0.50.5/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-29 02:23:37.000000 abstract_gui-0.0.50.5/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/
+-rw-r--r--   0 root         (0) root         (0)     3833 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3086 2023-07-28 00:06:19.000000 abstract_gui-0.0.50.6/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.6/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1134 2023-07-29 04:22:44.000000 abstract_gui-0.0.50.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.6/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.6/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.6/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.6/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.6/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.6/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    12533 2023-07-29 04:22:32.000000 abstract_gui-0.0.50.6/src/abstract_gui/simple_gui/gui_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:23:06.784620 abstract_gui-0.0.50.6/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3833 2023-07-29 04:23:06.000000 abstract_gui-0.0.50.6/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      505 2023-07-29 04:23:06.000000 abstract_gui-0.0.50.6/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-29 04:23:06.000000 abstract_gui-0.0.50.6/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-29 04:23:06.000000 abstract_gui-0.0.50.6/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-29 04:23:06.000000 abstract_gui-0.0.50.6/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.50.5/PKG-INFO` & `abstract_gui-0.0.50.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.50.5
+Version: 0.0.50.6
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.50.5/README.md` & `abstract_gui-0.0.50.6/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.5/setup.py` & `abstract_gui-0.0.50.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.50.5',
+    version='0.0.50.6',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.50.5/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.50.6/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.5/src/abstract_gui/main.py` & `abstract_gui-0.0.50.6/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.5/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.50.6/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.5/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.50.6/src/abstract_gui/simple_gui/gui_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,36 +194,56 @@
 
     Returns:
         any: The retrieved value or None if the key doesn't exist.
     """
     if st in js:
         return js[st]
 
-def while_basic_events(event_win: type(get_window()) = get_window(), win_name: str = create_win_name(), events: dict = {},global_values:dict=globals()):
+def while_basic_events(window, events, global_values=None):
     """
     Executes a while loop for handling basic events in a PySimpleGUI window.
 
     Args:
-        event_win (type(get_window())): The window to handle events for.
-        win_name (str): The name of the window.
+        window: The window to handle events for.
         events (dict): The dictionary of events and their corresponding function specifications.
+        global_values (dict): Optional. A dictionary of global variables to use in function calls. Defaults to None.
     """
-    while verify_window(event_win):
-        update_read(curr_win=event_win, win_name='event_win')
-        if win_closed(get_event(event_win)):
+    if global_values is None:
+        global_values = globals()
+
+    def call_nested_function_args(args):
+        if isinstance(args, dict):
+            if args.get('type') == 'get':
+                function_name = args.get('name')
+                function_args = args.get('args', {})
+                instance = args.get('instance')
+                return call_functions(function_name, function_args, instance, global_values)
+            else:
+                new_args = {}
+                for key, value in args.items():
+                    new_args[key] = call_nested_function_args(value)
+                return new_args
+        elif isinstance(args, list):
+            return [call_nested_function_args(arg) for arg in args]
+        else:
+            return args
+
+    while verify_window(window):
+        update_read(window)
+        event = get_event(window)
+        if win_closed(event):
             break
-        keys = get_keys(events)
-        for k in range(0, len(keys)):
-            key = keys[k]
-            if T_or_F_obj_eq(event=get_event(curr_win=win_name), obj=key):
-                func_specs = events[key]
-                if func_specs:
-                    args = process_args(func_specs['args'])
-                call_functions(args=args, instance=get_js_st(func_specs, 'instance'), function_name=get_js_st(func_specs, 'name'), glob=global_values)
-    close_window(event_win)
+
+        if event in events:
+            func_specs = events[event]
+            args = process_args(func_specs['args'])
+            processed_args = call_nested_function_args(args)
+            call_functions(func_specs['name'], processed_args, func_specs['instance'], global_values)
+
+    close_window(window)
 
 def while_basic(win=None):
     """
     Executes a while loop for handling basic events in a PySimpleGUI window.
 
     Args:
         win: The window to handle events for. If not provided, it uses the 'window' global object.
```

### Comparing `abstract_gui-0.0.50.5/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.50.6/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.50.5
+Version: 0.0.50.6
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

