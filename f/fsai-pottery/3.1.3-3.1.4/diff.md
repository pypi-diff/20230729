# Comparing `tmp/fsai_pottery-3.1.3.tar.gz` & `tmp/fsai_pottery-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsai_pottery-3.1.3.tar", max compression
+gzip compressed data, was "fsai_pottery-3.1.4.tar", max compression
```

## Comparing `fsai_pottery-3.1.3.tar` & `fsai_pottery-3.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11358 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/LICENSE
--rw-r--r--   0        0        0    33773 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/README.md
--rw-r--r--   0        0        0     4330 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/__init__.py
--rw-r--r--   0        0        0     6128 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/aionextid.py
--rw-r--r--   0        0        0    24162 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/aioredlock.py
--rw-r--r--   0        0        0     1705 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/annotations.py
--rw-r--r--   0        0        0    11408 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/base.py
--rw-r--r--   0        0        0    15338 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/bloom.py
--rw-r--r--   0        0        0    13808 2023-07-29 17:12:06.937767 fsai_pottery-3.1.3/pottery/cache.py
--rw-r--r--   0        0        0    10795 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/counter.py
--rw-r--r--   0        0        0     7840 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/deque.py
--rw-r--r--   0        0        0     6962 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/dict.py
--rw-r--r--   0        0        0     3021 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/exceptions.py
--rw-r--r--   0        0        0     3803 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/executor.py
--rw-r--r--   0        0        0     9265 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/hyper.py
--rw-r--r--   0        0        0    16529 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/list.py
--rw-r--r--   0        0        0     2864 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/monkey.py
--rw-r--r--   0        0        0    10485 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/nextid.py
--rw-r--r--   0        0        0        0 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/py.typed
--rw-r--r--   0        0        0     6103 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/queue.py
--rw-r--r--   0        0        0    28690 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/redlock.py
--rw-r--r--   0        0        0    11741 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/set.py
--rw-r--r--   0        0        0     4620 2023-07-29 17:12:06.941767 fsai_pottery-3.1.3/pottery/timer.py
--rw-r--r--   0        0        0     1447 2023-07-29 17:12:07.697758 fsai_pottery-3.1.3/pyproject.toml
--rw-r--r--   0        0        0    36304 1970-01-01 00:00:00.000000 fsai_pottery-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/LICENSE
+-rw-r--r--   0        0        0    33773 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/README.md
+-rw-r--r--   0        0        0     4330 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/__init__.py
+-rw-r--r--   0        0        0     6128 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/aionextid.py
+-rw-r--r--   0        0        0    24162 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/aioredlock.py
+-rw-r--r--   0        0        0     1705 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/annotations.py
+-rw-r--r--   0        0        0    11408 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/base.py
+-rw-r--r--   0        0        0    15338 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/bloom.py
+-rw-r--r--   0        0        0    13808 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/cache.py
+-rw-r--r--   0        0        0    10795 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/counter.py
+-rw-r--r--   0        0        0     7840 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/deque.py
+-rw-r--r--   0        0        0     6962 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/dict.py
+-rw-r--r--   0        0        0     3021 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/exceptions.py
+-rw-r--r--   0        0        0     3803 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/executor.py
+-rw-r--r--   0        0        0     9265 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/hyper.py
+-rw-r--r--   0        0        0    16529 2023-07-29 17:18:07.125935 fsai_pottery-3.1.4/pottery/list.py
+-rw-r--r--   0        0        0     2864 2023-07-29 17:18:07.129935 fsai_pottery-3.1.4/pottery/monkey.py
+-rw-r--r--   0        0        0    10485 2023-07-29 17:18:07.129935 fsai_pottery-3.1.4/pottery/nextid.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:18:07.129935 fsai_pottery-3.1.4/pottery/py.typed
+-rw-r--r--   0        0        0     6103 2023-07-29 17:18:07.129935 fsai_pottery-3.1.4/pottery/queue.py
+-rw-r--r--   0        0        0    28690 2023-07-29 17:18:07.129935 fsai_pottery-3.1.4/pottery/redlock.py
+-rw-r--r--   0        0        0    11741 2023-07-29 17:18:07.129935 fsai_pottery-3.1.4/pottery/set.py
+-rw-r--r--   0        0        0     4620 2023-07-29 17:18:07.129935 fsai_pottery-3.1.4/pottery/timer.py
+-rw-r--r--   0        0        0     1501 2023-07-29 17:18:07.729942 fsai_pottery-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0    36685 1970-01-01 00:00:00.000000 fsai_pottery-3.1.4/PKG-INFO
```

### Comparing `fsai_pottery-3.1.3/LICENSE` & `fsai_pottery-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/README.md` & `fsai_pottery-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/__init__.py` & `fsai_pottery-3.1.4/pottery/__init__.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/aionextid.py` & `fsai_pottery-3.1.4/pottery/aionextid.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/aioredlock.py` & `fsai_pottery-3.1.4/pottery/aioredlock.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/annotations.py` & `fsai_pottery-3.1.4/pottery/annotations.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/base.py` & `fsai_pottery-3.1.4/pottery/base.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/bloom.py` & `fsai_pottery-3.1.4/pottery/bloom.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/cache.py` & `fsai_pottery-3.1.4/pottery/cache.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/counter.py` & `fsai_pottery-3.1.4/pottery/counter.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/deque.py` & `fsai_pottery-3.1.4/pottery/deque.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/dict.py` & `fsai_pottery-3.1.4/pottery/dict.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/exceptions.py` & `fsai_pottery-3.1.4/pottery/exceptions.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/executor.py` & `fsai_pottery-3.1.4/pottery/executor.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/hyper.py` & `fsai_pottery-3.1.4/pottery/hyper.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/list.py` & `fsai_pottery-3.1.4/pottery/list.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/monkey.py` & `fsai_pottery-3.1.4/pottery/monkey.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/nextid.py` & `fsai_pottery-3.1.4/pottery/nextid.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/queue.py` & `fsai_pottery-3.1.4/pottery/queue.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/redlock.py` & `fsai_pottery-3.1.4/pottery/redlock.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/set.py` & `fsai_pottery-3.1.4/pottery/set.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/pottery/timer.py` & `fsai_pottery-3.1.4/pottery/timer.py`

 * *Files identical despite different names*

### Comparing `fsai_pottery-3.1.3/PKG-INFO` & `fsai_pottery-3.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: fsai-pottery
-Version: 3.1.3
+Version: 3.1.4
 Summary: Redis for humans. 🌎🌍🌏
 License: Apache License
 Author: Rajiv Bakulesh Shah
 Requires-Python: >=3.7,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: async-timeout (==4.0.2)
-Requires-Dist: attrs (==21.4.0)
-Requires-Dist: bandit (==1.7.4)
-Requires-Dist: bleach (==4.1.0)
-Requires-Dist: certifi (==2021.10.8)
-Requires-Dist: charset-normalizer (==2.0.12)
-Requires-Dist: click (==8.0.4)
-Requires-Dist: colorama (==0.4.4)
-Requires-Dist: coverage (==6.3.2)
-Requires-Dist: deprecated (==1.2.13)
-Requires-Dist: docutils (==0.18.1)
-Requires-Dist: dparse (==0.5.1)
-Requires-Dist: flake8 (==4.0.1)
-Requires-Dist: gitdb (==4.0.9)
-Requires-Dist: gitpython (==3.1.27)
+Requires-Dist: async-timeout (>=4.0.2,<5.0.0)
+Requires-Dist: attrs (>=21.4.0,<22.0.0)
+Requires-Dist: bandit (>=1.7.4,<2.0.0)
+Requires-Dist: bleach (>=4.1.0,<5.0.0)
+Requires-Dist: certifi (>=2021.10.8,<2022.0.0)
+Requires-Dist: charset-normalizer (>=2.0.12,<3.0.0)
+Requires-Dist: click (>=8.0.4,<9.0.0)
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
+Requires-Dist: coverage (>=6.3.2,<7.0.0)
+Requires-Dist: deprecated (>=1.2.13,<2.0.0)
+Requires-Dist: docutils (>=0.18.1,<0.19.0)
+Requires-Dist: dparse (>=0.5.1,<0.6.0)
+Requires-Dist: flake8 (>=4.0.1,<5.0.0)
+Requires-Dist: gitdb (>=4.0.9,<5.0.0)
+Requires-Dist: gitpython (>=3.1.27,<4.0.0)
 Requires-Dist: hiredis (>=2.0.0,<3.0.0)
-Requires-Dist: idna (==3.3)
-Requires-Dist: importlib-metadata (==4.2.0)
-Requires-Dist: iniconfig (==1.1.1)
-Requires-Dist: isort (==5.10.1)
-Requires-Dist: keyring (==23.5.0)
-Requires-Dist: mccabe (==0.6.1)
-Requires-Dist: mmh3 (==3.0.0)
-Requires-Dist: mypy (==0.941)
-Requires-Dist: mypy-extensions (==0.4.3)
-Requires-Dist: packaging (==21.3)
-Requires-Dist: pbr (==5.8.1)
-Requires-Dist: pkginfo (==1.8.2)
-Requires-Dist: pluggy (==1.0.0)
-Requires-Dist: py (==1.11.0)
-Requires-Dist: pycodestyle (==2.8.0)
-Requires-Dist: pyflakes (==2.4.0)
-Requires-Dist: pygments (==2.11.2)
-Requires-Dist: pyparsing (==3.0.7)
-Requires-Dist: pytest (==7.1.0)
-Requires-Dist: pytest-asyncio (==0.18.2)
-Requires-Dist: pytest-cov (==3.0.0)
-Requires-Dist: pyyaml (==6.0)
-Requires-Dist: readme-renderer (==34.0)
+Requires-Dist: idna (>=3.3,<4.0)
+Requires-Dist: importlib-metadata (>=4.2.0,<5.0.0)
+Requires-Dist: iniconfig (>=1.1.1,<2.0.0)
+Requires-Dist: isort (>=5.10.1,<6.0.0)
+Requires-Dist: keyring (>=23.5.0,<24.0.0)
+Requires-Dist: mccabe (>=0.6.1,<0.7.0)
+Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
+Requires-Dist: mypy (>=0.941,<0.942)
+Requires-Dist: mypy-extensions (>=0.4.3,<0.5.0)
+Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: pbr (>=5.8.1,<6.0.0)
+Requires-Dist: pkginfo (>=1.8.2,<2.0.0)
+Requires-Dist: pluggy (>=1.0.0,<2.0.0)
+Requires-Dist: py (>=1.11.0,<2.0.0)
+Requires-Dist: pycodestyle (>=2.8.0,<3.0.0)
+Requires-Dist: pyflakes (>=2.4.0,<3.0.0)
+Requires-Dist: pygments (>=2.11.2,<3.0.0)
+Requires-Dist: pyparsing (>=3.0.7,<4.0.0)
+Requires-Dist: pytest (>=7.1.0,<8.0.0)
+Requires-Dist: pytest-asyncio (>=0.18.2,<0.19.0)
+Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: readme-renderer (>=34.0,<35.0)
 Requires-Dist: redis (>=4.2.2,<5.0.0)
-Requires-Dist: requests (==2.27.1)
-Requires-Dist: requests-toolbelt (==0.9.1)
-Requires-Dist: rfc3986 (==2.0.0)
-Requires-Dist: safety (==1.10.3)
-Requires-Dist: six (==1.16.0)
-Requires-Dist: smmap (==5.0.0)
-Requires-Dist: stevedore (==3.5.0)
-Requires-Dist: toml (==0.10.2)
-Requires-Dist: tomli (==2.0.1)
-Requires-Dist: tqdm (==4.63.0)
-Requires-Dist: twine (==3.8.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
+Requires-Dist: rfc3986 (>=2.0.0,<3.0.0)
+Requires-Dist: safety (>=1.10.3,<2.0.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: smmap (>=5.0.0,<6.0.0)
+Requires-Dist: stevedore (>=3.5.0,<4.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: tqdm (>=4.63.0,<5.0.0)
+Requires-Dist: twine (>=3.8.0,<4.0.0)
 Requires-Dist: types-redis (>=4.1.17,<5.0.0)
-Requires-Dist: typing-extensions (==4.1.1)
-Requires-Dist: urllib3 (==1.26.8)
-Requires-Dist: webencodings (==0.5.1)
-Requires-Dist: wrapt (==1.14.0)
-Requires-Dist: zipp (==3.7.0)
+Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
+Requires-Dist: urllib3 (>=1.26.8,<2.0.0)
+Requires-Dist: webencodings (>=0.5.1,<0.6.0)
+Requires-Dist: wrapt (>=1.14.0,<2.0.0)
+Requires-Dist: zipp (>=3.7.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Pottery: Redis for Humans 🌎🌍🌏
 
 [Redis](http://redis.io/) is awesome, but [Redis
 commands](http://redis.io/commands) are not always intuitive.  Pottery is a
 Pythonic way to access Redis.  If you know how to use Python dicts, then you
```

