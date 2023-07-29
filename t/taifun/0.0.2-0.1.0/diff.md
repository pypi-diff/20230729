# Comparing `tmp/taifun-0.0.2.tar.gz` & `tmp/taifun-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taifun-0.0.2.tar", max compression
+gzip compressed data, was "taifun-0.1.0.tar", max compression
```

## Comparing `taifun-0.0.2.tar` & `taifun-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3843 2023-07-28 19:05:16.682037 taifun-0.0.2/README.md
--rw-r--r--   0        0        0      630 2023-07-28 19:05:31.022106 taifun-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-28 19:05:16.682037 taifun-0.0.2/taifun/__init__.py
--rw-r--r--   0        0        0      458 2023-07-28 19:05:16.682037 taifun-0.0.2/taifun/openai_api.py
--rw-r--r--   0        0        0     3611 2023-07-28 19:05:16.682037 taifun-0.0.2/taifun/runner.py
--rw-r--r--   0        0        0     3034 2023-07-28 19:05:16.682037 taifun-0.0.2/taifun/taifun.py
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 taifun-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5835 2023-07-29 20:07:46.713957 taifun-0.1.0/README.md
+-rw-r--r--   0        0        0      629 2023-07-29 20:07:46.713957 taifun-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-29 20:07:46.713957 taifun-0.1.0/taifun/__init__.py
+-rw-r--r--   0        0        0      458 2023-07-29 20:07:46.713957 taifun-0.1.0/taifun/openai_api.py
+-rw-r--r--   0        0        0     3611 2023-07-29 20:07:46.713957 taifun-0.1.0/taifun/runner.py
+-rw-r--r--   0        0        0     3455 2023-07-29 20:07:46.713957 taifun-0.1.0/taifun/taifun.py
+-rw-r--r--   0        0        0     6399 1970-01-01 00:00:00.000000 taifun-0.1.0/PKG-INFO
```

### Comparing `taifun-0.0.2/README.md` & `taifun-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,29 +5,120 @@
 It inspects the function's docstring and parameters to create functions for OpenAI's API.
 
 Then takes a task and loops through the conversational flow until the task is complete.
 
 
 ## Usage
 
-### Just functions to pass to OpenAI
+Initialize a Taifun instance and decorate your functions with `@taifun.fn()`
+
+```python
+
+taifun = Taifun()
+
+@taifun.fn()
+def weather_forcast(location: str) -> str:
+    """
+    Get the weather forcast for a given location
+
+    Parameters
+    ----------
+    location: str
+        the user's location like a Ciry and State, e.g. San Francisco, CA
+
+    """
+
+    return f"The weather in {location} is rainy"
+
+```
+
+Then you can use the `functions_as_dict` method to get a dict that can be passed to OpenAI's functions field
+
+```python
+functions = taifun.functions_as_dict()
+```
+
+Then you can use the `handle_function_call` method to handle a function call from OpenAI's API
+
+
+`functions` is a dict that can be passed to OpenAI's functions field
+
+```json
+[
+ {
+  "name": "weather_forcast",
+  "description": "Get the weather forcast for a given location",
+  "parameters": {
+   "properties": {
+    "location": {
+     "description": "the user's location like a Ciry and State, e.g. San Francisco, CA",
+     "title": "Location",
+     "type": "string"
+    }
+   },
+   "required": [
+    "location"
+   ],
+   "title": "FunctionParameters",
+   "type": "object"
+  }
+ }
+]
+```
+
+Pass functions to the `functions` field of OpenAI's API
+
+```python
+
+messages = [...]
+result = openai.ChatCompletion.create(
+    model="gpt-4",
+    messages=messages,
+    functions=functions,
+    function_call="auto",
+)
+```
+
+If the response from OpenAI's API has a function call, you can handle it with `handle_function_call`
+
+```python
+function_call = result["choices"][0]["message"].get("function_call")
+
+if function_call is not None:
+    # handle the function call
+    function_response = taifun.handle_function_call(function_call)
+    # return the function response
+    messages.append(
+        {
+            "role": "function",
+            "name": function_call["name"],
+            "content": function_response,
+        }
+    )
+    # reply
+```
+
+
+
+### Demo with functions to pass to OpenAI
 
 ```python
 
 taifun = Taifun()
 
 
 @taifun.fn()
 def weather_forcast(location: str) -> str:
     """
     Get the weather forcast for a given location
 
     Parameters
     ----------
-    location (str): the location to get the weather forcast for
+    location: str
+        the location to get the weather forcast for
 
     """
 
     # random weather
     weather = random.choice(["sunny", "rainy", "cloudy", "snowy"])
 
     return f"The weather in {location} is {weather}"
@@ -78,14 +169,16 @@
         function_call="auto",
     )
     response_message2 = result2["choices"][0]["message"]
     print(f"assistant: {response_message2['content']}")
 
 ```
 
+### A full example including the TaifunConversationRunner
+
 ```python
 
 taifun = Taifun()
 
 
 @taifun.fn()
 def get_location() -> str:
@@ -102,15 +195,16 @@
 @taifun.fn()
 def get_lang_lat(location: str) -> dict:
     """
     Get the latitude and longitude of a location
 
     Parameters
     ----------
-    location (str): the user's location like a Ciry and State, e.g. San Francisco, CA
+    location: str 
+        the user's location like a Ciry and State, e.g. San Francisco, CA
 
     """
 
     response = httpx.get(
         f"https://nominatim.openstreetmap.org/search/{urlparse.quote(location)}",
         params={
             "format": "json",
@@ -135,15 +229,16 @@
 
 @taifun.fn()
 def get_current_weather(coordinates: Coordinates):
     """Get the current weather in a given longitude and latitude
 
     Parameters
     ----------
-    coordinates (Coordinates): the latitude and longitude of a location
+    coordinates: Coordinates
+        the latitude and longitude of a location
 
     Returns:
         dict: a dictionary of the current weather
 
     """
 
     response = httpx.get(
```

### Comparing `taifun-0.0.2/pyproject.toml` & `taifun-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taifun"
-version = "0.0.2"
+version = "0.1.0"
 description = "Function mapper for Open AI Chat"
 authors = ["Max Fröhlich <maxbruchmann@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0"
@@ -24,8 +24,8 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
```

### Comparing `taifun-0.0.2/taifun/runner.py` & `taifun-0.1.0/taifun/runner.py`

 * *Files identical despite different names*

### Comparing `taifun-0.0.2/taifun/taifun.py` & `taifun-0.1.0/taifun/taifun.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 
 
 class FunctionCallDict(TypedDict):
     name: str
     arguments: str
 
 
+class MissingDescriptionError(Exception):
+    def __init__(self, function_name: str, param_name: str):
+        self.function_name = function_name
+        self.param_name = param_name
+
+    def __str__(self):
+        return f"Missing description for parameter {self.param_name} in function {self.function_name}"
+
+
 class Taifun:
     def __init__(self):
         self.functions: Dict[str, Tuple[Function, Callable, BaseModel]] = {}
 
     def fn(self: "Taifun") -> Any:
         def inner(func):
             sig: inspect.Signature = inspect.signature(func)
@@ -33,15 +42,17 @@
                 if param.name == "self":
                     continue
                 if param.name == "return":
                     continue
                 if param.name == "return_type":
                     continue
 
-                description = docstring_params.get(param.name, "") or ""
+                description = docstring_params.get(param.name, "")
+                if description == "":
+                    raise MissingDescriptionError(func.__name__, param.name)
 
                 param_type_default_tuples_by_name[param.name] = (
                     param.annotation,
                     Field(
                         title=None,
                         description=description,
                         default=param.default
```

### Comparing `taifun-0.0.2/PKG-INFO` & `taifun-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taifun
-Version: 0.0.2
+Version: 0.1.0
 Summary: Function mapper for Open AI Chat
 Author: Max Fröhlich
 Author-email: maxbruchmann@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (>=0.15,<0.16)
@@ -22,29 +22,120 @@
 It inspects the function's docstring and parameters to create functions for OpenAI's API.
 
 Then takes a task and loops through the conversational flow until the task is complete.
 
 
 ## Usage
 
-### Just functions to pass to OpenAI
+Initialize a Taifun instance and decorate your functions with `@taifun.fn()`
+
+```python
+
+taifun = Taifun()
+
+@taifun.fn()
+def weather_forcast(location: str) -> str:
+    """
+    Get the weather forcast for a given location
+
+    Parameters
+    ----------
+    location: str
+        the user's location like a Ciry and State, e.g. San Francisco, CA
+
+    """
+
+    return f"The weather in {location} is rainy"
+
+```
+
+Then you can use the `functions_as_dict` method to get a dict that can be passed to OpenAI's functions field
+
+```python
+functions = taifun.functions_as_dict()
+```
+
+Then you can use the `handle_function_call` method to handle a function call from OpenAI's API
+
+
+`functions` is a dict that can be passed to OpenAI's functions field
+
+```json
+[
+ {
+  "name": "weather_forcast",
+  "description": "Get the weather forcast for a given location",
+  "parameters": {
+   "properties": {
+    "location": {
+     "description": "the user's location like a Ciry and State, e.g. San Francisco, CA",
+     "title": "Location",
+     "type": "string"
+    }
+   },
+   "required": [
+    "location"
+   ],
+   "title": "FunctionParameters",
+   "type": "object"
+  }
+ }
+]
+```
+
+Pass functions to the `functions` field of OpenAI's API
+
+```python
+
+messages = [...]
+result = openai.ChatCompletion.create(
+    model="gpt-4",
+    messages=messages,
+    functions=functions,
+    function_call="auto",
+)
+```
+
+If the response from OpenAI's API has a function call, you can handle it with `handle_function_call`
+
+```python
+function_call = result["choices"][0]["message"].get("function_call")
+
+if function_call is not None:
+    # handle the function call
+    function_response = taifun.handle_function_call(function_call)
+    # return the function response
+    messages.append(
+        {
+            "role": "function",
+            "name": function_call["name"],
+            "content": function_response,
+        }
+    )
+    # reply
+```
+
+
+
+### Demo with functions to pass to OpenAI
 
 ```python
 
 taifun = Taifun()
 
 
 @taifun.fn()
 def weather_forcast(location: str) -> str:
     """
     Get the weather forcast for a given location
 
     Parameters
     ----------
-    location (str): the location to get the weather forcast for
+    location: str
+        the location to get the weather forcast for
 
     """
 
     # random weather
     weather = random.choice(["sunny", "rainy", "cloudy", "snowy"])
 
     return f"The weather in {location} is {weather}"
@@ -95,14 +186,16 @@
         function_call="auto",
     )
     response_message2 = result2["choices"][0]["message"]
     print(f"assistant: {response_message2['content']}")
 
 ```
 
+### A full example including the TaifunConversationRunner
+
 ```python
 
 taifun = Taifun()
 
 
 @taifun.fn()
 def get_location() -> str:
@@ -119,15 +212,16 @@
 @taifun.fn()
 def get_lang_lat(location: str) -> dict:
     """
     Get the latitude and longitude of a location
 
     Parameters
     ----------
-    location (str): the user's location like a Ciry and State, e.g. San Francisco, CA
+    location: str 
+        the user's location like a Ciry and State, e.g. San Francisco, CA
 
     """
 
     response = httpx.get(
         f"https://nominatim.openstreetmap.org/search/{urlparse.quote(location)}",
         params={
             "format": "json",
@@ -152,15 +246,16 @@
 
 @taifun.fn()
 def get_current_weather(coordinates: Coordinates):
     """Get the current weather in a given longitude and latitude
 
     Parameters
     ----------
-    coordinates (Coordinates): the latitude and longitude of a location
+    coordinates: Coordinates
+        the latitude and longitude of a location
 
     Returns:
         dict: a dictionary of the current weather
 
     """
 
     response = httpx.get(
```

