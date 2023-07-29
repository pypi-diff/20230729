# Comparing `tmp/jsno-1.0.2.tar.gz` & `tmp/jsno-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsno-1.0.2.tar", last modified: Sat Jul 29 14:13:54 2023, max compression
+gzip compressed data, was "jsno-1.0.3.tar", last modified: Sat Jul 29 14:43:03 2023, max compression
```

## Comparing `jsno-1.0.2.tar` & `jsno-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.556135 jsno-1.0.2/
--rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.2/LICENSE
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:13:54.555737 jsno-1.0.2/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)     2281 2023-07-29 10:12:41.000000 jsno-1.0.2/README.md
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.550322 jsno-1.0.2/jsno/
--rw-r--r--   0 pekka      (501) staff       (20)     1405 2023-07-29 14:12:43.000000 jsno-1.0.2/jsno/__init__.py
--rw-r--r--   0 pekka      (501) staff       (20)     2280 2023-07-28 18:51:39.000000 jsno-1.0.2/jsno/abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     4438 2023-07-29 09:40:36.000000 jsno-1.0.2/jsno/jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      425 2023-07-23 10:01:17.000000 jsno-1.0.2/jsno/jsonize.py
--rw-r--r--   0 pekka      (501) staff       (20)      494 2023-07-23 10:02:00.000000 jsno-1.0.2/jsno/method.py
--rw-r--r--   0 pekka      (501) staff       (20)     5236 2023-07-29 13:29:17.000000 jsno-1.0.2/jsno/standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4079 2023-07-29 14:07:49.000000 jsno-1.0.2/jsno/unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      869 2023-07-29 09:00:26.000000 jsno-1.0.2/jsno/utils.py
--rw-r--r--   0 pekka      (501) staff       (20)     3387 2023-07-29 08:59:40.000000 jsno-1.0.2/jsno/variant.py
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.551695 jsno-1.0.2/jsno.egg-info/
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)      512 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/SOURCES.txt
--rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/dependency_links.txt
--rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/requires.txt
--rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/top_level.txt
--rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-29 14:13:01.000000 jsno-1.0.2/pyproject.toml
--rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-29 14:13:54.556256 jsno-1.0.2/setup.cfg
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.555190 jsno-1.0.2/tests/
--rw-r--r--   0 pekka      (501) staff       (20)     1129 2023-07-29 09:57:25.000000 jsno-1.0.2/tests/test_abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     3734 2023-07-29 14:05:59.000000 jsno-1.0.2/tests/test_dataclasses.py
--rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 13:51:44.000000 jsno-1.0.2/tests/test_dates.py
--rw-r--r--   0 pekka      (501) staff       (20)     1087 2023-07-15 09:44:23.000000 jsno-1.0.2/tests/test_examples.py
--rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 13:40:19.000000 jsno-1.0.2/tests/test_jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2734 2023-07-16 16:57:33.000000 jsno-1.0.2/tests/test_methods.py
--rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 13:38:35.000000 jsno-1.0.2/tests/test_standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4422 2023-07-29 14:00:17.000000 jsno-1.0.2/tests/test_unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2885 2023-07-29 07:58:13.000000 jsno-1.0.2/tests/test_variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.088676 jsno-1.0.3/
+-rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.3/LICENSE
+-rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:43:03.088272 jsno-1.0.3/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)     2281 2023-07-29 10:12:41.000000 jsno-1.0.3/README.md
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.080115 jsno-1.0.3/jsno/
+-rw-r--r--   0 pekka      (501) staff       (20)     1405 2023-07-29 14:38:38.000000 jsno-1.0.3/jsno/__init__.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2398 2023-07-29 14:33:44.000000 jsno-1.0.3/jsno/abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4438 2023-07-29 09:40:36.000000 jsno-1.0.3/jsno/jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      425 2023-07-23 10:01:17.000000 jsno-1.0.3/jsno/jsonize.py
+-rw-r--r--   0 pekka      (501) staff       (20)      494 2023-07-23 10:02:00.000000 jsno-1.0.3/jsno/method.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5243 2023-07-29 14:17:17.000000 jsno-1.0.3/jsno/standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4079 2023-07-29 14:35:11.000000 jsno-1.0.3/jsno/unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      869 2023-07-29 09:00:26.000000 jsno-1.0.3/jsno/utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3387 2023-07-29 08:59:40.000000 jsno-1.0.3/jsno/variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.082078 jsno-1.0.3/jsno.egg-info/
+-rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)      512 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/SOURCES.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/dependency_links.txt
+-rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/requires.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/top_level.txt
+-rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-29 14:38:45.000000 jsno-1.0.3/pyproject.toml
+-rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-29 14:43:03.088805 jsno-1.0.3/setup.cfg
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.087494 jsno-1.0.3/tests/
+-rw-r--r--   0 pekka      (501) staff       (20)     1129 2023-07-29 09:57:25.000000 jsno-1.0.3/tests/test_abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4207 2023-07-29 14:40:19.000000 jsno-1.0.3/tests/test_dataclasses.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 13:51:44.000000 jsno-1.0.3/tests/test_dates.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1087 2023-07-15 09:44:23.000000 jsno-1.0.3/tests/test_examples.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 13:40:19.000000 jsno-1.0.3/tests/test_jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2734 2023-07-16 16:57:33.000000 jsno-1.0.3/tests/test_methods.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 13:38:35.000000 jsno-1.0.3/tests/test_standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4436 2023-07-29 14:16:23.000000 jsno-1.0.3/tests/test_unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2885 2023-07-29 07:58:13.000000 jsno-1.0.3/tests/test_variant.py
```

### Comparing `jsno-1.0.2/LICENSE` & `jsno-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/PKG-INFO` & `jsno-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.2
+Version: 1.0.3
 Summary: Convert Python data to and from json-compatible data structures
 Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsno-1.0.2/README.md` & `jsno-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/jsno/__init__.py` & `jsno-1.0.3/jsno/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 from jsno.standard import jsonify_as_string
 from jsno.unjsonify import unjsonify, UnjsonifyError
 from jsno.variant import get_variantfamily, variantfamily, variantlabel
 
 import jsno.abc
 
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

### Comparing `jsno-1.0.2/jsno/abc.py` & `jsno-1.0.3/jsno/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import base64
 
 from collections.abc import ByteString, Mapping, Sequence, Set
 
 from jsno.jsonify import jsonify
 from jsno.unjsonify import unjsonify, typecheck, raise_error, cast
-from jsno.utils import get_args
+from jsno.utils import get_args, get_origin
 
 
 # Mapping
 
 
 @jsonify.register(Mapping)
 def _(value):
@@ -25,20 +25,25 @@
     Unjsonify any Mapping type. Expects the input value to be
     a JSON object (dict).
     """
 
     typecheck(value, dict, as_type)
 
     arg_types = get_args(as_type)
+
+    # need to take origin for this to work for Dict and List
+    origin = get_origin(as_type) or as_type
+
     if not arg_types:
-        return cast(value, as_type)
+        return cast(value, origin)
     else:
         unjsonify_key = unjsonify[arg_types[0]]
         unjsonify_val = unjsonify[arg_types[1]]
-        return as_type({
+
+        return origin({
             unjsonify_key(key): unjsonify_val(val)
             for (key, val) in value.items()
         })
 
 
 # Sequence
```

### Comparing `jsno-1.0.2/jsno/jsonify.py` & `jsno-1.0.3/jsno/jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/jsno/standard.py` & `jsno-1.0.3/jsno/standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 @jsonify.register(float)
 def _(value):
     return float(value)
 
 
 @unjsonify.register(float)
 def _(value, as_type):
-    typecheck(value, float, as_type)
+    typecheck(value, (float, int), as_type)
     return cast(value, as_type)
 
 
 # tuples
 
 
 @unjsonify.register(tuple)
```

### Comparing `jsno-1.0.2/jsno/unjsonify.py` & `jsno-1.0.3/jsno/unjsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/jsno/utils.py` & `jsno-1.0.3/jsno/utils.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/jsno/variant.py` & `jsno-1.0.3/jsno/variant.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/jsno.egg-info/PKG-INFO` & `jsno-1.0.3/jsno.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.2
+Version: 1.0.3
 Summary: Convert Python data to and from json-compatible data structures
 Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsno-1.0.2/jsno.egg-info/SOURCES.txt` & `jsno-1.0.3/jsno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/pyproject.toml` & `jsno-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsno"
-version = "1.0.2"
+version = "1.0.3"
 description = "Convert Python data to and from json-compatible data structures"
 readme = "README.md"
 authors = [{ name = "Pekka Uronen", email = "pekka.uronen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `jsno-1.0.2/tests/test_abc.py` & `jsno-1.0.3/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/tests/test_dataclasses.py` & `jsno-1.0.3/tests/test_dataclasses.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """
 
 import dataclasses
 import enum
 import pytest
 
+from typing import Any, Dict, List
 
 from jsno import jsonify, unjsonify, jsonify_with_method, UnjsonifyError
 
 
 class Color(enum.Enum):
     Red = 1
     Green = 2
@@ -155,21 +156,32 @@
         unjsonify[Box]({})
 
 
 @dataclasses.dataclass
 class User:
     username: str
     password: str = 'pAssW0rd'
+    metadata: List[Dict[str, Any]] = dataclasses.field(default_factory=list)
 
 
 def test_jsonifty_dataclass_with_default_value():
     assert (
         jsonify(User(username="usr")) ==
-        {"username": "usr", "password": "pAssW0rd"}
+        {"username": "usr", "password": "pAssW0rd", "metadata": []}
+    )
+
+    assert (
+        jsonify(User(username="usr", password="", metadata=[{"key": 100}])) ==
+        {"username": "usr", "password": "", "metadata": [{"key": 100}]}
     )
 
 
 def test_unjsonifty_dataclass_with_default_value():
     user = unjsonify[User]({"username": "usr"})
 
     assert user == User(username="usr")
     assert user.password == "pAssW0rd"
+
+    user = unjsonify[User]({"username": "usr", "password": "", "metadata":  [{"key": 100}]})
+
+    assert user == User(username="usr", password="", metadata=[{"key": 100}])
+
```

### Comparing `jsno-1.0.2/tests/test_dates.py` & `jsno-1.0.3/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/tests/test_examples.py` & `jsno-1.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/tests/test_jsonify.py` & `jsno-1.0.3/tests/test_jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/tests/test_methods.py` & `jsno-1.0.3/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/tests/test_standard.py` & `jsno-1.0.3/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.2/tests/test_unjsonify.py` & `jsno-1.0.3/tests/test_unjsonify.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 def test_unjsonify_typed_dict():
     assert unjsonify[dict[str, int]]({'x': 1, 'y': 2}) == {'x': 1, 'y': 2}
 
 
 def test_unjsonify_list_of_floats():
-    assert unjsonify[list[float]]([1.0, 2.0, 3.0]) == [1, 2, 3.0]
+    assert unjsonify[list[float]]([1.0, 2.0, 3.0, 0, -2]) == [1, 2, 3.0, 0, -2]
 
 
 def test_unjsonify_list_of_bools():
     assert unjsonify[list[bool]]([True, False]) == [True, False]
 
 
 def test_unjsonify_set_of_ints():
```

### Comparing `jsno-1.0.2/tests/test_variant.py` & `jsno-1.0.3/tests/test_variant.py`

 * *Files identical despite different names*

