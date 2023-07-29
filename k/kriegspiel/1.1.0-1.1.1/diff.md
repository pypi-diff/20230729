# Comparing `tmp/kriegspiel-1.1.0.tar.gz` & `tmp/kriegspiel-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kriegspiel-1.1.0.tar", last modified: Wed Jul 26 03:20:06 2023, max compression
+gzip compressed data, was "kriegspiel-1.1.1.tar", last modified: Sat Jul 29 17:00:24 2023, max compression
```

## Comparing `kriegspiel-1.1.0.tar` & `kriegspiel-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.335423 kriegspiel-1.1.0/
--rw-r--r--   0 fil        (501) staff       (20)     1067 2022-02-05 22:22:30.000000 kriegspiel-1.1.0/LICENSE
--rw-r--r--   0 fil        (501) staff       (20)     1560 2023-07-26 03:20:06.335476 kriegspiel-1.1.0/PKG-INFO
--rw-r--r--   0 fil        (501) staff       (20)      936 2023-07-23 17:01:30.000000 kriegspiel-1.1.0/README.md
-drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.333923 kriegspiel-1.1.0/kriegspiel/
--rw-r--r--   0 fil        (501) staff       (20)      121 2023-07-26 03:18:38.000000 kriegspiel-1.1.0/kriegspiel/__init__.py
--rw-r--r--   0 fil        (501) staff       (20)    14642 2023-07-26 03:11:02.000000 kriegspiel-1.1.0/kriegspiel/berkeley.py
--rw-r--r--   0 fil        (501) staff       (20)    10639 2023-07-26 03:11:02.000000 kriegspiel-1.1.0/kriegspiel/move.py
-drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.334632 kriegspiel-1.1.0/kriegspiel.egg-info/
--rw-r--r--   0 fil        (501) staff       (20)     1560 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/PKG-INFO
--rw-r--r--   0 fil        (501) staff       (20)      312 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/SOURCES.txt
--rw-r--r--   0 fil        (501) staff       (20)        1 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/dependency_links.txt
--rw-r--r--   0 fil        (501) staff       (20)       28 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/requires.txt
--rw-r--r--   0 fil        (501) staff       (20)       11 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/top_level.txt
--rw-r--r--   0 fil        (501) staff       (20)      253 2023-07-26 03:20:06.335680 kriegspiel-1.1.0/setup.cfg
--rw-r--r--   0 fil        (501) staff       (20)     3730 2022-02-05 22:22:30.000000 kriegspiel-1.1.0/setup.py
-drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.335202 kriegspiel-1.1.0/tests/
--rw-r--r--   0 fil        (501) staff       (20)    36433 2023-07-26 03:10:24.000000 kriegspiel-1.1.0/tests/test_berkeley.py
--rw-r--r--   0 fil        (501) staff       (20)     4854 2023-07-26 03:10:24.000000 kriegspiel-1.1.0/tests/test_move.py
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-29 17:00:24.509569 kriegspiel-1.1.1/
+-rw-r--r--   0 fil        (501) staff       (20)     1067 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/LICENSE
+-rw-r--r--   0 fil        (501) staff       (20)     1570 2023-07-29 17:00:24.509620 kriegspiel-1.1.1/PKG-INFO
+-rw-r--r--   0 fil        (501) staff       (20)      936 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/README.md
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-29 17:00:24.508310 kriegspiel-1.1.1/kriegspiel/
+-rw-r--r--   0 fil        (501) staff       (20)      121 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/kriegspiel/__init__.py
+-rw-r--r--   0 fil        (501) staff       (20)    14642 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/kriegspiel/berkeley.py
+-rw-r--r--   0 fil        (501) staff       (20)    10639 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/kriegspiel/move.py
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-29 17:00:24.508891 kriegspiel-1.1.1/kriegspiel.egg-info/
+-rw-r--r--   0 fil        (501) staff       (20)     1570 2023-07-29 17:00:24.000000 kriegspiel-1.1.1/kriegspiel.egg-info/PKG-INFO
+-rw-r--r--   0 fil        (501) staff       (20)      285 2023-07-29 17:00:24.000000 kriegspiel-1.1.1/kriegspiel.egg-info/SOURCES.txt
+-rw-r--r--   0 fil        (501) staff       (20)        1 2023-07-29 17:00:24.000000 kriegspiel-1.1.1/kriegspiel.egg-info/dependency_links.txt
+-rw-r--r--   0 fil        (501) staff       (20)       11 2023-07-29 17:00:24.000000 kriegspiel-1.1.1/kriegspiel.egg-info/top_level.txt
+-rw-r--r--   0 fil        (501) staff       (20)      733 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/pyproject.toml
+-rw-r--r--   0 fil        (501) staff       (20)      253 2023-07-29 17:00:24.509837 kriegspiel-1.1.1/setup.cfg
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-29 17:00:24.509413 kriegspiel-1.1.1/tests/
+-rw-r--r--   0 fil        (501) staff       (20)    36433 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/tests/test_berkeley.py
+-rw-r--r--   0 fil        (501) staff       (20)     4854 2023-07-29 16:58:48.000000 kriegspiel-1.1.1/tests/test_move.py
```

### Comparing `kriegspiel-1.1.0/LICENSE` & `kriegspiel-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kriegspiel-1.1.0/PKG-INFO` & `kriegspiel-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: kriegspiel
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python Kriegspiel Game
-Home-page: https://github.com/Kriegspiel/ks-game
-Author: Alexander Filatov
-Author-email: alexander@kriegspiel.org
-License: MIT
-Keywords: kriegspiel chess variant
-Classifier: Development Status :: 4 - Beta
+Author-email: Fil <alexander@kriegspiel.org>
+Project-URL: Homepage, https://github.com/Kriegspiel/ks-game/
+Project-URL: Bug Tracker, https://github.com/Kriegspiel/ks-game/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Games/Entertainment
 Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: test
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Kriegspiel Game
 
 [![Build Status](https://travis-ci.org/Kriegspiel/ks-game.svg?branch=master)](https://travis-ci.org/Kriegspiel/ks-game)
 [![PyPI version](https://badge.fury.io/py/kriegspiel.svg)](https://badge.fury.io/py/kriegspiel)
 [![codecov](https://codecov.io/gh/Kriegspiel/ks-game/branch/master/graph/badge.svg)](https://codecov.io/gh/Kriegspiel/ks-game)
```

### Comparing `kriegspiel-1.1.0/README.md` & `kriegspiel-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kriegspiel-1.1.0/kriegspiel/berkeley.py` & `kriegspiel-1.1.1/kriegspiel/berkeley.py`

 * *Files identical despite different names*

### Comparing `kriegspiel-1.1.0/kriegspiel/move.py` & `kriegspiel-1.1.1/kriegspiel/move.py`

 * *Files identical despite different names*

### Comparing `kriegspiel-1.1.0/kriegspiel.egg-info/PKG-INFO` & `kriegspiel-1.1.1/kriegspiel.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: kriegspiel
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python Kriegspiel Game
-Home-page: https://github.com/Kriegspiel/ks-game
-Author: Alexander Filatov
-Author-email: alexander@kriegspiel.org
-License: MIT
-Keywords: kriegspiel chess variant
-Classifier: Development Status :: 4 - Beta
+Author-email: Fil <alexander@kriegspiel.org>
+Project-URL: Homepage, https://github.com/Kriegspiel/ks-game/
+Project-URL: Bug Tracker, https://github.com/Kriegspiel/ks-game/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Games/Entertainment
 Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: test
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Kriegspiel Game
 
 [![Build Status](https://travis-ci.org/Kriegspiel/ks-game.svg?branch=master)](https://travis-ci.org/Kriegspiel/ks-game)
 [![PyPI version](https://badge.fury.io/py/kriegspiel.svg)](https://badge.fury.io/py/kriegspiel)
 [![codecov](https://codecov.io/gh/Kriegspiel/ks-game/branch/master/graph/badge.svg)](https://codecov.io/gh/Kriegspiel/ks-game)
```

### Comparing `kriegspiel-1.1.0/tests/test_berkeley.py` & `kriegspiel-1.1.1/tests/test_berkeley.py`

 * *Files identical despite different names*

### Comparing `kriegspiel-1.1.0/tests/test_move.py` & `kriegspiel-1.1.1/tests/test_move.py`

 * *Files identical despite different names*

