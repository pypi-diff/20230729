# Comparing `tmp/SPCEj9bbotw-0.0.3.tar.gz` & `tmp/SPCEj9bbotw-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPCEj9bbotw-0.0.3.tar", last modified: Sat Jul 29 11:20:36 2023, max compression
+gzip compressed data, was "SPCEj9bbotw-0.0.4.tar", last modified: Sat Jul 29 11:24:44 2023, max compression
```

## Comparing `SPCEj9bbotw-0.0.3.tar` & `SPCEj9bbotw-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:20:36.633211 SPCEj9bbotw-0.0.3/
--rw-rw-rw-   0        0        0       58 2023-07-29 11:20:36.633211 SPCEj9bbotw-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 11:20:36.626207 SPCEj9bbotw-0.0.3/SPCEj9bbotw/
--rw-rw-rw-   0        0        0     3028 2023-06-14 07:31:18.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw/_.py
--rw-rw-rw-   0        0        0       21 2023-07-29 11:19:15.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-07-29 11:17:04.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw/_main.py
--rw-rw-rw-   0        0        0     8306 2023-07-29 08:22:02.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw/kernels.py
--rw-rw-rw-   0        0        0    14642 2023-07-29 11:13:11.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw/optimizer.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:20:36.632211 SPCEj9bbotw-0.0.3/SPCEj9bbotw.egg-info/
--rw-rw-rw-   0        0        0       58 2023-07-29 11:20:36.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-29 11:20:36.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:20:36.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-29 11:20:36.000000 SPCEj9bbotw-0.0.3/SPCEj9bbotw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:20:36.634210 SPCEj9bbotw-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-07-29 11:19:27.000000 SPCEj9bbotw-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:24:44.748187 SPCEj9bbotw-0.0.4/
+-rw-rw-rw-   0        0        0       58 2023-07-29 11:24:44.748187 SPCEj9bbotw-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 11:24:44.736184 SPCEj9bbotw-0.0.4/SPCEj9bbotw/
+-rw-rw-rw-   0        0        0     3028 2023-06-14 07:31:18.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/_.py
+-rw-rw-rw-   0        0        0       21 2023-07-29 11:24:02.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-07-29 11:24:24.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/_main.py
+-rw-rw-rw-   0        0        0     8306 2023-07-29 08:22:02.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/kernels.py
+-rw-rw-rw-   0        0        0    14654 2023-07-29 11:24:26.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:24:44.746187 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-29 11:24:44.000000 SPCEj9bbotw-0.0.4/SPCEj9bbotw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 11:24:44.748187 SPCEj9bbotw-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-07-29 11:24:22.000000 SPCEj9bbotw-0.0.4/setup.py
```

### Comparing `SPCEj9bbotw-0.0.3/SPCEj9bbotw/_.py` & `SPCEj9bbotw-0.0.4/SPCEj9bbotw/_.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.3/SPCEj9bbotw/_main.py` & `SPCEj9bbotw-0.0.4/SPCEj9bbotw/_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import numpy.linalg as lg
 import cupy as cp
-from kernels import *
-from optimizer import *
+from SPCEj9bbotw.kernels import *
+from SPCEj9bbotw.optimizer import *
 import time
 import matplotlib.pyplot as plt
 
 
 x_0 =np.array([2400, 450, -330, -10, -40, 10])[:,np.newaxis]
 x_des = np.zeros(6)
 n = 100
```

### Comparing `SPCEj9bbotw-0.0.3/SPCEj9bbotw/kernels.py` & `SPCEj9bbotw-0.0.4/SPCEj9bbotw/kernels.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.3/SPCEj9bbotw/optimizer.py` & `SPCEj9bbotw-0.0.4/SPCEj9bbotw/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import numpy.linalg as lg
 import cupy as cp
-from _ import *
+from SPCEj9bbotw._ import *
 
 
 '''
 coefficient matrix of primal variable is calculated by cupy inverse function.
 '''
 class gpu_optimizer:
     def __init__(self, x_0, n, dt, rho, cond, g, ang_vel, epoch, func_gpu):
```

