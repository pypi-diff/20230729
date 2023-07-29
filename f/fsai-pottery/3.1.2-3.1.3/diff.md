# Comparing `tmp/fsai_pottery-3.1.2.tar.gz` & `tmp/fsai_pottery-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsai_pottery-3.1.2.tar", max compression
+gzip compressed data, was "fsai_pottery-3.1.3.tar", max compression
```

## Comparing `fsai_pottery-3.1.2.tar` & `fsai_pottery-3.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11358 2023-07-29 16:22:56.696850 fsai_pottery-3.1.2/LICENSE
--rw-r--r--   0        0        0    33773 2023-07-29 16:22:56.697140 fsai_pottery-3.1.2/README.md
--rw-r--r--   0        0        0     4330 2023-07-29 16:22:56.697362 fsai_pottery-3.1.2/pottery/__init__.py
--rw-r--r--   0        0        0     6128 2023-07-29 16:22:56.697490 fsai_pottery-3.1.2/pottery/aionextid.py
--rw-r--r--   0        0        0    24162 2023-07-29 16:22:56.697565 fsai_pottery-3.1.2/pottery/aioredlock.py
--rw-r--r--   0        0        0     1705 2023-07-29 16:22:56.697701 fsai_pottery-3.1.2/pottery/annotations.py
--rw-r--r--   0        0        0    11408 2023-07-29 16:22:56.697817 fsai_pottery-3.1.2/pottery/base.py
--rw-r--r--   0        0        0    15338 2023-07-29 16:22:56.697917 fsai_pottery-3.1.2/pottery/bloom.py
--rw-r--r--   0        0        0    13808 2023-07-29 16:22:56.698018 fsai_pottery-3.1.2/pottery/cache.py
--rw-r--r--   0        0        0    10795 2023-07-29 16:22:56.698106 fsai_pottery-3.1.2/pottery/counter.py
--rw-r--r--   0        0        0     7840 2023-07-29 16:22:56.698191 fsai_pottery-3.1.2/pottery/deque.py
--rw-r--r--   0        0        0     6962 2023-07-29 16:22:56.698341 fsai_pottery-3.1.2/pottery/dict.py
--rw-r--r--   0        0        0     3021 2023-07-29 16:22:56.698444 fsai_pottery-3.1.2/pottery/exceptions.py
--rw-r--r--   0        0        0     3803 2023-07-29 16:22:56.698521 fsai_pottery-3.1.2/pottery/executor.py
--rw-r--r--   0        0        0     9265 2023-07-29 16:22:56.698800 fsai_pottery-3.1.2/pottery/hyper.py
--rw-r--r--   0        0        0    16529 2023-07-29 16:22:56.698955 fsai_pottery-3.1.2/pottery/list.py
--rw-r--r--   0        0        0     2864 2023-07-29 16:22:56.699507 fsai_pottery-3.1.2/pottery/monkey.py
--rw-r--r--   0        0        0    10485 2023-07-29 16:22:56.699653 fsai_pottery-3.1.2/pottery/nextid.py
--rw-r--r--   0        0        0        0 2023-07-29 16:22:56.699687 fsai_pottery-3.1.2/pottery/py.typed
--rw-r--r--   0        0        0     6103 2023-07-29 16:22:56.699786 fsai_pottery-3.1.2/pottery/queue.py
--rw-r--r--   0        0        0    28690 2023-07-29 16:22:56.699855 fsai_pottery-3.1.2/pottery/redlock.py
--rw-r--r--   0        0        0    11741 2023-07-29 16:22:56.699927 fsai_pottery-3.1.2/pottery/set.py
--rw-r--r--   0        0        0     4620 2023-07-29 16:22:56.700000 fsai_pottery-3.1.2/pottery/timer.py
--rw-r--r--   0        0        0     1447 2023-07-29 17:09:40.967478 fsai_pottery-3.1.2/pyproject.toml
--rw-r--r--   0        0        0    36304 1970-01-01 00:00:00.000000 fsai_pottery-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/LICENSE
+-rw-r--r--   0        0        0    33773 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/README.md
+-rw-r--r--   0        0        0     4330 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/__init__.py
+-rw-r--r--   0        0        0     6128 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/aionextid.py
+-rw-r--r--   0        0        0    24162 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/aioredlock.py
+-rw-r--r--   0        0        0     1705 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/annotations.py
+-rw-r--r--   0        0        0    11408 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/base.py
+-rw-r--r--   0        0        0    15338 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/bloom.py
+-rw-r--r--   0        0        0    13808 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/cache.py
+-rw-r--r--   0        0        0    10795 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/counter.py
+-rw-r--r--   0        0        0     7840 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/deque.py
+-rw-r--r--   0        0        0     6962 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/dict.py
+-rw-r--r--   0        0        0     3021 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/exceptions.py
+-rw-r--r--   0        0        0     3803 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/executor.py
+-rw-r--r--   0        0        0     9265 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/hyper.py
+-rw-r--r--   0        0        0    16529 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/list.py
+-rw-r--r--   0        0        0     2864 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/monkey.py
+-rw-r--r--   0        0        0    10485 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/nextid.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/py.typed
+-rw-r--r--   0        0        0     6103 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/queue.py
+-rw-r--r--   0        0        0    28690 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/redlock.py
+-rw-r--r--   0        0        0    11741 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/set.py
+-rw-r--r--   0        0        0     4620 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/timer.py
+-rw-r--r--   0        0        0     1447 2023-07-29 17:12:07.697758 fsai_pottery-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0    36304 1970-01-01 00:00:00.000000 fsai_pottery-3.1.3/PKG-INFO
```

### Comparing `fsai_pottery-3.1.2/LICENSE` & `fsai_pottery-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/README.md` & `fsai_pottery-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/__init__.py` & `fsai_pottery-3.1.3/pottery/__init__.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/aionextid.py` & `fsai_pottery-3.1.3/pottery/aionextid.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/aioredlock.py` & `fsai_pottery-3.1.3/pottery/aioredlock.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/annotations.py` & `fsai_pottery-3.1.3/pottery/annotations.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/base.py` & `fsai_pottery-3.1.3/pottery/base.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/bloom.py` & `fsai_pottery-3.1.3/pottery/bloom.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/cache.py` & `fsai_pottery-3.1.3/pottery/cache.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/counter.py` & `fsai_pottery-3.1.3/pottery/counter.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/deque.py` & `fsai_pottery-3.1.3/pottery/deque.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/dict.py` & `fsai_pottery-3.1.3/pottery/dict.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/exceptions.py` & `fsai_pottery-3.1.3/pottery/exceptions.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/executor.py` & `fsai_pottery-3.1.3/pottery/executor.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/hyper.py` & `fsai_pottery-3.1.3/pottery/hyper.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/list.py` & `fsai_pottery-3.1.3/pottery/list.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/monkey.py` & `fsai_pottery-3.1.3/pottery/monkey.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/nextid.py` & `fsai_pottery-3.1.3/pottery/nextid.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/queue.py` & `fsai_pottery-3.1.3/pottery/queue.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/redlock.py` & `fsai_pottery-3.1.3/pottery/redlock.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/set.py` & `fsai_pottery-3.1.3/pottery/set.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pottery/timer.py` & `fsai_pottery-3.1.3/pottery/timer.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.2/pyproject.toml` & `fsai_pottery-3.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fsai-pottery"
-version = "v3.1.2"
+version = "v3.1.3"
 description = "Redis for humans. 🌎🌍🌏"
 authors = ["Rajiv Bakulesh Shah"]
 license = "Apache License"
 readme = "README.md"
 packages = [{include = "pottery"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fsai_pottery-3.1.2/PKG-INFO` & `fsai_pottery-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsai-pottery
-Version: 3.1.2
+Version: 3.1.3
 Summary: Redis for humans. 🌎🌍🌏
 License: Apache License
 Author: Rajiv Bakulesh Shah
 Requires-Python: >=3.7,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

