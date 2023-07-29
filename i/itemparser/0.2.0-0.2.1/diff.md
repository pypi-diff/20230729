# Comparing `tmp/itemparser-0.2.0.tar.gz` & `tmp/itemparser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemparser-0.2.0.tar", max compression
+gzip compressed data, was "itemparser-0.2.1.tar", max compression
```

## Comparing `itemparser-0.2.0.tar` & `itemparser-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       12 2023-07-26 03:43:21.765278 itemparser-0.2.0/README.md
--rw-r--r--   0        0        0      407 2023-07-26 03:43:21.765278 itemparser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      106 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/__init__.py
--rw-r--r--   0        0        0     1490 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/field.py
--rw-r--r--   0        0        0     2243 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/parser.py
--rw-r--r--   0        0        0     3317 2023-07-26 03:43:21.765278 itemparser-0.2.0/src/itemparser/processor.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 itemparser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-07-29 15:46:20.124358 itemparser-0.2.1/README.md
+-rw-r--r--   0        0        0      407 2023-07-29 15:46:20.124358 itemparser-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-07-29 15:46:20.124358 itemparser-0.2.1/src/itemparser/__init__.py
+-rw-r--r--   0        0        0     1490 2023-07-29 15:46:20.124358 itemparser-0.2.1/src/itemparser/field.py
+-rw-r--r--   0        0        0     2243 2023-07-29 15:46:20.124358 itemparser-0.2.1/src/itemparser/parser.py
+-rw-r--r--   0        0        0     3557 2023-07-29 15:46:20.124358 itemparser-0.2.1/src/itemparser/processor.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 itemparser-0.2.1/PKG-INFO
```

### Comparing `itemparser-0.2.0/src/itemparser/field.py` & `itemparser-0.2.1/src/itemparser/field.py`

 * *Files identical despite different names*

### Comparing `itemparser-0.2.0/src/itemparser/parser.py` & `itemparser-0.2.1/src/itemparser/parser.py`

 * *Files identical despite different names*

### Comparing `itemparser-0.2.0/src/itemparser/processor.py` & `itemparser-0.2.1/src/itemparser/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,14 +84,24 @@
 
     def __call__(self, values):
         for value in values:
             if value and value != "":
                 return value
 
 
+class Join(Processor):
+    """ Concatenate any list of strings. """
+
+    def __init__(self, join_string=''):
+        self.join_string = join_string
+
+    def __call__(self, values):
+        return self.join_string.join(values)
+
+
 class Middle(Processor):
     """ get middle text from value """
 
     def __init__(self, left: str, right: str, flags=0):
         self.left = left
         self.right = right
         self.pattern = re.compile(fr"{left}(.*?){right}", flags)
@@ -150,14 +160,15 @@
 
 
 __all__ = [
     'Identity',
     'Compose',
     'Loop',
     'First',
+    'Join',
     'Middle',
     'Format',
     'Upper',
     'Strip',
     'Filter',
     'To',
 ]
```

