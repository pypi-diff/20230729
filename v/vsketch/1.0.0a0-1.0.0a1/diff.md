# Comparing `tmp/vsketch-1.0.0a0.tar.gz` & `tmp/vsketch-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsketch-1.0.0a0.tar", max compression
+gzip compressed data, was "vsketch-1.0.0a1.tar", max compression
```

## Comparing `vsketch-1.0.0a0.tar` & `vsketch-1.0.0a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    17977 2020-08-24 21:05:21.010612 vsketch-1.0.0a0/LICENSE
--rw-r--r--   0        0        0     7450 2022-10-16 14:53:54.123137 vsketch-1.0.0a0/README.md
--rw-r--r--   0        0        0     1882 2023-03-19 10:02:09.446818 vsketch-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      426 2022-06-13 08:48:02.682849 vsketch-1.0.0a0/vsketch/__init__.py
--rw-r--r--   0        0        0     5008 2022-05-09 11:03:29.137380 vsketch-1.0.0a0/vsketch/curves.py
--rw-r--r--   0        0        0     4064 2022-11-11 17:39:56.236755 vsketch-1.0.0a0/vsketch/display.py
--rw-r--r--   0        0        0     1465 2022-05-09 11:03:29.138754 vsketch-1.0.0a0/vsketch/easing.py
--rw-r--r--   0        0        0     1736 2022-11-11 17:39:56.237009 vsketch-1.0.0a0/vsketch/fill.py
--rw-r--r--   0        0        0    32830 2023-07-25 20:26:43.220158 vsketch-1.0.0a0/vsketch/shape.py
--rw-r--r--   0        0        0     8566 2023-07-25 20:26:43.221423 vsketch-1.0.0a0/vsketch/sketch_class.py
--rw-r--r--   0        0        0     1895 2022-05-09 11:03:29.141090 vsketch-1.0.0a0/vsketch/style.py
--rw-r--r--   0        0        0     2429 2022-05-09 11:03:29.141590 vsketch-1.0.0a0/vsketch/utils.py
--rw-r--r--   0        0        0    72383 2023-07-25 20:26:43.222065 vsketch-1.0.0a0/vsketch/vsketch.py
--rw-r--r--   0        0        0        0 2021-03-26 10:23:18.168609 vsketch-1.0.0a0/vsketch_cli/__init__.py
--rw-r--r--   0        0        0       28 2021-03-26 10:23:18.169029 vsketch-1.0.0a0/vsketch_cli/__main__.py
--rw-r--r--   0        0        0    17381 2023-07-25 20:26:43.222494 vsketch-1.0.0a0/vsketch_cli/cli.py
--rw-r--r--   0        0        0     3257 2023-03-19 10:02:09.449108 vsketch-1.0.0a0/vsketch_cli/config_widget.py
--rw-r--r--   0        0        0     1445 2023-07-25 20:26:43.223227 vsketch-1.0.0a0/vsketch_cli/gui.py
--rw-r--r--   0        0        0     6475 2023-03-19 10:02:09.450348 vsketch-1.0.0a0/vsketch_cli/param_widget.py
--rw-r--r--   0        0        0      687 2022-11-11 17:39:56.238493 vsketch-1.0.0a0/vsketch_cli/seed_widget.py
--rw-r--r--   0        0        0     7701 2023-07-25 20:26:43.223626 vsketch-1.0.0a0/vsketch_cli/sketch_viewer.py
--rw-r--r--   0        0        0     2424 2023-07-25 20:26:43.224002 vsketch-1.0.0a0/vsketch_cli/threads.py
--rw-r--r--   0        0        0     2770 2022-11-11 09:48:06.345677 vsketch-1.0.0a0/vsketch_cli/utils.py
--rw-r--r--   0        0        0     8503 1970-01-01 00:00:00.000000 vsketch-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0    17977 2023-07-29 08:47:29.764203 vsketch-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     7419 2023-07-29 08:47:29.764203 vsketch-1.0.0a1/README.md
+-rw-r--r--   0        0        0     1876 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      426 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/__init__.py
+-rw-r--r--   0        0        0     5008 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/curves.py
+-rw-r--r--   0        0        0     4064 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/display.py
+-rw-r--r--   0        0        0     1465 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/easing.py
+-rw-r--r--   0        0        0     1736 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/fill.py
+-rw-r--r--   0        0        0    32830 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/shape.py
+-rw-r--r--   0        0        0     8566 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/sketch_class.py
+-rw-r--r--   0        0        0     1895 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/style.py
+-rw-r--r--   0        0        0     2429 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/utils.py
+-rw-r--r--   0        0        0    72383 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch/vsketch.py
+-rw-r--r--   0        0        0        0 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch_cli/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch_cli/__main__.py
+-rw-r--r--   0        0        0    17381 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch_cli/cli.py
+-rw-r--r--   0        0        0     3257 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch_cli/config_widget.py
+-rw-r--r--   0        0        0     1445 2023-07-29 08:47:29.888204 vsketch-1.0.0a1/vsketch_cli/gui.py
+-rw-r--r--   0        0        0     6475 2023-07-29 08:47:29.892205 vsketch-1.0.0a1/vsketch_cli/param_widget.py
+-rw-r--r--   0        0        0      687 2023-07-29 08:47:29.892205 vsketch-1.0.0a1/vsketch_cli/seed_widget.py
+-rw-r--r--   0        0        0     7701 2023-07-29 08:47:29.892205 vsketch-1.0.0a1/vsketch_cli/sketch_viewer.py
+-rw-r--r--   0        0        0     2424 2023-07-29 08:47:29.892205 vsketch-1.0.0a1/vsketch_cli/threads.py
+-rw-r--r--   0        0        0     2770 2023-07-29 08:47:29.892205 vsketch-1.0.0a1/vsketch_cli/utils.py
+-rw-r--r--   0        0        0     8472 1970-01-01 00:00:00.000000 vsketch-1.0.0a1/PKG-INFO
```

### Comparing `vsketch-1.0.0a0/LICENSE` & `vsketch-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/README.md` & `vsketch-1.0.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
 
 ## Installing *vsketch*
 
 The recommended way to install *vsketch* is as a stand-alone installation using pipx:
 
 ```bash
-$ pipx install git+https://github.com/abey79/vsketch
+$ pipx install vsketch
 ```
 
-To run the examples, they must be [downloaded](https://github.com/abey79/vsketch/archive/refs/heads/master.zip) separately. After uncompressing the archive, they can be run using the following command:
+To run the examples, they must be [downloaded](https://github.com/abey79/vsketch/archive/refs/heads/master.zip) separately. After decompressing the archive, they can be run using the following command:
 
 ```bash
 $ vsk run path/to/vsketch-master/examples/schotter
 ```
 
 Check the [installation instructions](https://vsketch.readthedocs.io/en/latest/install.html) for more details.
 
@@ -159,15 +159,15 @@
 
 Finally, being extremely picky, it would be nice to be able to generate ONE HUNDRED versions of this sketch with various random seeds, in hope to find the most perfect version for plotting and framing. `vsk` will do this for you, using all CPU cores available:
 
 ```bash
 $ vsk save --config "Best config" --seed 0..99 my_project
 ```
 
-You'll find all the SVG file in the project's `output` sub-directory:
+You'll find all the SVG file in the project's `output` subdirectory:
 
 <img width="600" alt="image" src="https://user-images.githubusercontent.com/49431240/107375111-abab0180-6ae8-11eb-8034-d84c9d400ab2.png">
 
 Next steps:
 * Use `vsk` integrated help to learn about the all the possibilities (`vsk --help`).
 * Learn the vsketch API on the documentation's [overview](https://vsketch.readthedocs.io/en/latest/overview.html) and [reference](https://vsketch.readthedocs.io/en/latest/reference.html) pages.
```

### Comparing `vsketch-1.0.0a0/pyproject.toml` & `vsketch-1.0.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vsketch"
-version = "1.0.0-alpha.0"
+version = "1.0.0a1"
 description = "Plotter generative art environment"
 authors = ["Antoine Beyeler <abeyeler@ab-ware.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/abey79/vsketch"
 documentation = "https://vsketch.readthedocs.io/en/latest/"
 classifiers = [
```

### Comparing `vsketch-1.0.0a0/vsketch/curves.py` & `vsketch-1.0.0a1/vsketch/curves.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/display.py` & `vsketch-1.0.0a1/vsketch/display.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/easing.py` & `vsketch-1.0.0a1/vsketch/easing.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/fill.py` & `vsketch-1.0.0a1/vsketch/fill.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/shape.py` & `vsketch-1.0.0a1/vsketch/shape.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/sketch_class.py` & `vsketch-1.0.0a1/vsketch/sketch_class.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/style.py` & `vsketch-1.0.0a1/vsketch/style.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/utils.py` & `vsketch-1.0.0a1/vsketch/utils.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch/vsketch.py` & `vsketch-1.0.0a1/vsketch/vsketch.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/cli.py` & `vsketch-1.0.0a1/vsketch_cli/cli.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/config_widget.py` & `vsketch-1.0.0a1/vsketch_cli/config_widget.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/gui.py` & `vsketch-1.0.0a1/vsketch_cli/gui.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/param_widget.py` & `vsketch-1.0.0a1/vsketch_cli/param_widget.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/seed_widget.py` & `vsketch-1.0.0a1/vsketch_cli/seed_widget.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/sketch_viewer.py` & `vsketch-1.0.0a1/vsketch_cli/sketch_viewer.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/threads.py` & `vsketch-1.0.0a1/vsketch_cli/threads.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/vsketch_cli/utils.py` & `vsketch-1.0.0a1/vsketch_cli/utils.py`

 * *Files identical despite different names*

### Comparing `vsketch-1.0.0a0/PKG-INFO` & `vsketch-1.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsketch
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Plotter generative art environment
 Home-page: https://github.com/abey79/vsketch
 License: MIT
 Author: Antoine Beyeler
 Author-email: abeyeler@ab-ware.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -60,18 +60,18 @@
 
 
 ## Installing *vsketch*
 
 The recommended way to install *vsketch* is as a stand-alone installation using pipx:
 
 ```bash
-$ pipx install git+https://github.com/abey79/vsketch
+$ pipx install vsketch
 ```
 
-To run the examples, they must be [downloaded](https://github.com/abey79/vsketch/archive/refs/heads/master.zip) separately. After uncompressing the archive, they can be run using the following command:
+To run the examples, they must be [downloaded](https://github.com/abey79/vsketch/archive/refs/heads/master.zip) separately. After decompressing the archive, they can be run using the following command:
 
 ```bash
 $ vsk run path/to/vsketch-master/examples/schotter
 ```
 
 Check the [installation instructions](https://vsketch.readthedocs.io/en/latest/install.html) for more details.
 
@@ -188,15 +188,15 @@
 
 Finally, being extremely picky, it would be nice to be able to generate ONE HUNDRED versions of this sketch with various random seeds, in hope to find the most perfect version for plotting and framing. `vsk` will do this for you, using all CPU cores available:
 
 ```bash
 $ vsk save --config "Best config" --seed 0..99 my_project
 ```
 
-You'll find all the SVG file in the project's `output` sub-directory:
+You'll find all the SVG file in the project's `output` subdirectory:
 
 <img width="600" alt="image" src="https://user-images.githubusercontent.com/49431240/107375111-abab0180-6ae8-11eb-8034-d84c9d400ab2.png">
 
 Next steps:
 * Use `vsk` integrated help to learn about the all the possibilities (`vsk --help`).
 * Learn the vsketch API on the documentation's [overview](https://vsketch.readthedocs.io/en/latest/overview.html) and [reference](https://vsketch.readthedocs.io/en/latest/reference.html) pages.
```

