# Comparing `tmp/MetAromatic-1.2.0.tar.gz` & `tmp/MetAromatic-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetAromatic-1.2.0.tar", last modified: Sat Jul 29 10:44:55 2023, max compression
+gzip compressed data, was "MetAromatic-1.3.0.tar", last modified: Sat Jul 29 10:57:30 2023, max compression
```

## Comparing `MetAromatic-1.2.0.tar` & `MetAromatic-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:44:55.918142 MetAromatic-1.2.0/
--rw-rw-rw-   0 dsw       (1000) dsw       (1000)    35149 2022-02-13 05:52:09.000000 MetAromatic-1.2.0/LICENSE
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:44:55.883235 MetAromatic-1.2.0/MetAromatic/
--rw-r--r--   0 dsw       (1000) dsw       (1000)      191 2023-07-29 09:48:32.000000 MetAromatic-1.2.0/MetAromatic/__init__.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     7565 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/MetAromatic/batch.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2648 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/MetAromatic/bridge.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      987 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/MetAromatic/complex_types.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      117 2023-07-18 05:41:26.000000 MetAromatic-1.2.0/MetAromatic/consts.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2029 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/MetAromatic/get_aromatic_midpoints.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     3210 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/MetAromatic/lone_pair_interpolators.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)    11907 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/MetAromatic/pair.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     4752 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/MetAromatic/runner.py
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:44:55.898195 MetAromatic-1.2.0/MetAromatic.egg-info/
--rw-r--r--   0 dsw       (1000) dsw       (1000)      930 2023-07-29 10:44:55.000000 MetAromatic-1.2.0/MetAromatic.egg-info/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)      806 2023-07-29 10:44:55.000000 MetAromatic-1.2.0/MetAromatic.egg-info/SOURCES.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-29 10:44:55.000000 MetAromatic-1.2.0/MetAromatic.egg-info/dependency_links.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       50 2023-07-29 10:44:55.000000 MetAromatic-1.2.0/MetAromatic.egg-info/entry_points.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       47 2023-07-29 10:44:55.000000 MetAromatic-1.2.0/MetAromatic.egg-info/requires.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       17 2023-07-29 10:44:55.000000 MetAromatic-1.2.0/MetAromatic.egg-info/top_level.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)      930 2023-07-29 10:44:55.916147 MetAromatic-1.2.0/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)    19963 2023-07-29 10:40:58.000000 MetAromatic-1.2.0/README.md
--rw-r--r--   0 dsw       (1000) dsw       (1000)      566 2023-07-29 10:42:33.000000 MetAromatic-1.2.0/README_PYPI.md
--rw-r--r--   0 dsw       (1000) dsw       (1000)      651 2023-07-29 10:43:10.000000 MetAromatic-1.2.0/pyproject.toml
--rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-29 10:44:55.918142 MetAromatic-1.2.0/setup.cfg
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:44:55.915150 MetAromatic-1.2.0/tests/
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1805 2023-07-29 09:51:22.000000 MetAromatic-1.2.0/tests/test_api_bridge.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1575 2023-07-29 09:51:09.000000 MetAromatic-1.2.0/tests/test_api_bridge_benchmark.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     4344 2023-07-29 09:51:45.000000 MetAromatic-1.2.0/tests/test_api_pair.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2831 2023-07-29 09:51:36.000000 MetAromatic-1.2.0/tests/test_api_pair_benchmark.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      308 2023-07-19 06:46:26.000000 MetAromatic-1.2.0/tests/test_get_hexagon_midpoints.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1152 2023-04-22 10:25:54.000000 MetAromatic-1.2.0/tests/test_lone_pair_interpolators.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      304 2023-04-22 10:25:54.000000 MetAromatic-1.2.0/tests/test_resolve_runner_from_path.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     4712 2023-04-24 08:25:14.000000 MetAromatic-1.2.0/tests/test_runner_batch.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1959 2023-04-23 12:19:11.000000 MetAromatic-1.2.0/tests/test_runner_bridge.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     3906 2023-05-23 08:25:27.000000 MetAromatic-1.2.0/tests/test_runner_pair.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.292993 MetAromatic-1.3.0/
+-rw-rw-rw-   0 dsw       (1000) dsw       (1000)    35149 2022-02-13 05:52:09.000000 MetAromatic-1.3.0/LICENSE
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.249112 MetAromatic-1.3.0/MetAromatic/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      191 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/MetAromatic/__init__.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     7565 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/batch.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2648 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/bridge.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      987 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/complex_types.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      117 2023-07-18 05:41:26.000000 MetAromatic-1.3.0/MetAromatic/consts.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2029 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/get_aromatic_midpoints.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     3210 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/lone_pair_interpolators.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)    11907 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/pair.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     4752 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/MetAromatic/runner.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.277036 MetAromatic-1.3.0/MetAromatic.egg-info/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      931 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      806 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/SOURCES.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/dependency_links.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       50 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/entry_points.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       47 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/requires.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       17 2023-07-29 10:57:30.000000 MetAromatic-1.3.0/MetAromatic.egg-info/top_level.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      931 2023-07-29 10:57:30.292993 MetAromatic-1.3.0/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)    19961 2023-07-29 10:56:09.000000 MetAromatic-1.3.0/README.md
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      567 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/README_PYPI.md
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      651 2023-07-29 10:57:00.000000 MetAromatic-1.3.0/pyproject.toml
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-29 10:57:30.293991 MetAromatic-1.3.0/setup.cfg
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-29 10:57:30.290999 MetAromatic-1.3.0/tests/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1805 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_bridge.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1575 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_bridge_benchmark.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     4344 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_pair.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2831 2023-07-29 10:47:14.000000 MetAromatic-1.3.0/tests/test_api_pair_benchmark.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      308 2023-07-19 06:46:26.000000 MetAromatic-1.3.0/tests/test_get_hexagon_midpoints.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1152 2023-04-22 10:25:54.000000 MetAromatic-1.3.0/tests/test_lone_pair_interpolators.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      304 2023-04-22 10:25:54.000000 MetAromatic-1.3.0/tests/test_resolve_runner_from_path.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     4712 2023-04-24 08:25:14.000000 MetAromatic-1.3.0/tests/test_runner_batch.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1959 2023-04-23 12:19:11.000000 MetAromatic-1.3.0/tests/test_runner_bridge.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     3906 2023-05-23 08:25:27.000000 MetAromatic-1.3.0/tests/test_runner_pair.py
```

### Comparing `MetAromatic-1.2.0/LICENSE` & `MetAromatic-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic/batch.py` & `MetAromatic-1.3.0/MetAromatic/batch.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic/bridge.py` & `MetAromatic-1.3.0/MetAromatic/bridge.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic/complex_types.py` & `MetAromatic-1.3.0/MetAromatic/complex_types.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic/get_aromatic_midpoints.py` & `MetAromatic-1.3.0/MetAromatic/get_aromatic_midpoints.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic/lone_pair_interpolators.py` & `MetAromatic-1.3.0/MetAromatic/lone_pair_interpolators.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic/pair.py` & `MetAromatic-1.3.0/MetAromatic/pair.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic/runner.py` & `MetAromatic-1.3.0/MetAromatic/runner.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/MetAromatic.egg-info/PKG-INFO` & `MetAromatic-1.3.0/MetAromatic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetAromatic
-Version: 1.2.0
+Version: 1.3.0
 Summary: MetAromatic algorithm
 Author: David Weber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -13,8 +13,9 @@
 # Met-aromatic
 Code for the following publications:
 * Weber, D. S.; Warren, J. J. The Interaction between Methionine and Two Aromatic Amino Acids Is an Abundant
   and Multifunctional Motif in Proteins. _Arch. Biochem. Biophys._ **2019**, _672_, 108053.
 * Weber, D. S.; Warren, J. J. A Survey of Methionine-Aromatic Interaction Geometries in the Oxidoreductase
   Class of Enzymes: What Could Met-Aromatic Interactions be Doing Near Metal Sites? _J. Inorg. Biochem._
 **2018**, _186_, 34-41.
+
 See [MetAromatic](https://github.com/dsw7/MetAromatic) for more information.
```

### Comparing `MetAromatic-1.2.0/MetAromatic.egg-info/SOURCES.txt` & `MetAromatic-1.3.0/MetAromatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/PKG-INFO` & `MetAromatic-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetAromatic
-Version: 1.2.0
+Version: 1.3.0
 Summary: MetAromatic algorithm
 Author: David Weber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -13,8 +13,9 @@
 # Met-aromatic
 Code for the following publications:
 * Weber, D. S.; Warren, J. J. The Interaction between Methionine and Two Aromatic Amino Acids Is an Abundant
   and Multifunctional Motif in Proteins. _Arch. Biochem. Biophys._ **2019**, _672_, 108053.
 * Weber, D. S.; Warren, J. J. A Survey of Methionine-Aromatic Interaction Geometries in the Oxidoreductase
   Class of Enzymes: What Could Met-Aromatic Interactions be Doing Near Metal Sites? _J. Inorg. Biochem._
 **2018**, _186_, 34-41.
+
 See [MetAromatic](https://github.com/dsw7/MetAromatic) for more information.
```

### Comparing `MetAromatic-1.2.0/README.md` & `MetAromatic-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
     arguments = {
         'cutoff_distance': 4.1,
         'cutoff_angle': 109.5,
         'chain': 'A',
         'model': 'cp'
     }
 
-    results = MetAromatic(**arguments).get_met_aromatic_interactions('1rcy')
+    results = MetAromatic(arguments).get_met_aromatic_interactions('1rcy')
 
     for interaction in results.interactions:
         print(dumps(interaction, indent=4))
 
 if __name__ == '__main__':
     main()
 ```
```

### Comparing `MetAromatic-1.2.0/README_PYPI.md` & `MetAromatic-1.3.0/README_PYPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Met-aromatic
 Code for the following publications:
 * Weber, D. S.; Warren, J. J. The Interaction between Methionine and Two Aromatic Amino Acids Is an Abundant
   and Multifunctional Motif in Proteins. _Arch. Biochem. Biophys._ **2019**, _672_, 108053.
 * Weber, D. S.; Warren, J. J. A Survey of Methionine-Aromatic Interaction Geometries in the Oxidoreductase
   Class of Enzymes: What Could Met-Aromatic Interactions be Doing Near Metal Sites? _J. Inorg. Biochem._
 **2018**, _186_, 34-41.
+
 See [MetAromatic](https://github.com/dsw7/MetAromatic) for more information.
```

### Comparing `MetAromatic-1.2.0/pyproject.toml` & `MetAromatic-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "MetAromatic"
-version = "1.2.0"
+version = "1.3.0"
 authors = [{name="David Weber"}]
 description = "MetAromatic algorithm"
 readme = "README_PYPI.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `MetAromatic-1.2.0/tests/test_api_bridge.py` & `MetAromatic-1.3.0/tests/test_api_bridge.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/tests/test_api_bridge_benchmark.py` & `MetAromatic-1.3.0/tests/test_api_bridge_benchmark.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/tests/test_api_pair.py` & `MetAromatic-1.3.0/tests/test_api_pair.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/tests/test_api_pair_benchmark.py` & `MetAromatic-1.3.0/tests/test_api_pair_benchmark.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/tests/test_lone_pair_interpolators.py` & `MetAromatic-1.3.0/tests/test_lone_pair_interpolators.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/tests/test_runner_batch.py` & `MetAromatic-1.3.0/tests/test_runner_batch.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/tests/test_runner_bridge.py` & `MetAromatic-1.3.0/tests/test_runner_bridge.py`

 * *Files identical despite different names*

### Comparing `MetAromatic-1.2.0/tests/test_runner_pair.py` & `MetAromatic-1.3.0/tests/test_runner_pair.py`

 * *Files identical despite different names*

