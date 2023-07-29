# Comparing `tmp/collatz-1.0.0.tar.gz` & `tmp/collatz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collatz-1.0.0.tar", last modified: Sat Apr  9 16:22:08 2022, max compression
+gzip compressed data, was "collatz-1.0.1.tar", last modified: Sat Jul 29 18:59:56 2023, max compression
```

## Comparing `collatz-1.0.0.tar` & `collatz-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 16:22:08.648273 collatz-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-09 16:22:01.000000 collatz-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-09 16:21:44.000000 collatz-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4932 2022-04-09 16:22:08.648273 collatz-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-04-09 16:21:44.000000 collatz-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-04-09 16:21:44.000000 collatz-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-04-09 16:22:08.648273 collatz-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-04-09 16:21:44.000000 collatz-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 16:22:08.648273 collatz-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 16:22:08.648273 collatz-1.0.0/src/collatz/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-04-09 16:21:44.000000 collatz-1.0.0/src/collatz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-09 16:21:44.000000 collatz-1.0.0/src/collatz/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14359 2022-04-09 16:21:44.000000 collatz-1.0.0/src/collatz/parameterised.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 16:22:08.648273 collatz-1.0.0/src/collatz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4932 2022-04-09 16:22:07.000000 collatz-1.0.0/src/collatz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-04-09 16:22:08.000000 collatz-1.0.0/src/collatz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-09 16:22:08.000000 collatz-1.0.0/src/collatz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-09 16:22:08.000000 collatz-1.0.0/src/collatz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-09 16:22:08.648273 collatz-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-09 16:21:44.000000 collatz-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13172 2022-04-09 16:21:44.000000 collatz-1.0.0/tests/test_parameterised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:56.838818 collatz-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:56.838818 collatz-1.0.1/.demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 18:59:14.000000 collatz-1.0.1/.demo/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-29 18:59:14.000000 collatz-1.0.1/.demo/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:56.838818 collatz-1.0.1/.demo/_/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 18:59:14.000000 collatz-1.0.1/.demo/_/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-29 18:59:14.000000 collatz-1.0.1/.demo/_/hailstone_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-29 18:59:14.000000 collatz-1.0.1/.demo/_/reverse_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-29 18:59:14.000000 collatz-1.0.1/.demo/_/stopping_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-29 18:59:14.000000 collatz-1.0.1/.demo/_/tree_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-29 18:59:14.000000 collatz-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-29 18:59:14.000000 collatz-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-29 18:59:56.838818 collatz-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-29 18:59:14.000000 collatz-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-29 18:59:14.000000 collatz-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 18:59:56.838818 collatz-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-29 18:59:14.000000 collatz-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:56.834818 collatz-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:56.838818 collatz-1.0.1/src/collatz/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-29 18:59:14.000000 collatz-1.0.1/src/collatz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 18:59:14.000000 collatz-1.0.1/src/collatz/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-07-29 18:59:14.000000 collatz-1.0.1/src/collatz/parameterised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:56.838818 collatz-1.0.1/src/collatz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-29 18:59:56.000000 collatz-1.0.1/src/collatz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-29 18:59:56.000000 collatz-1.0.1/src/collatz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:59:56.000000 collatz-1.0.1/src/collatz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-29 18:59:56.000000 collatz-1.0.1/src/collatz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:56.838818 collatz-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 18:59:14.000000 collatz-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-07-29 18:59:14.000000 collatz-1.0.1/tests/test_parameterised.py
```

### Comparing `collatz-1.0.0/LICENSE` & `collatz-1.0.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2022 Nathan Levett
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `collatz-1.0.0/PKG-INFO` & `collatz-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 Metadata-Version: 2.1
 Name: collatz
-Version: 1.0.0
+Version: 1.0.1
 Summary: Enabling experimenting with functions related to or involved in the Collatz conjecture.
 Home-page: https://github.com/Skenvy/Collatz
 Author: Skenvy
 Author-email: nathan.a.z.levett@gmail.com
-License: UNKNOWN
+License: Apache Software License
 Project-URL: Bug Tracker, https://github.com/Skenvy/Collatz/issues
-Platform: UNKNOWN
+Keywords: Collatz,Ulam,Kakutani's,Thwaites,Hasse's,Syracus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [Collatz](https://github.com/Skenvy/Collatz): [Python](https://github.com/Skenvy/Collatz/tree/main/python)
-Functions related to [the Collatz/Syracuse/3N+1 problem](https://en.wikipedia.org/wiki/Collatz_conjecture), implemented in Python.
+# [Collatz](https://github.com/Skenvy/Collatz): [Python](https://github.com/Skenvy/Collatz/tree/main/python) 🐍🐍🐍
+Functions related to [the Collatz/Syracuse/3N+1 problem](https://en.wikipedia.org/wiki/Collatz_conjecture), implemented in [Python](https://www.python.org/).
 ## Getting Started
-To [install the latest](https://pypi.org/project/collatz/);
-```
+[To install the latest from pypi](https://pypi.org/project/collatz/);
+```sh
 pip install collatz
 ```
-### Developing
-#### The first time virtual env
-```
-git clone https://github.com/Skenvy/Collatz.git
-cd Collatz/python
-make venv
-```
-#### Iterative development
-`make build` will test and build the wheel and force reinstall it into the local venv, to test the built distribution
 ## Usage
 Provides the basic functionality to interact with the Collatz conjecture.
 The parameterisation uses the same `(P,a,b)` notation as Conway's generalisations.
 Besides the function and reverse function, there is also functionality to retrieve the hailstone sequence, the "stopping time"/"total stopping time", or tree-graph. 
 The only restriction placed on parameters is that both `P` and `a` can't be `0`.
 ### collatz.function(~)
 `(n:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # The default "Collatz function"
 >>> collatz.function(5)
 16
 >>> # Alternatively, you can parameterise the function.
 >>> collatz.function(5, P=7, a=5, b=17)
 42
 ```
 ### collatz.reverse_function(~)
 `(n:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # Get the list of values that return the input.
 >>> collatz.reverse_function(4)
 [1, 8]
 >>> # Alternatively, you can parameterise the reverse_function.
 >>> collatz.reverse_function(5, P=5, a=2, b=3)
 [1, 25]
 ```
 ### collatz.hailstone_sequence(~)
 `(initial_value:int, P:int=2,  a:int=3, b:int=1, max_total_stopping_time:int=1000, total_stopping_time:bool=True, verbose:bool=True)`
-```
+```python
 >>> import collatz
 >>> # Get the sequence of values forming the hailstone from an initial value
 >>> collatz.hailstone_sequence(10)
 [10, 5, 16, 8, 4, 2, 1, ['TOTAL_STOPPING_TIME', 6]]
 >>> # Determines if it's in a cycle
 >>> collatz.hailstone_sequence(-56)
 [-56, -28, 'CYCLE_INIT', [-14, -7, -20, -10, -5], ['CYCLE_LENGTH', 5]]
@@ -73,15 +65,15 @@
 [-200, -100, -50, -25, -74, -37, -110, -55, -164, -82, -41, -122, -61, -182, -91, -272, -136, -68, -34, -17, -50]
 >>> # Although hailstones typically go to the "total stop" of 1, they can be set to terminate on the regular stop
 >>> collatz.hailstone_sequence(5, total_stopping_time=False)
 [5, 16, 8, 4, ['STOPPING_TIME', 3]]
 ```
 ### collatz.stopping_time(~)
 `(initial_value:int, P:int=2, a:int=3, b:int=1, max_stopping_time:int=1000, total_stopping_time:bool=False)`
-```
+```python
 >>> import collatz
 >>> # Reports the stopping time, the amount of iterations of the function to reach a value lower than the initial value.
 >>> collatz.stopping_time(5)
 3
 >>> # Can be used to find the "total stopping time" as well, the amount of iterations to reach "1"
 >>> collatz.stopping_time(5, total_stopping_time=True)
 5
@@ -93,20 +85,27 @@
 inf
 >>> # If it overruns maximum stopping time, returns nothing.
 >>> collatz.stopping_time(5, max_stopping_time=-1)
 >>> # <None>
 ```
 ### collatz.tree_graph(~)
 `(initial_value:int, max_orbit_distance:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # See the tree graph built by a reverse function traversal, to the depth specified by max_orbit_distance.
 >>> collatz.tree_graph(1, 3)
 {1: {2: {4: {'CYCLE_INIT': 1, 8: {}}}}}
 >>> collatz.tree_graph(1, 12)
 {1: {2: {4: {'CYCLE_INIT': 1, 8: {16: {5: {10: {3: {6: {12: {24: {48: {96: {}}}}}}, 20: {40: {13: {26: {52: {17: {}, 104: {}}}}, 80: {160: {53: {106: {}}, 320: {640: {}}}}}}}}, 32: {64: {21: {42: {84: {168: {336: {672: {}}}}}}, 128: {256: {85: {170: {340: {113: {}, 680: {}}}}, 512: {1024: {341: {682: {}}, 2048: {4096: {}}}}}}}}}}}}}}
 >>> # Can also be parameterised;
 >>> collatz.tree_graph(1, 2, P=5, a=2, b=3)
 {1: {-1: {-5: {}, -2: {}}, 5: {'CYCLE_INIT': 1, 25: {}}}}
 ```
-
-
+## [Sphinx+MyST generated docs](https://skenvy.github.io/Collatz/python/)
+## Developing
+### The first time setup
+```
+git clone https://github.com/Skenvy/Collatz.git && cd Collatz/python && make venv
+```
+### Iterative development
+* `make build` will test and build the wheel and force reinstall it into the local venv, to test the built distribution
+## [Open Source Insights](https://deps.dev/pypi/collatz)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `collatz-1.0.0/README.md` & `collatz-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,44 @@
-# [Collatz](https://github.com/Skenvy/Collatz): [Python](https://github.com/Skenvy/Collatz/tree/main/python)
-Functions related to [the Collatz/Syracuse/3N+1 problem](https://en.wikipedia.org/wiki/Collatz_conjecture), implemented in Python.
+# [Collatz](https://github.com/Skenvy/Collatz): [Python](https://github.com/Skenvy/Collatz/tree/main/python) 🐍🐍🐍
+Functions related to [the Collatz/Syracuse/3N+1 problem](https://en.wikipedia.org/wiki/Collatz_conjecture), implemented in [Python](https://www.python.org/).
 ## Getting Started
-To [install the latest](https://pypi.org/project/collatz/);
-```
+[To install the latest from pypi](https://pypi.org/project/collatz/);
+```sh
 pip install collatz
 ```
-### Developing
-#### The first time virtual env
-```
-git clone https://github.com/Skenvy/Collatz.git
-cd Collatz/python
-make venv
-```
-#### Iterative development
-`make build` will test and build the wheel and force reinstall it into the local venv, to test the built distribution
 ## Usage
 Provides the basic functionality to interact with the Collatz conjecture.
 The parameterisation uses the same `(P,a,b)` notation as Conway's generalisations.
 Besides the function and reverse function, there is also functionality to retrieve the hailstone sequence, the "stopping time"/"total stopping time", or tree-graph. 
 The only restriction placed on parameters is that both `P` and `a` can't be `0`.
 ### collatz.function(~)
 `(n:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # The default "Collatz function"
 >>> collatz.function(5)
 16
 >>> # Alternatively, you can parameterise the function.
 >>> collatz.function(5, P=7, a=5, b=17)
 42
 ```
 ### collatz.reverse_function(~)
 `(n:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # Get the list of values that return the input.
 >>> collatz.reverse_function(4)
 [1, 8]
 >>> # Alternatively, you can parameterise the reverse_function.
 >>> collatz.reverse_function(5, P=5, a=2, b=3)
 [1, 25]
 ```
 ### collatz.hailstone_sequence(~)
 `(initial_value:int, P:int=2,  a:int=3, b:int=1, max_total_stopping_time:int=1000, total_stopping_time:bool=True, verbose:bool=True)`
-```
+```python
 >>> import collatz
 >>> # Get the sequence of values forming the hailstone from an initial value
 >>> collatz.hailstone_sequence(10)
 [10, 5, 16, 8, 4, 2, 1, ['TOTAL_STOPPING_TIME', 6]]
 >>> # Determines if it's in a cycle
 >>> collatz.hailstone_sequence(-56)
 [-56, -28, 'CYCLE_INIT', [-14, -7, -20, -10, -5], ['CYCLE_LENGTH', 5]]
@@ -56,15 +47,15 @@
 [-200, -100, -50, -25, -74, -37, -110, -55, -164, -82, -41, -122, -61, -182, -91, -272, -136, -68, -34, -17, -50]
 >>> # Although hailstones typically go to the "total stop" of 1, they can be set to terminate on the regular stop
 >>> collatz.hailstone_sequence(5, total_stopping_time=False)
 [5, 16, 8, 4, ['STOPPING_TIME', 3]]
 ```
 ### collatz.stopping_time(~)
 `(initial_value:int, P:int=2, a:int=3, b:int=1, max_stopping_time:int=1000, total_stopping_time:bool=False)`
-```
+```python
 >>> import collatz
 >>> # Reports the stopping time, the amount of iterations of the function to reach a value lower than the initial value.
 >>> collatz.stopping_time(5)
 3
 >>> # Can be used to find the "total stopping time" as well, the amount of iterations to reach "1"
 >>> collatz.stopping_time(5, total_stopping_time=True)
 5
@@ -76,18 +67,27 @@
 inf
 >>> # If it overruns maximum stopping time, returns nothing.
 >>> collatz.stopping_time(5, max_stopping_time=-1)
 >>> # <None>
 ```
 ### collatz.tree_graph(~)
 `(initial_value:int, max_orbit_distance:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # See the tree graph built by a reverse function traversal, to the depth specified by max_orbit_distance.
 >>> collatz.tree_graph(1, 3)
 {1: {2: {4: {'CYCLE_INIT': 1, 8: {}}}}}
 >>> collatz.tree_graph(1, 12)
 {1: {2: {4: {'CYCLE_INIT': 1, 8: {16: {5: {10: {3: {6: {12: {24: {48: {96: {}}}}}}, 20: {40: {13: {26: {52: {17: {}, 104: {}}}}, 80: {160: {53: {106: {}}, 320: {640: {}}}}}}}}, 32: {64: {21: {42: {84: {168: {336: {672: {}}}}}}, 128: {256: {85: {170: {340: {113: {}, 680: {}}}}, 512: {1024: {341: {682: {}}, 2048: {4096: {}}}}}}}}}}}}}}
 >>> # Can also be parameterised;
 >>> collatz.tree_graph(1, 2, P=5, a=2, b=3)
 {1: {-1: {-5: {}, -2: {}}, 5: {'CYCLE_INIT': 1, 25: {}}}}
 ```
+## [Sphinx+MyST generated docs](https://skenvy.github.io/Collatz/python/)
+## Developing
+### The first time setup
+```
+git clone https://github.com/Skenvy/Collatz.git && cd Collatz/python && make venv
+```
+### Iterative development
+* `make build` will test and build the wheel and force reinstall it into the local venv, to test the built distribution
+## [Open Source Insights](https://deps.dev/pypi/collatz)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `collatz-1.0.0/setup.cfg` & `collatz-1.0.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 [metadata]
 name = collatz
 author = Skenvy
 author_email = nathan.a.z.levett@gmail.com
 description = Enabling experimenting with functions related to or involved in the Collatz conjecture.
 long_description = file: README.md
 long_description_content_type = text/markdown
+license = Apache Software License
 url = https://github.com/Skenvy/Collatz
 project_urls = 
 	Bug Tracker = https://github.com/Skenvy/Collatz/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
+	Topic :: Scientific/Engineering :: Mathematics
+keywords = 
+	Collatz
+	Ulam
+	Kakutani's
+	Thwaites
+	Hasse's
+	Syracus
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
```

### Comparing `collatz-1.0.0/src/collatz/parameterised.py` & `collatz-1.0.1/src/collatz/parameterised.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-from enum import Enum
-from typing import Optional, Set
-from math import inf as infinity
-
-
 """
 Provides the basic functionality to interact with the Collatz conjecture.
 The parameterisation uses the same (P,a,b) notation as Conway's generalisations.
 Besides the function and reverse function, there is also functionality to
 retrieve the hailstone sequence, the "stopping time"/"total stopping time", or
 tree-graph.
 """
 
+from enum import Enum
+from typing import Optional, Set
+from math import inf as infinity
+
 
-_KNOWN_CYCLES = [[1, 4, 2], [-1, -2], [-5, -14, -7, -20, -10], 
-[-17,-50,-25,-74,-37,-110,-55,-164,-82,-41,-122,-61,-182,-91,-272,-136,-68,-34]]
+# The four known cycles for the standard parameterisation.
+_KNOWN_CYCLES = [[1, 4, 2], [-1, -2], [-5, -14, -7, -20, -10],
+                 [-17, -50, -25, -74, -37, -110, -55, -164, -82,
+                  -41, -122, -61, -182, -91, -272, -136, -68, -34]]
+# The current value up to which the standard parameterisation has been verified.
 __VERIFIED_MAXIMUM = 295147905179352825856
-__VERIFIED_MINIMUM = -272  #TODO: Check the actual lowest bound.
+# The current value down to which the standard parameterisation has been verified.
+__VERIFIED_MINIMUM = -272  # TODO: Check the actual lowest bound.
 
 
-"""
-Error message constant.
-"""
 class _ErrMsg(Enum):
+    """
+    Error message constant.
+    """
     SANE_PARAMS_P = "'P' should not be 0 ~ violates modulo being non-zero."
     SANE_PARAMS_A = "'a' should not be 0 ~ violates the reversability."
 
 
-"""
-Cycle Control: Descriptive flags to indicate when some event occurs in the
-hailstone sequences, when set to verbose, or stopping time check.
-"""
 class _CC(Enum):
+    """
+    Cycle Control: Descriptive flags to indicate when some event occurs in the
+    hailstone sequences, when set to verbose, or stopping time check.
+    """
     STOPPING_TIME = 'STOPPING_TIME'
     TOTAL_STOPPING_TIME = 'TOTAL_STOPPING_TIME'
     CYCLE_INIT = 'CYCLE_INIT'
     CYCLE_LENGTH = 'CYCLE_LENGTH'
     MAX_STOP_OOB = 'MAX_STOP_OOB'  # ~ "out of bounds"
     ZERO_STOP = 'ZERO_STOP'
 
 
-def __assert_sane_parameterisation(P:int, a:int, b:int):
+def __assert_sane_parameterisation(P: int, a: int, _: int):
     """
     Handles the sanity check for the parameterisation (P,a,b) required by both
     the function and reverse function.
 
     Args:
         P (int): Modulus used to devide n, iff n is equivalent to (0 mod P).
         a (int): Factor by which to multiply n.
@@ -62,103 +65,103 @@
     # "b" being zero would cause behaviour not consistant with the collatz
     # function, but would not violate the reversability, so no check either.
     # " != 0" is redundant for python assertions.
     assert P, _ErrMsg.SANE_PARAMS_P.value
     assert a, _ErrMsg.SANE_PARAMS_A.value
 
 
-def function(n:int, P:int=2, a:int=3, b:int=1):
+def function(n: int, P: int = 2, a: int = 3, b: int = 1):
     """
     Returns the output of a single application of a Collatz-esque function.
 
     Args:
         n (int): The value on which to perform the Collatz-esque function
-    
-    Kwargs:
+
+    Keyword Args:
         P (int): Modulus used to devide n, iff n is equivalent to (0 mod P).
             Default is 2.
         a (int): Factor by which to multiply n. Default is 3.
         b (int): Value to add to the scaled value of n. Default is 1.
     """
-    __assert_sane_parameterisation(P,a,b)
-    return n//P if n%P == 0 else (a*n+b)
+    __assert_sane_parameterisation(P, a, b)
+    return n//P if n % P == 0 else (a*n+b)
 
 
-def reverse_function(n:int, P:int=2, a:int=3, b:int=1):
+def reverse_function(n: int, P: int = 2, a: int = 3, b: int = 1):
     """
     Returns the output of a single application of a Collatz-esque reverse
     function.
 
     Args:
         n (int): The value on which to perform the reverse Collatz function
-    
-    Kwargs:
-        P (int): Modulus used to devide n, iff n is equivalent to (0 mod P)
+
+    Keyword Args:
+        P (int): Modulus used to devide n, iff n is equivalent to (0 mod P).
             Default is 2.
         a (int): Factor by which to multiply n. Default is 3.
         b (int): Value to add to the scaled value of n. Default is 1.
     """
-    __assert_sane_parameterisation(P,a,b)
+    __assert_sane_parameterisation(P, a, b)
     # Every input can be reversed as the result of "n/P" division, which yields
     # "Pn"... {f(n) = an + b}≡{(f(n) - b)/a = n} ~ if n was such that the
     # muliplication step was taken instead of the division by the modulus, then
     # (f(n) - b)/a) must be an integer that is not in (0 mod P). Because we're
     # not placing restrictions on the parameters yet, although there is a better
     # way of shortcutting this for the default variables, we need to always
     # attempt (f(n) - b)/a)
     pre_values = [P*n]
-    if (n-b)%a == 0 and (n-b)%(P*a) != 0:
+    if (n-b) % a == 0 and (n-b) % (P*a) != 0:
         pre_values += [(n-b)//a]
         pre_values.sort()
     return pre_values
 
 
-def __initial_value_outside_verified_range(x:int):
+def __initial_value_outside_verified_range(x: int):
     """
     Checks if the initial value is greater than __VERIFIED_MAXIMUM or less than
     __VERIFIED_MINIMUM. Only intended for the default parameterisation.
 
     Args:
         x (int): The initial value to check if it is within range or not.
     """
     return (__VERIFIED_MAXIMUM < x) or (x < __VERIFIED_MINIMUM)
 
 
-def __stopping_time_terminus(n:int, total_stop:bool):
+def __stopping_time_terminus(n: int, total_stop: bool):
     """
     Provides the appropriate lambda to use to check if iterations on an initial
     value have reached either the stopping time, or total stopping time.
 
     Args:
         n (int): The initial value to confirm against a stopping time check.
         total_stop (bool): If false, the lambda will confirm that iterations
             of n have reached the oriented stopping time to reach a value closer
             to 0. If true, the lambda will simply check equality to 1.
     """
-    return (lambda x: x == 1) if total_stop else ((lambda x: x < n and x > 0)
-                                   if n >= 0 else (lambda x: x > n and x < 0))
+    return (lambda x: x == 1) if total_stop else (
+        (lambda x: x < n and x > 0) if n >= 0 else (lambda x: x > n and x < 0))
 
 
-def hailstone_sequence(initial_value:int, P:int=2, a:int=3,
-                       b:int=1, max_total_stopping_time:int=1000,
-                       total_stopping_time:bool=True, verbose:bool=True):
+def hailstone_sequence(initial_value: int, P: int = 2, a: int = 3,
+                       b: int = 1, max_total_stopping_time: int = 1000,
+                       total_stopping_time: bool = True, verbose: bool = True):
     """
     Returns a list of successive values obtained by iterating a Collatz-esque
     function, until either 1 is reached, or the total amount of iterations
     exceeds max_total_stopping_time, unless total_stopping_time is False,
     which will terminate the hailstone at the "stopping time" value, i.e. the
     first value less than the initial value. While the sequence has the
     capability to determine that it has encountered a cycle, the cycle from "1"
     wont be attempted or reported as part of a cycle, regardless of default or
     custom parameterisation, as "1" is considered a "total stop".
 
     Args:
         initial_value (int): The value to begin the hailstone sequence from.
-    
-    Kwargs:
+
+    Keyword Args:
         P (int): Modulus used to devide n, iff n is equivalent to (0 mod P)
             Default is 2.
         a (int): Factor by which to multiply n. Default is 3.
         b (int): Value to add to the scaled value of n. Default is 1.
         max_total_stopping_time (int): Maximum amount of times to iterate the
             function, if 1 is not reached. Default is 1000.
         total_stopping_time (bool): Whether or not to execute until the "total"
@@ -167,45 +170,48 @@
             than the initial value). Default is True.
         verbose (bool): If set to verbose, the hailstone sequence will include
             control string sequences to provide information about how the
             sequence terminated, whether by reaching a stopping time or entering
             a cycle. Default is True.
     """
     # Call out the function before any magic returns to trap bad values.
-    _ = function(initial_value,P=P,a=a,b=b)
+    _ = function(initial_value, P=P, a=a, b=b)
     # 0 is always an immediate stop.
     if initial_value == 0:
         return [[_CC.ZERO_STOP.value, 0]] if verbose else [0]
     # 1 is always an immediate stop, with 0 stopping time.
     if initial_value == 1:
         return [[_CC.TOTAL_STOPPING_TIME.value, 0]] if verbose else [1]
     terminate = __stopping_time_terminus(initial_value, total_stopping_time)
     # Start the hailstone sequence.
     _max_total_stopping_time = max(max_total_stopping_time, 1)
     hailstone = [initial_value]
     cyclic = (lambda x: x in hailstone)
-    for k in range(_max_total_stopping_time):
-        _next = function(hailstone[-1],P=P,a=a,b=b)
+    for _ in range(_max_total_stopping_time):
+        _next = function(hailstone[-1], P=P, a=a, b=b)
         # Check if the next hailstone is either the stopping time, total
         # stopping time, the same as the initial value, or stuck at zero.
         if terminate(_next):
             hailstone += [_next]
             if verbose:
                 m = _CC.TOTAL_STOPPING_TIME if _next == 1 else _CC.STOPPING_TIME
                 hailstone += [[m.value, len(hailstone)-1]]
             break
         if cyclic(_next):
             cycle_init = 1
-            for j in range(1,len(hailstone)+1):
+            for j in range(1, len(hailstone)+1):
                 if hailstone[-j] == _next:
                     cycle_init = j
                     break
             if verbose:
-                hailstone = hailstone[:-cycle_init] + [_CC.CYCLE_INIT.value,
-                    hailstone[-cycle_init:],[_CC.CYCLE_LENGTH.value,cycle_init]]
+                hailstone = hailstone[:-cycle_init] + [
+                    _CC.CYCLE_INIT.value,
+                    hailstone[-cycle_init:],
+                    [_CC.CYCLE_LENGTH.value, cycle_init]
+                ]
             else:
                 hailstone += [_next]
             break
         if _next == 0:
             hailstone += [0]
             if verbose:
                 hailstone += [[_CC.ZERO_STOP.value, -(len(hailstone)-1)]]
@@ -213,32 +219,32 @@
         hailstone += [_next]
     else:
         if verbose:
             hailstone += [[_CC.MAX_STOP_OOB.value, _max_total_stopping_time]]
     return hailstone
 
 
-def stopping_time(initial_value:int, P:int=2, a:int=3,
-                  b:int=1, max_stopping_time:int=1000,
-                  total_stopping_time:bool=False):
+def stopping_time(initial_value: int, P: int = 2, a: int = 3,
+                  b: int = 1, max_stopping_time: int = 1000,
+                  total_stopping_time: bool = False):
     """
     Returns the stopping time, the amount of iterations required to reach a
     value less than the initial value, or None if max_stopping_time is exceeded.
     Alternatively, if total_stopping_time is True, then it will instead count
     the amount of iterations to reach 1. If the sequence does not stop, but
     instead ends in a cycle, the result will be (math.inf). If (P,a,b) are such
     that it is possible to get stuck on zero, the result will be the negative of
     what would otherwise be the "total stopping time" to reach 1, where 0 is
     considered a "total stop" that should not occur as it does form a cycle of
     length 1.
 
     Args:
         initial_value (int): The value for which to find the stopping time.
-    
-    Kwargs:
+
+    Keyword Args:
         P (int): Modulus used to devide n, iff n is equivalent to (0 mod P)
             Default is 2.
         a (int): Factor by which to multiply n. Default is 3.
         b (int): Value to add to the scaled value of n. Default is 1.
         max_stopping_time (int): Maximum amount of times to iterate the
             function, if the stopping time is not reached. IF the
             max_stopping_time is reached, the function will return None.
@@ -263,51 +269,51 @@
             _CC.STOPPING_TIME.value: end_msg[1],
             _CC.CYCLE_LENGTH.value: infinity,
             _CC.ZERO_STOP.value: end_msg[1],
             _CC.MAX_STOP_OOB.value: None,
             }.get(end_msg[0], None)
 
 
-def tree_graph(initial_value:int, max_orbit_distance:int, P:int=2, a:int=3,
-               b:int=1, __cycle_prevention:Optional[Set[int]]=None):
+def tree_graph(initial_value: int, max_orbit_distance: int, P: int = 2, a: int = 3,
+               b: int = 1, __cycle_prevention: Optional[Set[int]] = None):
     """
     Returns nested dictionaries that model the directed tree graph up to a
     maximum nesting of max_orbit_distance, with the initial_value as the root.
 
     Args:
         initial_value (int): The root value of the directed tree graph.
         max_orbit_distance (int): Maximum amount of times to iterate the reverse
             function. There is no natural termination to populating the tree
             graph, equivalent to the termination of hailstone sequences or
             stopping time attempts, so this is not an optional argument like
             max_stopping_time / max_total_stopping_time, as it is the intended
             target of orbits to obtain, rather than a limit to avoid uncapped
             computation.
-    
-    Kwargs:
+
+    Keyword Args:
         P (int): Modulus used to devide n, iff n is equivalent to (0 mod P)
             Default is 2.
         a (int): Factor by which to multiply n. Default is 3.
         b (int): Value to add to the scaled value of n. Default is 1.
-    
-    Internal Kwargs:
+
+    Internal Keyword Args:
         __cycle_prevention (set[int]): Used to prevent cycles from precipitating
             by keeping track of all values added across previous nest depths.
     """
     # Call out the reverse_function before any magic returns to trap bad values.
-    _ = reverse_function(initial_value,P=P,a=a,b=b)
-    tgraph = {initial_value:{}}
+    _ = reverse_function(initial_value, P=P, a=a, b=b)
+    tgraph = {initial_value: {}}
     if max(0, max_orbit_distance) == 0:
         return tgraph
     # Handle cycle prevention for recursive calls ~
     # Shouldn't use a mutable object initialiser for a default.
     if __cycle_prevention is None:
         __cycle_prevention = set()
     __cycle_prevention.add(initial_value)
     for branch_value in reverse_function(initial_value, P=P, a=a, b=b):
         if branch_value in __cycle_prevention:
             tgraph[initial_value][_CC.CYCLE_INIT.value] = branch_value
         else:
-            tgraph[initial_value][branch_value] = tree_graph(branch_value,
-                max_orbit_distance-1, P=P, a=a, b=b,
+            tgraph[initial_value][branch_value] = tree_graph(
+                branch_value, max_orbit_distance-1, P=P, a=a, b=b,
                 __cycle_prevention=__cycle_prevention)[branch_value]
     return tgraph
```

### Comparing `collatz-1.0.0/src/collatz.egg-info/PKG-INFO` & `collatz-1.0.1/src/collatz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 Metadata-Version: 2.1
 Name: collatz
-Version: 1.0.0
+Version: 1.0.1
 Summary: Enabling experimenting with functions related to or involved in the Collatz conjecture.
 Home-page: https://github.com/Skenvy/Collatz
 Author: Skenvy
 Author-email: nathan.a.z.levett@gmail.com
-License: UNKNOWN
+License: Apache Software License
 Project-URL: Bug Tracker, https://github.com/Skenvy/Collatz/issues
-Platform: UNKNOWN
+Keywords: Collatz,Ulam,Kakutani's,Thwaites,Hasse's,Syracus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [Collatz](https://github.com/Skenvy/Collatz): [Python](https://github.com/Skenvy/Collatz/tree/main/python)
-Functions related to [the Collatz/Syracuse/3N+1 problem](https://en.wikipedia.org/wiki/Collatz_conjecture), implemented in Python.
+# [Collatz](https://github.com/Skenvy/Collatz): [Python](https://github.com/Skenvy/Collatz/tree/main/python) 🐍🐍🐍
+Functions related to [the Collatz/Syracuse/3N+1 problem](https://en.wikipedia.org/wiki/Collatz_conjecture), implemented in [Python](https://www.python.org/).
 ## Getting Started
-To [install the latest](https://pypi.org/project/collatz/);
-```
+[To install the latest from pypi](https://pypi.org/project/collatz/);
+```sh
 pip install collatz
 ```
-### Developing
-#### The first time virtual env
-```
-git clone https://github.com/Skenvy/Collatz.git
-cd Collatz/python
-make venv
-```
-#### Iterative development
-`make build` will test and build the wheel and force reinstall it into the local venv, to test the built distribution
 ## Usage
 Provides the basic functionality to interact with the Collatz conjecture.
 The parameterisation uses the same `(P,a,b)` notation as Conway's generalisations.
 Besides the function and reverse function, there is also functionality to retrieve the hailstone sequence, the "stopping time"/"total stopping time", or tree-graph. 
 The only restriction placed on parameters is that both `P` and `a` can't be `0`.
 ### collatz.function(~)
 `(n:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # The default "Collatz function"
 >>> collatz.function(5)
 16
 >>> # Alternatively, you can parameterise the function.
 >>> collatz.function(5, P=7, a=5, b=17)
 42
 ```
 ### collatz.reverse_function(~)
 `(n:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # Get the list of values that return the input.
 >>> collatz.reverse_function(4)
 [1, 8]
 >>> # Alternatively, you can parameterise the reverse_function.
 >>> collatz.reverse_function(5, P=5, a=2, b=3)
 [1, 25]
 ```
 ### collatz.hailstone_sequence(~)
 `(initial_value:int, P:int=2,  a:int=3, b:int=1, max_total_stopping_time:int=1000, total_stopping_time:bool=True, verbose:bool=True)`
-```
+```python
 >>> import collatz
 >>> # Get the sequence of values forming the hailstone from an initial value
 >>> collatz.hailstone_sequence(10)
 [10, 5, 16, 8, 4, 2, 1, ['TOTAL_STOPPING_TIME', 6]]
 >>> # Determines if it's in a cycle
 >>> collatz.hailstone_sequence(-56)
 [-56, -28, 'CYCLE_INIT', [-14, -7, -20, -10, -5], ['CYCLE_LENGTH', 5]]
@@ -73,15 +65,15 @@
 [-200, -100, -50, -25, -74, -37, -110, -55, -164, -82, -41, -122, -61, -182, -91, -272, -136, -68, -34, -17, -50]
 >>> # Although hailstones typically go to the "total stop" of 1, they can be set to terminate on the regular stop
 >>> collatz.hailstone_sequence(5, total_stopping_time=False)
 [5, 16, 8, 4, ['STOPPING_TIME', 3]]
 ```
 ### collatz.stopping_time(~)
 `(initial_value:int, P:int=2, a:int=3, b:int=1, max_stopping_time:int=1000, total_stopping_time:bool=False)`
-```
+```python
 >>> import collatz
 >>> # Reports the stopping time, the amount of iterations of the function to reach a value lower than the initial value.
 >>> collatz.stopping_time(5)
 3
 >>> # Can be used to find the "total stopping time" as well, the amount of iterations to reach "1"
 >>> collatz.stopping_time(5, total_stopping_time=True)
 5
@@ -93,20 +85,27 @@
 inf
 >>> # If it overruns maximum stopping time, returns nothing.
 >>> collatz.stopping_time(5, max_stopping_time=-1)
 >>> # <None>
 ```
 ### collatz.tree_graph(~)
 `(initial_value:int, max_orbit_distance:int, P:int=2, a:int=3, b:int=1)`
-```
+```python
 >>> import collatz
 >>> # See the tree graph built by a reverse function traversal, to the depth specified by max_orbit_distance.
 >>> collatz.tree_graph(1, 3)
 {1: {2: {4: {'CYCLE_INIT': 1, 8: {}}}}}
 >>> collatz.tree_graph(1, 12)
 {1: {2: {4: {'CYCLE_INIT': 1, 8: {16: {5: {10: {3: {6: {12: {24: {48: {96: {}}}}}}, 20: {40: {13: {26: {52: {17: {}, 104: {}}}}, 80: {160: {53: {106: {}}, 320: {640: {}}}}}}}}, 32: {64: {21: {42: {84: {168: {336: {672: {}}}}}}, 128: {256: {85: {170: {340: {113: {}, 680: {}}}}, 512: {1024: {341: {682: {}}, 2048: {4096: {}}}}}}}}}}}}}}
 >>> # Can also be parameterised;
 >>> collatz.tree_graph(1, 2, P=5, a=2, b=3)
 {1: {-1: {-5: {}, -2: {}}, 5: {'CYCLE_INIT': 1, 25: {}}}}
 ```
-
-
+## [Sphinx+MyST generated docs](https://skenvy.github.io/Collatz/python/)
+## Developing
+### The first time setup
+```
+git clone https://github.com/Skenvy/Collatz.git && cd Collatz/python && make venv
+```
+### Iterative development
+* `make build` will test and build the wheel and force reinstall it into the local venv, to test the built distribution
+## [Open Source Insights](https://deps.dev/pypi/collatz)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `collatz-1.0.0/tests/test_parameterised.py` & `collatz-1.0.1/tests/test_parameterised.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,15 +72,16 @@
         collatz.reverse_function(1, P=0, a=0, b=3)
     with pytest.raises(AssertionError, match=_REGEX_ERR_A_IS_ZERO):
         collatz.reverse_function(1, P=1, a=0, b=3)
     # If b is a multiple of a, but not of Pa, then 0 can have a reverse.
     assert collatz.reverse_function(0, P=17, a=2, b=-6) == [0, 3]
     assert collatz.reverse_function(0, P=17, a=2, b=102) == [0]
 
-# Test def hailstone_sequence(initial_value:int, P:int=2, 
+
+# Test def hailstone_sequence(initial_value:int, P:int=2,
 # a:int=3, b:int=1, max_total_stopping_time:int=1000,
 # total_stopping_time:bool=True, verbose:bool=True)
 def test_hailstone_sequence():
     # Test 0's immediated termination.
     assert collatz.hailstone_sequence(0) == [[_CC.ZERO_STOP.value, 0]]
     assert collatz.hailstone_sequence(0, verbose=False) == [0]
     # The cycle containing 1 wont yield a cycle termination, as 1 is considered
@@ -89,46 +90,46 @@
     assert collatz.hailstone_sequence(1, verbose=False) == [1]
     # Test the 3 known default parameter's cycles (ignoring [1,4,2])
     # If not verbose, then the result will be the cycle plus the final value
     # being the start of the cycle. If verbose, then the output will be the
     # values not in the cycle, a CC flag, then the cycle and another CC flag.
     for kc in [kc for kc in _KNOWN_CYCLES if 1 not in kc]:
         assert collatz.hailstone_sequence(kc[0], verbose=False) == kc + [kc[0]]
-        assert collatz.hailstone_sequence(kc[0]) == [_CC.CYCLE_INIT.value, kc,
-                                            [_CC.CYCLE_LENGTH.value, len(kc)]]
+        assert collatz.hailstone_sequence(kc[0]) == [
+            _CC.CYCLE_INIT.value, kc, [_CC.CYCLE_LENGTH.value, len(kc)]]
     # Test the lead into a cycle by entering two of the cycles.
     seq = [kc for kc in _KNOWN_CYCLES if -5 in kc][0]
     seq = [seq[1]*4, seq[1]*2] + seq[1:] + [seq[0]]
     assert collatz.hailstone_sequence(-56, verbose=False) == seq + [seq[2]]
-    assert collatz.hailstone_sequence(-56) == seq[:2] + [_CC.CYCLE_INIT.value,
-                            seq[2:], [_CC.CYCLE_LENGTH.value, len(seq[2:])]]
+    assert collatz.hailstone_sequence(-56) == seq[:2] + [
+        _CC.CYCLE_INIT.value, seq[2:], [_CC.CYCLE_LENGTH.value, len(seq[2:])]]
     seq = [kc for kc in _KNOWN_CYCLES if -17 in kc][0]
     seq = [seq[1]*4, seq[1]*2] + seq[1:] + [seq[0]]
     assert collatz.hailstone_sequence(-200, verbose=False) == seq + [seq[2]]
-    assert collatz.hailstone_sequence(-200) == seq[:2] + [_CC.CYCLE_INIT.value,
-                            seq[2:], [_CC.CYCLE_LENGTH.value, len(seq[2:])]]
+    assert collatz.hailstone_sequence(-200) == seq[:2] + [
+        _CC.CYCLE_INIT.value, seq[2:], [_CC.CYCLE_LENGTH.value, len(seq[2:])]]
     # 1's cycle wont yield a description of it being a "cycle" as far as the
     # hailstones are concerned, which is to be expected, so..
     assert collatz.hailstone_sequence(4, verbose=False) == [4, 2, 1]
-    assert collatz.hailstone_sequence(4) == [4, 2, 1,
-                            [_CC.TOTAL_STOPPING_TIME.value, 2]]
+    assert collatz.hailstone_sequence(4) == [
+        4, 2, 1, [_CC.TOTAL_STOPPING_TIME.value, 2]]
     assert collatz.hailstone_sequence(16, verbose=False) == [16, 8, 4, 2, 1]
-    assert collatz.hailstone_sequence(16) == [16, 8, 4, 2, 1,
-                            [_CC.TOTAL_STOPPING_TIME.value, 4]]
+    assert collatz.hailstone_sequence(16) == [
+        16, 8, 4, 2, 1, [_CC.TOTAL_STOPPING_TIME.value, 4]]
     # Test the regular stopping time check.
-    assert collatz.hailstone_sequence(4, total_stopping_time=False) == [4, 2,
-                            [_CC.STOPPING_TIME.value, 1]]
-    assert collatz.hailstone_sequence(5, total_stopping_time=False) == [5, 16,
-                            8, 4, [_CC.STOPPING_TIME.value, 3]]
+    assert collatz.hailstone_sequence(4, total_stopping_time=False) == [
+        4, 2, [_CC.STOPPING_TIME.value, 1]]
+    assert collatz.hailstone_sequence(5, total_stopping_time=False) == [
+        5, 16, 8, 4, [_CC.STOPPING_TIME.value, 3]]
     # Test small max_total_stopping_time: (minimum internal value is one)
-    assert collatz.hailstone_sequence(4, max_total_stopping_time=-100) == [4, 2,
-                            [_CC.MAX_STOP_OOB.value, 1]]
+    assert collatz.hailstone_sequence(4, max_total_stopping_time=-100) == [
+        4, 2, [_CC.MAX_STOP_OOB.value, 1]]
     # Test the zero stop mid hailing. This wont happen with default params tho.
-    assert collatz.hailstone_sequence(3, P=2, a=3, b=-9) == [3, 0,
-                            [_CC.ZERO_STOP.value, -1]]
+    assert collatz.hailstone_sequence(3, P=2, a=3, b=-9) == [
+        3, 0, [_CC.ZERO_STOP.value, -1]]
     # Lastly, while the function wont let you use a P value of 0, 1 and -1 are
     # still allowed, although they will generate immediate 1 or 2 length cycles
     # respectively, so confirm the behaviour of each of these hailstones.
     assert collatz.hailstone_sequence(3, P=1, verbose=False) == [3, 3]
     assert collatz.hailstone_sequence(3, P=-1, verbose=False) == [3, -3, 3]
     # Set P and a to 0 to assert on __assert_sane_parameterisation
     with pytest.raises(AssertionError, match=_REGEX_ERR_P_IS_ZERO):
@@ -160,15 +161,15 @@
     # hailstones are concerned, which is to be expected, so..
     assert collatz.stopping_time(4, total_stopping_time=True) == 2
     assert collatz.stopping_time(16, total_stopping_time=True) == 4
     # Test the regular stopping time check.
     assert collatz.stopping_time(4) == 1
     assert collatz.stopping_time(5) == 3
     # Test small max_total_stopping_time: (minimum internal value is one)
-    assert collatz.stopping_time(5, max_stopping_time=-100) == None
+    assert collatz.stopping_time(5, max_stopping_time=-100) is None
     # Test the zero stop mid hailing. This wont happen with default params tho.
     assert collatz.stopping_time(3, P=2, a=3, b=-9) == -1
     # Lastly, while the function wont let you use a P value of 0, 1 and -1 are
     # still allowed, although they will generate immediate 1 or 2 length cycles
     # respectively, so confirm the behaviour of each of these stopping times.
     assert collatz.stopping_time(3, P=1) == infinity
     assert collatz.stopping_time(3, P=-1) == infinity
@@ -188,48 +189,48 @@
 
 # Test def tree_graph(initial_value:int, max_orbit_distance:int, P:int=2,
 # a:int=3, b:int=1, __cycle_prevention:Optional[Set[int]]=None)
 def test_tree_graph():
     C = _CC.CYCLE_INIT.value  # Shorthand the cycle terminus
     D = {}  # Just to colourise the below in the editor..
     # The default zero trap
-    assert collatz.tree_graph(0, 0) == {0:D}
-    assert collatz.tree_graph(0, 1) == {0:{C:0}}
-    assert collatz.tree_graph(0, 2) == {0:{C:0}}
+    assert collatz.tree_graph(0, 0) == {0: D}
+    assert collatz.tree_graph(0, 1) == {0: {C: 0}}
+    assert collatz.tree_graph(0, 2) == {0: {C: 0}}
     # The roundings of the 1 cycle.
-    assert collatz.tree_graph(1, 1) == {1:{2:D}}
-    assert collatz.tree_graph(1, 0) == {1:D}
-    assert collatz.tree_graph(1, 1) == {1:{2:D}}
-    assert collatz.tree_graph(1, 2) == {1:{2:{4:D}}}
-    assert collatz.tree_graph(1, 3) == {1:{2:{4:{C:1,8:D}}}}
-    assert collatz.tree_graph(2, 3) == {2:{4:{1:{C:2},8:{16:D}}}}
-    assert collatz.tree_graph(4, 3) == {4:{1:{2:{C:4}},8:{16:{5:D,32:D}}}}
+    assert collatz.tree_graph(1, 1) == {1: {2: D}}
+    assert collatz.tree_graph(1, 0) == {1: D}
+    assert collatz.tree_graph(1, 1) == {1: {2: D}}
+    assert collatz.tree_graph(1, 2) == {1: {2: {4: D}}}
+    assert collatz.tree_graph(1, 3) == {1: {2: {4: {C: 1, 8: D}}}}
+    assert collatz.tree_graph(2, 3) == {2: {4: {1: {C: 2}, 8: {16: D}}}}
+    assert collatz.tree_graph(4, 3) == {4: {1: {2: {C: 4}}, 8: {16: {5: D, 32: D}}}}
     # The roundings of the -1 cycle
-    assert collatz.tree_graph(-1, 1) == {-1:{-2:D}}
-    assert collatz.tree_graph(-1, 2) == {-1:{-2:{-4:D,C:-1}}}
+    assert collatz.tree_graph(-1, 1) == {-1: {-2: D}}
+    assert collatz.tree_graph(-1, 2) == {-1: {-2: {-4: D, C: -1}}}
     # Test a wider modulo sweep by upping P to 5, a to 2, and b to 3.
-    T = lambda x,y: {1:{-1:x,5:y}}
-    orb_1 = T(D,D)
-    orb_2 = T({-5:D,-2:D},{C:1,25:D})
-    T = lambda x,y,z: {1:{-1:{-5:x,-2:y},5:{C:1,25:z}}}
-    orb_3 = T({-25:D,-4:D},{-10:D},{11:D,125:D})
+    tree = lambda x, y: {1: {-1: x, 5: y}}
+    orb_1 = tree(D, D)
+    orb_2 = tree({-5: D, -2: D}, {C: 1, 25: D})
+    tree = lambda x, y, z: {1: {-1: {-5: x, -2: y}, 5: {C: 1, 25: z}}}
+    orb_3 = tree({-25: D, -4: D}, {-10: D}, {11: D, 125: D})
     assert collatz.tree_graph(1, 1, P=5, a=2, b=3) == orb_1
     assert collatz.tree_graph(1, 2, P=5, a=2, b=3) == orb_2
     assert collatz.tree_graph(1, 3, P=5, a=2, b=3) == orb_3
     # Test negative P, a and b.
-    orb_1 = {1:{-3:D}}
-    T = lambda x,y: {1:{-3:{-1:x,9:y}}}
-    orb_2 = T(D,D)
-    orb_3 = T({-2:D,3:D},{-27:D,-7:D})
+    orb_1 = {1: {-3: D}}
+    tree = lambda x, y: {1: {-3: {-1: x, 9: y}}}
+    orb_2 = tree(D, D)
+    orb_3 = tree({-2: D, 3: D}, {-27: D, -7: D})
     assert collatz.tree_graph(1, 1, P=-3, a=-2, b=-5) == orb_1
     assert collatz.tree_graph(1, 2, P=-3, a=-2, b=-5) == orb_2
     assert collatz.tree_graph(1, 3, P=-3, a=-2, b=-5) == orb_3
     # Set P and a to 0 to assert on __assert_sane_parameterisation
     with pytest.raises(AssertionError, match=_REGEX_ERR_P_IS_ZERO):
         collatz.tree_graph(1, 1, P=0, a=2, b=3)
     with pytest.raises(AssertionError, match=_REGEX_ERR_P_IS_ZERO):
         collatz.tree_graph(1, 1, P=0, a=0, b=3)
     with pytest.raises(AssertionError, match=_REGEX_ERR_A_IS_ZERO):
         collatz.tree_graph(1, 1, P=1, a=0, b=3)
     # If b is a multiple of a, but not of Pa, then 0 can have a reverse.
-    assert collatz.tree_graph(0, 1, P=17, a=2, b=-6) == {0:{C:0,3:D}}
-    assert collatz.tree_graph(0, 1, P=17, a=2, b=102) == {0:{C:0}}
+    assert collatz.tree_graph(0, 1, P=17, a=2, b=-6) == {0: {C: 0, 3: D}}
+    assert collatz.tree_graph(0, 1, P=17, a=2, b=102) == {0: {C: 0}}
```

