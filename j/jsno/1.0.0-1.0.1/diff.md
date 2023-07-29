# Comparing `tmp/jsno-1.0.0.tar.gz` & `tmp/jsno-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsno-1.0.0.tar", last modified: Sat Jul 29 12:50:06 2023, max compression
+gzip compressed data, was "jsno-1.0.1.tar", last modified: Sat Jul 29 13:54:48 2023, max compression
```

## Comparing `jsno-1.0.0.tar` & `jsno-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 12:50:06.803198 jsno-1.0.0/
--rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.0/LICENSE
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 12:50:06.802758 jsno-1.0.0/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)     2281 2023-07-29 10:12:41.000000 jsno-1.0.0/README.md
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 12:50:06.794408 jsno-1.0.0/jsno/
--rw-r--r--   0 pekka      (501) staff       (20)     1405 2023-07-29 12:20:29.000000 jsno-1.0.0/jsno/__init__.py
--rw-r--r--   0 pekka      (501) staff       (20)     2280 2023-07-28 18:51:39.000000 jsno-1.0.0/jsno/abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     4438 2023-07-29 09:40:36.000000 jsno-1.0.0/jsno/jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      425 2023-07-23 10:01:17.000000 jsno-1.0.0/jsno/jsonize.py
--rw-r--r--   0 pekka      (501) staff       (20)      494 2023-07-23 10:02:00.000000 jsno-1.0.0/jsno/method.py
--rw-r--r--   0 pekka      (501) staff       (20)     5090 2023-07-29 10:12:32.000000 jsno-1.0.0/jsno/standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4103 2023-07-29 09:28:49.000000 jsno-1.0.0/jsno/unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      869 2023-07-29 09:00:26.000000 jsno-1.0.0/jsno/utils.py
--rw-r--r--   0 pekka      (501) staff       (20)     3387 2023-07-29 08:59:40.000000 jsno-1.0.0/jsno/variant.py
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 12:50:06.796076 jsno-1.0.0/jsno.egg-info/
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 12:50:06.000000 jsno-1.0.0/jsno.egg-info/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)      492 2023-07-29 12:50:06.000000 jsno-1.0.0/jsno.egg-info/SOURCES.txt
--rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-29 12:50:06.000000 jsno-1.0.0/jsno.egg-info/dependency_links.txt
--rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-29 12:50:06.000000 jsno-1.0.0/jsno.egg-info/requires.txt
--rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-29 12:50:06.000000 jsno-1.0.0/jsno.egg-info/top_level.txt
--rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-29 12:49:34.000000 jsno-1.0.0/pyproject.toml
--rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-29 12:50:06.803322 jsno-1.0.0/setup.cfg
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 12:50:06.801652 jsno-1.0.0/tests/
--rw-r--r--   0 pekka      (501) staff       (20)     1129 2023-07-29 09:57:25.000000 jsno-1.0.0/tests/test_abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     3303 2023-07-28 20:12:26.000000 jsno-1.0.0/tests/test_dataclasses.py
--rw-r--r--   0 pekka      (501) staff       (20)     1087 2023-07-15 09:44:23.000000 jsno-1.0.0/tests/test_examples.py
--rw-r--r--   0 pekka      (501) staff       (20)     3937 2023-07-29 09:58:01.000000 jsno-1.0.0/tests/test_jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2734 2023-07-16 16:57:33.000000 jsno-1.0.0/tests/test_methods.py
--rw-r--r--   0 pekka      (501) staff       (20)     1714 2023-07-29 10:11:48.000000 jsno-1.0.0/tests/test_standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     5371 2023-07-29 09:58:55.000000 jsno-1.0.0/tests/test_unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2885 2023-07-29 07:58:13.000000 jsno-1.0.0/tests/test_variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.422252 jsno-1.0.1/
+-rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.1/LICENSE
+-rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 13:54:48.421816 jsno-1.0.1/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)     2281 2023-07-29 10:12:41.000000 jsno-1.0.1/README.md
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.413819 jsno-1.0.1/jsno/
+-rw-r--r--   0 pekka      (501) staff       (20)     1405 2023-07-29 13:52:59.000000 jsno-1.0.1/jsno/__init__.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2280 2023-07-28 18:51:39.000000 jsno-1.0.1/jsno/abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4438 2023-07-29 09:40:36.000000 jsno-1.0.1/jsno/jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      425 2023-07-23 10:01:17.000000 jsno-1.0.1/jsno/jsonize.py
+-rw-r--r--   0 pekka      (501) staff       (20)      494 2023-07-23 10:02:00.000000 jsno-1.0.1/jsno/method.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5236 2023-07-29 13:29:17.000000 jsno-1.0.1/jsno/standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4103 2023-07-29 09:28:49.000000 jsno-1.0.1/jsno/unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      869 2023-07-29 09:00:26.000000 jsno-1.0.1/jsno/utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3387 2023-07-29 08:59:40.000000 jsno-1.0.1/jsno/variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.415717 jsno-1.0.1/jsno.egg-info/
+-rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)      512 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/SOURCES.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/dependency_links.txt
+-rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/requires.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-29 13:54:48.000000 jsno-1.0.1/jsno.egg-info/top_level.txt
+-rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-29 13:52:56.000000 jsno-1.0.1/pyproject.toml
+-rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-29 13:54:48.422366 jsno-1.0.1/setup.cfg
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 13:54:48.421023 jsno-1.0.1/tests/
+-rw-r--r--   0 pekka      (501) staff       (20)     1129 2023-07-29 09:57:25.000000 jsno-1.0.1/tests/test_abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3303 2023-07-28 20:12:26.000000 jsno-1.0.1/tests/test_dataclasses.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 13:51:44.000000 jsno-1.0.1/tests/test_dates.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1087 2023-07-15 09:44:23.000000 jsno-1.0.1/tests/test_examples.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 13:40:19.000000 jsno-1.0.1/tests/test_jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2734 2023-07-16 16:57:33.000000 jsno-1.0.1/tests/test_methods.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 13:38:35.000000 jsno-1.0.1/tests/test_standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4349 2023-07-29 13:41:17.000000 jsno-1.0.1/tests/test_unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2885 2023-07-29 07:58:13.000000 jsno-1.0.1/tests/test_variant.py
```

### Comparing `jsno-1.0.0/LICENSE` & `jsno-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/PKG-INFO` & `jsno-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert Python data to and from json-compatible data structures
 Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsno-1.0.0/README.md` & `jsno-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/jsno/__init__.py` & `jsno-1.0.1/jsno/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 from jsno.standard import jsonify_as_string
 from jsno.unjsonify import unjsonify, UnjsonifyError
 from jsno.variant import get_variantfamily, variantfamily, variantlabel
 
 import jsno.abc
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `jsno-1.0.0/jsno/abc.py` & `jsno-1.0.1/jsno/abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/jsno/jsonify.py` & `jsno-1.0.1/jsno/jsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/jsno/standard.py` & `jsno-1.0.1/jsno/standard.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,22 +183,29 @@
 
 # datetime.datetime
 
 
 UTC = zoneinfo.ZoneInfo("UTC")
 
 
+def is_utc_datetime(dt) -> bool:
+    return (
+        dt.tzinfo is not None and
+        dt.tzinfo.utcoffset(dt).total_seconds() == 0.0
+    )
+
+
 @jsonify.register(datetime.datetime)
 def _(value):
     """
     Format the datetime as a string. Uses isoformat, except  when
     the timezone is UTC, attaches "Z" as the timezone, instead of "+00:00"
     """
 
-    if value.tzinfo == UTC:
+    if is_utc_datetime(value):
         return f"{value.date()}T{value.time()}Z"
     else:
         return value.isoformat()
 
 
 @unjsonify.register(datetime.datetime)
 def _(value, as_type):
```

### Comparing `jsno-1.0.0/jsno/unjsonify.py` & `jsno-1.0.1/jsno/unjsonify.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/jsno/utils.py` & `jsno-1.0.1/jsno/utils.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/jsno/variant.py` & `jsno-1.0.1/jsno/variant.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/jsno.egg-info/PKG-INFO` & `jsno-1.0.1/jsno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsno
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert Python data to and from json-compatible data structures
 Author-email: Pekka Uronen <pekka.uronen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 pek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsno-1.0.0/pyproject.toml` & `jsno-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsno"
-version = "1.0.0"
+version = "1.0.1"
 description = "Convert Python data to and from json-compatible data structures"
 readme = "README.md"
 authors = [{ name = "Pekka Uronen", email = "pekka.uronen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `jsno-1.0.0/tests/test_abc.py` & `jsno-1.0.1/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/tests/test_dataclasses.py` & `jsno-1.0.1/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/tests/test_examples.py` & `jsno-1.0.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/tests/test_jsonify.py` & `jsno-1.0.1/tests/test_jsonify.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import collections
 import datetime
-import zoneinfo
 
 import pytest
 
 from jsno.jsonify import jsonify
 
 
-helsinki = zoneinfo.ZoneInfo("Europe/Helsinki")
-utc = zoneinfo.ZoneInfo("UTC")
-
 
 def test_jsonify_none():
     assert jsonify(None) == None
 
 
 def test_jsonify_string():
     assert jsonify("foo") == "foo"
@@ -42,57 +38,14 @@
     assert jsonify([True, False]) == [True, False]
 
 
 def test_jsonify_counter():
     assert jsonify(collections.Counter("abababa") == {"a": 4, "b": 3})
 
 
-def test_jsonify_dates():
-
-    assert (
-        jsonify(
-            [
-                datetime.datetime(2023, 7, 15, 8, 39, 0, tzinfo=helsinki),
-                datetime.datetime(2023, 7, 15, 8, 40, 10, tzinfo=utc),
-                datetime.datetime(2023, 7, 15, 8, 41, 20),
-                datetime.datetime(2023, 7, 15, 8, 39, 0, 1, tzinfo=helsinki),
-                datetime.datetime(2023, 7, 15, 8, 40, 10, 120, tzinfo=utc),
-                datetime.datetime(5012, 7, 15, 8, 41, 20, 123400),
-            ]
-        )
-        ==
-        [
-            "2023-07-15T08:39:00+03:00",
-            "2023-07-15T08:40:10Z",
-            "2023-07-15T08:41:20",
-            "2023-07-15T08:39:00.000001+03:00",
-            "2023-07-15T08:40:10.000120Z",
-            "5012-07-15T08:41:20.123400",
-        ]
-    )
-
-def test_jsonify_old_dates():
-    assert (
-        jsonify(
-            [
-                datetime.datetime(1940, 7, 15, 8, 39, 0, tzinfo=helsinki),
-                datetime.datetime(1960, 7, 15, 8, 39, 0, tzinfo=helsinki),
-                datetime.datetime(1980, 7, 15, 8, 39, 0, tzinfo=helsinki),
-                datetime.datetime(1981, 7, 15, 8, 39, 0, tzinfo=helsinki),
-            ]
-        )
-        ==
-        [
-            "1940-07-15T08:39:00+02:00",
-            "1960-07-15T08:39:00+02:00",
-            "1980-07-15T08:39:00+02:00",
-            "1981-07-15T08:39:00+03:00",
-        ]
-    )
-
 def test_jsonify_dictionary_with_date_and_name():
     assert (
         jsonify({"name": "test", "date": datetime.date(2023, 7, 16)})
         ==
         {"name": "test", "date": "2023-07-16"}
     )
```

### Comparing `jsno-1.0.0/tests/test_methods.py` & `jsno-1.0.1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `jsno-1.0.0/tests/test_standard.py` & `jsno-1.0.1/tests/test_standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 def run_tests(value, json):
     assert jsonify(value) == json
     assert unjsonify[type(value)](json) == value
 
 
-
 def test_jsonify_decimal():
     assert jsonify(decimal.Decimal("99.9")) == "99.9"
 
 
 def test_unjsonify_decimal():
     assert unjsonify[decimal.Decimal]("99.9") == decimal.Decimal("99.9")
```

### Comparing `jsno-1.0.0/tests/test_unjsonify.py` & `jsno-1.0.1/tests/test_unjsonify.py`

 * *Files 15% similar despite different names*

```diff
@@ -114,38 +114,14 @@
 
 
 def test_unjsonify_literal_failure():
     with pytest.raises(UnjsonifyError):
         unjsonify[Literal["A", "B"]]("C")
 
 
-def test_unjsonify_list_of_datetimes():
-    assert (
-        unjsonify[list[datetime.datetime]](
-            [
-                "2023-07-15T08:39:00+03:00",
-                "2023-07-15T08:40:10Z",
-                "2023-07-15T08:41:20",
-                "2023-07-15T08:39:00.000001+03:00",
-                "2023-07-15T08:40:10.000120Z",
-                "5012-07-15T08:41:20.123400",
-            ]
-        ) == (
-            [
-                datetime.datetime(2023, 7, 15, 8, 39, 0, tzinfo=helsinki),
-                datetime.datetime(2023, 7, 15, 8, 40, 10, tzinfo=utc),
-                datetime.datetime(2023, 7, 15, 8, 41, 20),
-                datetime.datetime(2023, 7, 15, 8, 39, 0, 1, tzinfo=helsinki),
-                datetime.datetime(2023, 7, 15, 8, 40, 10, 120, tzinfo=utc),
-                datetime.datetime(5012, 7, 15, 8, 41, 20, 123400),
-            ]
-        )
-    )
-
-
 def test_unjsonify_dictionary_of_dates():
     assert(
         unjsonify[dict[datetime.date, datetime.date]](
             {
                 "2023-07-15": "2023-07-16",
                 "2023-07-16": "2023-07-17",
             }
@@ -154,19 +130,14 @@
                 datetime.date(2023, 7, 15): datetime.date(2023, 7, 16),
                 datetime.date(2023, 7, 16): datetime.date(2023, 7, 17),
             }
         )
     )
 
 
-def test_unjsonify_datetime_failure():
-    with pytest.raises(UnjsonifyError):
-        unjsonify[datetime.datetime]('2023-13-13T12:34:56')
-
-
 def test_unjsonify_bytes():
     assert unjsonify[bytes]("Zm9vYmFyIQ==") == b"foobar!"
 
 
 def test_unjsonify_str_subclass():
 
     class SpecialString(str):
```

### Comparing `jsno-1.0.0/tests/test_variant.py` & `jsno-1.0.1/tests/test_variant.py`

 * *Files identical despite different names*

