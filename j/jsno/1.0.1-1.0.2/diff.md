# Comparing `tmp/jsno-1.0.1.tar.gz` & `tmp/jsno-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsno-1.0.1.tar", last modified: Sat Jul 29 13:54:48 2023, max compression
+gzip compressed data, was "jsno-1.0.2.tar", last modified: Sat Jul 29 14:13:54 2023, max compression
```

## Comparing `jsno-1.0.1.tar` & `jsno-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.422252 jsno-1.0.1/
--rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.1/LICENSE
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 13:54:48.421816 jsno-1.0.1/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)     2281 2023-07-29 10:12:41.000000 jsno-1.0.1/README.md
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.413819 jsno-1.0.1/jsno/
--rw-r--r--   0 pekka      (501) staff       (20)     1405 2023-07-29 13:52:59.000000 jsno-1.0.1/jsno/__init__.py
--rw-r--r--   0 pekka      (501) staff       (20)     2280 2023-07-28 18:51:39.000000 jsno-1.0.1/jsno/abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     4438 2023-07-29 09:40:36.000000 jsno-1.0.1/jsno/jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      425 2023-07-23 10:01:17.000000 jsno-1.0.1/jsno/jsonize.py
--rw-r--r--   0 pekka      (501) staff       (20)      494 2023-07-23 10:02:00.000000 jsno-1.0.1/jsno/method.py
--rw-r--r--   0 pekka      (501) staff       (20)     5236 2023-07-29 13:29:17.000000 jsno-1.0.1/jsno/standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4103 2023-07-29 09:28:49.000000 jsno-1.0.1/jsno/unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      869 2023-07-29 09:00:26.000000 jsno-1.0.1/jsno/utils.py
--rw-r--r--   0 pekka      (501) staff       (20)     3387 2023-07-29 08:59:40.000000 jsno-1.0.1/jsno/variant.py
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.415717 jsno-1.0.1/jsno.egg-info/
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)      512 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/SOURCES.txt
--rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/dependency_links.txt
--rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/requires.txt
--rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/top_level.txt
--rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-29 13:52:56.000000 jsno-1.0.1/pyproject.toml
--rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-29 13:54:48.422366 jsno-1.0.1/setup.cfg
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.421023 jsno-1.0.1/tests/
--rw-r--r--   0 pekka      (501) staff       (20)     1129 2023-07-29 09:57:25.000000 jsno-1.0.1/tests/test_abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     3303 2023-07-28 20:12:26.000000 jsno-1.0.1/tests/test_dataclasses.py
--rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 13:51:44.000000 jsno-1.0.1/tests/test_dates.py
--rw-r--r--   0 pekka      (501) staff       (20)     1087 2023-07-15 09:44:23.000000 jsno-1.0.1/tests/test_examples.py
--rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 13:40:19.000000 jsno-1.0.1/tests/test_jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2734 2023-07-16 16:57:33.000000 jsno-1.0.1/tests/test_methods.py
--rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 13:38:35.000000 jsno-1.0.1/tests/test_standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4349 2023-07-29 13:41:17.000000 jsno-1.0.1/tests/test_unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2885 2023-07-29 07:58:13.000000 jsno-1.0.1/tests/test_variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.556135 jsno-1.0.2/
+-rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.2/LICENSE
+-rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:13:54.555737 jsno-1.0.2/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)     2281 2023-07-29 10:12:41.000000 jsno-1.0.2/README.md
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.550322 jsno-1.0.2/jsno/
+-rw-r--r--   0 pekka      (501) staff       (20)     1405 2023-07-29 14:12:43.000000 jsno-1.0.2/jsno/__init__.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2280 2023-07-28 18:51:39.000000 jsno-1.0.2/jsno/abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4438 2023-07-29 09:40:36.000000 jsno-1.0.2/jsno/jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      425 2023-07-23 10:01:17.000000 jsno-1.0.2/jsno/jsonize.py
+-rw-r--r--   0 pekka      (501) staff       (20)      494 2023-07-23 10:02:00.000000 jsno-1.0.2/jsno/method.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5236 2023-07-29 13:29:17.000000 jsno-1.0.2/jsno/standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4079 2023-07-29 14:07:49.000000 jsno-1.0.2/jsno/unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      869 2023-07-29 09:00:26.000000 jsno-1.0.2/jsno/utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3387 2023-07-29 08:59:40.000000 jsno-1.0.2/jsno/variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.551695 jsno-1.0.2/jsno.egg-info/
+-rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)      512 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/SOURCES.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/dependency_links.txt
+-rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/requires.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-29 14:13:54.000000 jsno-1.0.2/jsno.egg-info/top_level.txt
+-rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-29 14:13:01.000000 jsno-1.0.2/pyproject.toml
+-rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-29 14:13:54.556256 jsno-1.0.2/setup.cfg
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:13:54.555190 jsno-1.0.2/tests/
+-rw-r--r--   0 pekka      (501) staff       (20)     1129 2023-07-29 09:57:25.000000 jsno-1.0.2/tests/test_abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3734 2023-07-29 14:05:59.000000 jsno-1.0.2/tests/test_dataclasses.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 13:51:44.000000 jsno-1.0.2/tests/test_dates.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1087 2023-07-15 09:44:23.000000 jsno-1.0.2/tests/test_examples.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 13:40:19.000000 jsno-1.0.2/tests/test_jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2734 2023-07-16 16:57:33.000000 jsno-1.0.2/tests/test_methods.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 13:38:35.000000 jsno-1.0.2/tests/test_standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4422 2023-07-29 14:00:17.000000 jsno-1.0.2/tests/test_unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2885 2023-07-29 07:58:13.000000 jsno-1.0.2/tests/test_variant.py
```

### Comparing `jsno-1.0.1/LICENSE` & `jsno-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/PKG-INFO` & `jsno-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert Python data to and from json-compatible data structures
 Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsno-1.0.1/README.md` & `jsno-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/jsno/__init__.py` & `jsno-1.0.2/jsno/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 from jsno.standard import jsonify_as_string
 from jsno.unjsonify import unjsonify, UnjsonifyError
 from jsno.variant import get_variantfamily, variantfamily, variantlabel
 
 import jsno.abc
 
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
```

### Comparing `jsno-1.0.1/jsno/abc.py` & `jsno-1.0.2/jsno/abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/jsno/jsonify.py` & `jsno-1.0.2/jsno/jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/jsno/standard.py` & `jsno-1.0.2/jsno/standard.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/jsno/unjsonify.py` & `jsno-1.0.2/jsno/unjsonify.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,21 +65,17 @@
 
 def unjsonify_dataclass(value, as_type):
     typecheck(value, dict, as_type)
 
     # collect all properties in the input value that match any of
     # the dataclass fields
     kwargs = {
-        field.name:  unjsonify[field.type](value.get(field.name))
+        field.name: unjsonify[field.type](value.get(field.name))
         for field in get_dataclass_fields(as_type)
-        if (
-            field.name in value or
-            field.default is not dataclasses.MISSING or
-            field.default_factory is not dataclasses.MISSING
-        )
+        if field.name in value
     }
     try:
         return as_type(**kwargs)
     except TypeError as exc:
         detail = exc.args[0]
 
     raise_error(value, as_type, detail)
@@ -153,7 +149,13 @@
         try:
             return unjsonify[type_option](value)
         except UnjsonifyError:
             # try next option
             continue
 
     raise UnjsonifyError(f"Cannot unjsonify as {as_type}", value)
+
+
+@unjsonify.register(Any)
+def _(value, as_type):
+    """ Unjsonify Any type: just return the value """
+    return value
```

### Comparing `jsno-1.0.1/jsno/utils.py` & `jsno-1.0.2/jsno/utils.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/jsno/variant.py` & `jsno-1.0.2/jsno/variant.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/jsno.egg-info/PKG-INFO` & `jsno-1.0.2/jsno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert Python data to and from json-compatible data structures
 Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsno-1.0.1/jsno.egg-info/SOURCES.txt` & `jsno-1.0.2/jsno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/pyproject.toml` & `jsno-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsno"
-version = "1.0.1"
+version = "1.0.2"
 description = "Convert Python data to and from json-compatible data structures"
 readme = "README.md"
 authors = [{ name = "Pekka Uronen", email = "pekka.uronen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `jsno-1.0.1/tests/test_abc.py` & `jsno-1.0.2/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/tests/test_dataclasses.py` & `jsno-1.0.2/tests/test_dataclasses.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,7 +150,26 @@
         unjsonify[Brick]("Something else")
 
 
 def test_unjsonify_dataclass_error():
     with pytest.raises(UnjsonifyError):
         unjsonify[Box]({})
 
+
+@dataclasses.dataclass
+class User:
+    username: str
+    password: str = 'pAssW0rd'
+
+
+def test_jsonifty_dataclass_with_default_value():
+    assert (
+        jsonify(User(username="usr")) ==
+        {"username": "usr", "password": "pAssW0rd"}
+    )
+
+
+def test_unjsonifty_dataclass_with_default_value():
+    user = unjsonify[User]({"username": "usr"})
+
+    assert user == User(username="usr")
+    assert user.password == "pAssW0rd"
```

### Comparing `jsno-1.0.1/tests/test_dates.py` & `jsno-1.0.2/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/tests/test_examples.py` & `jsno-1.0.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/tests/test_jsonify.py` & `jsno-1.0.2/tests/test_jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/tests/test_methods.py` & `jsno-1.0.2/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/tests/test_standard.py` & `jsno-1.0.2/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.1/tests/test_unjsonify.py` & `jsno-1.0.2/tests/test_unjsonify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import collections
 import datetime
 import pytest
 import zoneinfo
 
-from typing import Callable, Optional, List, Literal
+from typing import Any, Callable, Optional, List, Literal
 
 from jsno.unjsonify import unjsonify, UnjsonifyError
 
 
 helsinki = zoneinfo.ZoneInfo("Europe/Helsinki")
 utc = zoneinfo.ZoneInfo("UTC")
 
 
 def test_unjsonify_none():
     assert unjsonify[type(None)](None) == None
 
 
+def test_unjsonify_any():
+    assert unjsonify[Any](None) == None
+
+
 def test_unjsonify_none_from_string_fails():
     with pytest.raises(UnjsonifyError):
         assert unjsonify[type(None)]("foo") == None
 
 
 def test_unjsonify_string():
     assert unjsonify[str]("foo") == "foo"
```

### Comparing `jsno-1.0.1/tests/test_variant.py` & `jsno-1.0.2/tests/test_variant.py`

 * *Files identical despite different names*

