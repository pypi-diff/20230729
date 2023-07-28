# Comparing `tmp/pysyd-6.10.0.tar.gz` & `tmp/pysyd-6.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysyd-6.10.0.tar", last modified: Fri Nov  4 18:29:26 2022, max compression
+gzip compressed data, was "pysyd-6.10.5.tar", last modified: Thu Mar 23 17:21:35 2023, max compression
```

## Comparing `pysyd-6.10.0.tar` & `pysyd-6.10.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2022-11-04 18:29:26.679084 pysyd-6.10.0/
--rw-r--r--   0 ashleychontos   (501) staff       (20)     5215 2022-03-14 21:00:31.000000 pysyd-6.10.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 ashleychontos   (501) staff       (20)     5287 2022-03-14 21:00:31.000000 pysyd-6.10.0/CONTRIBUTING.md
--rw-r--r--   0 ashleychontos   (501) staff       (20)     1093 2022-04-16 19:53:43.000000 pysyd-6.10.0/LICENSE
--rw-r--r--   0 ashleychontos   (501) staff       (20)      223 2022-10-29 15:44:24.000000 pysyd-6.10.0/MANIFEST.in
--rw-r--r--   0 ashleychontos   (501) staff       (20)     3566 2022-11-04 18:29:26.678840 pysyd-6.10.0/PKG-INFO
--rw-r--r--   0 ashleychontos   (501) staff       (20)     2521 2022-11-03 13:35:07.000000 pysyd-6.10.0/README.md
-drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2022-11-04 18:29:26.672333 pysyd-6.10.0/docs/
--rw-r--r--   0 ashleychontos   (501) staff       (20)       72 2022-03-14 21:00:31.000000 pysyd-6.10.0/docs/COLLABORATORS.rst
--rw-r--r--   0 ashleychontos   (501) staff       (20)      486 2022-03-14 21:00:31.000000 pysyd-6.10.0/docs/CONTRIBUTORS.rst
--rw-r--r--   0 ashleychontos   (501) staff       (20)      104 2021-04-17 02:06:06.000000 pysyd-6.10.0/pyproject.toml
-drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2022-11-04 18:29:26.674183 pysyd-6.10.0/pysyd.egg-info/
--rw-r--r--   0 ashleychontos   (501) staff       (20)     3566 2022-11-04 18:29:26.000000 pysyd-6.10.0/pysyd.egg-info/PKG-INFO
--rw-r--r--   0 ashleychontos   (501) staff       (20)      682 2022-11-04 18:29:26.000000 pysyd-6.10.0/pysyd.egg-info/SOURCES.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)        1 2022-11-04 18:29:26.000000 pysyd-6.10.0/pysyd.egg-info/dependency_links.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)       41 2022-11-04 18:29:26.000000 pysyd-6.10.0/pysyd.egg-info/entry_points.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)       87 2022-11-04 18:29:26.000000 pysyd-6.10.0/pysyd.egg-info/requires.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)        6 2022-11-04 18:29:26.000000 pysyd-6.10.0/pysyd.egg-info/top_level.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)       86 2022-11-02 17:01:43.000000 pysyd-6.10.0/requirements.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)       38 2022-11-04 18:29:26.679175 pysyd-6.10.0/setup.cfg
--rw-r--r--   0 ashleychontos   (501) staff       (20)     1923 2022-11-03 19:41:19.000000 pysyd-6.10.0/setup.py
-drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2022-11-04 18:29:26.668866 pysyd-6.10.0/src/
-drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2022-11-04 18:29:26.676515 pysyd-6.10.0/src/pysyd/
--rw-r--r--   0 ashleychontos   (501) staff       (20)     1583 2022-11-04 18:29:02.000000 pysyd-6.10.0/src/pysyd/__init__.py
--rw-r--r--   0 ashleychontos   (501) staff       (20)    56495 2022-11-03 22:07:29.000000 pysyd-6.10.0/src/pysyd/cli.py
-drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2022-11-04 18:29:26.677738 pysyd-6.10.0/src/pysyd/data/
-drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2022-11-04 18:29:26.678507 pysyd-6.10.0/src/pysyd/data/dicts/
--rw-r--r--   0 ashleychontos   (501) staff       (20)     3131 2022-11-03 15:25:09.000000 pysyd-6.10.0/src/pysyd/data/dicts/columns.dict
--rw-r--r--   0 ashleychontos   (501) staff       (20)     3275 2022-04-20 15:18:51.000000 pysyd-6.10.0/src/pysyd/data/dicts/params.dict
--rw-r--r--   0 ashleychontos   (501) staff       (20)      585 2022-04-20 15:18:51.000000 pysyd-6.10.0/src/pysyd/data/dicts/plots.dict
--rw-r--r--   0 ashleychontos   (501) staff       (20)     1205 2022-04-20 15:18:51.000000 pysyd-6.10.0/src/pysyd/data/pysyd.mplstyle
--rw-r--r--   0 ashleychontos   (501) staff       (20)    19272 2022-04-20 15:18:51.000000 pysyd-6.10.0/src/pysyd/data/pysyd_results.csv
--rw-r--r--   0 ashleychontos   (501) staff       (20)    58471 2022-04-20 15:18:51.000000 pysyd-6.10.0/src/pysyd/data/syd_results.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)     2871 2022-10-30 15:33:28.000000 pysyd-6.10.0/src/pysyd/data/test.txt
--rw-r--r--   0 ashleychontos   (501) staff       (20)    12076 2022-11-01 12:06:44.000000 pysyd-6.10.0/src/pysyd/models.py
--rw-r--r--   0 ashleychontos   (501) staff       (20)     6133 2022-11-04 17:12:13.000000 pysyd-6.10.0/src/pysyd/pipeline.py
--rw-r--r--   0 ashleychontos   (501) staff       (20)    38018 2022-11-03 19:19:54.000000 pysyd-6.10.0/src/pysyd/plots.py
--rw-r--r--   0 ashleychontos   (501) staff       (20)   103390 2022-11-04 17:33:39.000000 pysyd-6.10.0/src/pysyd/target.py
--rw-r--r--   0 ashleychontos   (501) staff       (20)    44950 2022-11-04 17:25:36.000000 pysyd-6.10.0/src/pysyd/utils.py
+drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2023-03-23 17:21:35.443024 pysyd-6.10.5/
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     5215 2022-03-14 21:00:31.000000 pysyd-6.10.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     5287 2022-03-14 21:00:31.000000 pysyd-6.10.5/CONTRIBUTING.md
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     1093 2022-04-16 19:53:43.000000 pysyd-6.10.5/LICENSE
+-rw-r--r--   0 ashleychontos   (501) staff       (20)      223 2022-10-29 15:44:24.000000 pysyd-6.10.5/MANIFEST.in
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     3565 2023-03-23 17:21:35.442772 pysyd-6.10.5/PKG-INFO
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     2520 2022-11-06 15:05:08.000000 pysyd-6.10.5/README.md
+drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2023-03-23 17:21:35.437215 pysyd-6.10.5/docs/
+-rw-r--r--   0 ashleychontos   (501) staff       (20)       72 2022-03-14 21:00:31.000000 pysyd-6.10.5/docs/COLLABORATORS.rst
+-rw-r--r--   0 ashleychontos   (501) staff       (20)      486 2022-03-14 21:00:31.000000 pysyd-6.10.5/docs/CONTRIBUTORS.rst
+-rw-r--r--   0 ashleychontos   (501) staff       (20)      104 2021-04-17 02:06:06.000000 pysyd-6.10.5/pyproject.toml
+drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2023-03-23 17:21:35.438636 pysyd-6.10.5/pysyd.egg-info/
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     3565 2023-03-23 17:21:35.000000 pysyd-6.10.5/pysyd.egg-info/PKG-INFO
+-rw-r--r--   0 ashleychontos   (501) staff       (20)      682 2023-03-23 17:21:35.000000 pysyd-6.10.5/pysyd.egg-info/SOURCES.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)        1 2023-03-23 17:21:35.000000 pysyd-6.10.5/pysyd.egg-info/dependency_links.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)       41 2023-03-23 17:21:35.000000 pysyd-6.10.5/pysyd.egg-info/entry_points.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)       87 2023-03-23 17:21:35.000000 pysyd-6.10.5/pysyd.egg-info/requires.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)        6 2023-03-23 17:21:35.000000 pysyd-6.10.5/pysyd.egg-info/top_level.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)       86 2022-11-02 17:01:43.000000 pysyd-6.10.5/requirements.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)       38 2023-03-23 17:21:35.443096 pysyd-6.10.5/setup.cfg
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     1923 2022-11-03 19:41:19.000000 pysyd-6.10.5/setup.py
+drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2023-03-23 17:21:35.434551 pysyd-6.10.5/src/
+drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2023-03-23 17:21:35.440562 pysyd-6.10.5/src/pysyd/
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     1583 2023-03-23 17:21:31.000000 pysyd-6.10.5/src/pysyd/__init__.py
+-rw-r--r--   0 ashleychontos   (501) staff       (20)    56495 2023-03-23 17:16:36.000000 pysyd-6.10.5/src/pysyd/cli.py
+drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2023-03-23 17:21:35.441711 pysyd-6.10.5/src/pysyd/data/
+drwxr-xr-x   0 ashleychontos   (501) staff       (20)        0 2023-03-23 17:21:35.442450 pysyd-6.10.5/src/pysyd/data/dicts/
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     3131 2022-11-03 15:25:09.000000 pysyd-6.10.5/src/pysyd/data/dicts/columns.dict
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     3275 2022-04-20 15:18:51.000000 pysyd-6.10.5/src/pysyd/data/dicts/params.dict
+-rw-r--r--   0 ashleychontos   (501) staff       (20)      585 2022-04-20 15:18:51.000000 pysyd-6.10.5/src/pysyd/data/dicts/plots.dict
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     1205 2022-04-20 15:18:51.000000 pysyd-6.10.5/src/pysyd/data/pysyd.mplstyle
+-rw-r--r--   0 ashleychontos   (501) staff       (20)    19272 2022-04-20 15:18:51.000000 pysyd-6.10.5/src/pysyd/data/pysyd_results.csv
+-rw-r--r--   0 ashleychontos   (501) staff       (20)    58471 2022-04-20 15:18:51.000000 pysyd-6.10.5/src/pysyd/data/syd_results.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     2871 2022-10-30 15:33:28.000000 pysyd-6.10.5/src/pysyd/data/test.txt
+-rw-r--r--   0 ashleychontos   (501) staff       (20)    12076 2022-11-01 12:06:44.000000 pysyd-6.10.5/src/pysyd/models.py
+-rw-r--r--   0 ashleychontos   (501) staff       (20)     5919 2022-11-05 17:28:19.000000 pysyd-6.10.5/src/pysyd/pipeline.py
+-rw-r--r--   0 ashleychontos   (501) staff       (20)    38169 2023-03-23 17:20:58.000000 pysyd-6.10.5/src/pysyd/plots.py
+-rw-r--r--   0 ashleychontos   (501) staff       (20)   103629 2023-03-23 17:19:00.000000 pysyd-6.10.5/src/pysyd/target.py
+-rw-r--r--   0 ashleychontos   (501) staff       (20)    46309 2023-02-28 15:55:39.000000 pysyd-6.10.5/src/pysyd/utils.py
```

### Comparing `pysyd-6.10.0/CODE_OF_CONDUCT.md` & `pysyd-6.10.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/CONTRIBUTING.md` & `pysyd-6.10.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/LICENSE` & `pysyd-6.10.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/PKG-INFO` & `pysyd-6.10.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyd
-Version: 6.10.0
+Version: 6.10.5
 Summary: automated measurements of global asteroseismic parameters
 Home-page: https://github.com/ashleychontos/pysyd
 Author: Ashley Chontos
 Author-email: achontos@hawaii.edu
 License: MIT
 Project-URL: Documentation, https://pysyd.readthedocs.io
 Project-URL: Source, https://github.com/ashleychontos/pySYD
@@ -40,15 +40,15 @@
 <a href="https://github.com/ashleychontos/pySYD/graphs/contributors"><img src="https://contrib.rocks/image?repo=ashleychontos/pySYD" /></a>
 </div>
 
 --------------------------------------------------------------------------------
 
 ## Documentation
 
-The documentation for `pySYD` can be found [here](https://pysyd.readthedocs.io).
+The documentation for `pySYD` can be found [here](https://pysyd.readthedocs.io)
 
 ## Attribution
 
 If you make use of `pySYD` in your work, please cite [Chontos et al. (2021)](https://arxiv.org/abs/2108.00582):
 
     @ARTICLE{2021arXiv210800582C,
            author = {{Chontos}, Ashley and {Huber}, Daniel and {Sayeed}, Maryum and {Yamsiri}, Pavadol},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pysyd Version: 6.10.0 Summary: automated
+Metadata-Version: 2.1 Name: pysyd Version: 6.10.5 Summary: automated
 measurements of global asteroseismic parameters Home-page: https://github.com/
 ashleychontos/pysyd Author: Ashley Chontos Author-email: achontos@hawaii.edu
 License: MIT Project-URL: Documentation, https://pysyd.readthedocs.io Project-
 URL: Source, https://github.com/ashleychontos/pySYD Project-URL: Bug Tracker,
 https://github.com/ashleychontos/pySYD/issues Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -21,15 +21,15 @@
 b31b1b.svg)](https://arxiv.org/abs/2108.00582) [![JOSS](https://joss.theoj.org/
  papers/6465a9dd3141c207175f200c7f891f1e/status.svg)](https://joss.theoj.org/
      papers/6465a9dd3141c207175f200c7f891f1e) [![PyPI downloads](https://
   img.shields.io/pypi/dm/pysyd?color=purple)](https://pypistats.org/packages/
  pysyd) [ascl:2111.017] [https://contrib.rocks/image?repo=ashleychontos/pySYD]
 -------------------------------------------------------------------------------
 - ## Documentation The documentation for `pySYD` can be found [here](https://
-pysyd.readthedocs.io). ## Attribution If you make use of `pySYD` in your work,
+pysyd.readthedocs.io) ## Attribution If you make use of `pySYD` in your work,
 please cite [Chontos et al. (2021)](https://arxiv.org/abs/2108.00582): @ARTICLE
 {2021arXiv210800582C, author = {{Chontos}, Ashley and {Huber}, Daniel and
 {Sayeed}, Maryum and {Yamsiri}, Pavadol}, title = "{$\texttt{pySYD}$: Automated
 measurements of global asteroseismic parameters}", journal = {arXiv e-prints},
 keywords = {Astrophysics - Solar and Stellar Astrophysics, Astrophysics -
 Instrumentation and Methods for Astrophysics}, year = 2021, month = aug, eid =
 {arXiv:2108.00582}, pages = {arXiv:2108.00582}, archivePrefix = {arXiv}, eprint
```

### Comparing `pysyd-6.10.0/README.md` & `pysyd-6.10.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 <a href="https://github.com/ashleychontos/pySYD/graphs/contributors"><img src="https://contrib.rocks/image?repo=ashleychontos/pySYD" /></a>
 </div>
 
 --------------------------------------------------------------------------------
 
 ## Documentation
 
-The documentation for `pySYD` can be found [here](https://pysyd.readthedocs.io).
+The documentation for `pySYD` can be found [here](https://pysyd.readthedocs.io)
 
 ## Attribution
 
 If you make use of `pySYD` in your work, please cite [Chontos et al. (2021)](https://arxiv.org/abs/2108.00582):
 
     @ARTICLE{2021arXiv210800582C,
            author = {{Chontos}, Ashley and {Huber}, Daniel and {Sayeed}, Maryum and {Yamsiri}, Pavadol},
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 b31b1b.svg)](https://arxiv.org/abs/2108.00582) [![JOSS](https://joss.theoj.org/
  papers/6465a9dd3141c207175f200c7f891f1e/status.svg)](https://joss.theoj.org/
      papers/6465a9dd3141c207175f200c7f891f1e) [![PyPI downloads](https://
   img.shields.io/pypi/dm/pysyd?color=purple)](https://pypistats.org/packages/
  pysyd) [ascl:2111.017] [https://contrib.rocks/image?repo=ashleychontos/pySYD]
 -------------------------------------------------------------------------------
 - ## Documentation The documentation for `pySYD` can be found [here](https://
-pysyd.readthedocs.io). ## Attribution If you make use of `pySYD` in your work,
+pysyd.readthedocs.io) ## Attribution If you make use of `pySYD` in your work,
 please cite [Chontos et al. (2021)](https://arxiv.org/abs/2108.00582): @ARTICLE
 {2021arXiv210800582C, author = {{Chontos}, Ashley and {Huber}, Daniel and
 {Sayeed}, Maryum and {Yamsiri}, Pavadol}, title = "{$\texttt{pySYD}$: Automated
 measurements of global asteroseismic parameters}", journal = {arXiv e-prints},
 keywords = {Astrophysics - Solar and Stellar Astrophysics, Astrophysics -
 Instrumentation and Methods for Astrophysics}, year = 2021, month = aug, eid =
 {arXiv:2108.00582}, pages = {arXiv:2108.00582}, archivePrefix = {arXiv}, eprint
```

### Comparing `pysyd-6.10.0/pysyd.egg-info/PKG-INFO` & `pysyd-6.10.5/pysyd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyd
-Version: 6.10.0
+Version: 6.10.5
 Summary: automated measurements of global asteroseismic parameters
 Home-page: https://github.com/ashleychontos/pysyd
 Author: Ashley Chontos
 Author-email: achontos@hawaii.edu
 License: MIT
 Project-URL: Documentation, https://pysyd.readthedocs.io
 Project-URL: Source, https://github.com/ashleychontos/pySYD
@@ -40,15 +40,15 @@
 <a href="https://github.com/ashleychontos/pySYD/graphs/contributors"><img src="https://contrib.rocks/image?repo=ashleychontos/pySYD" /></a>
 </div>
 
 --------------------------------------------------------------------------------
 
 ## Documentation
 
-The documentation for `pySYD` can be found [here](https://pysyd.readthedocs.io).
+The documentation for `pySYD` can be found [here](https://pysyd.readthedocs.io)
 
 ## Attribution
 
 If you make use of `pySYD` in your work, please cite [Chontos et al. (2021)](https://arxiv.org/abs/2108.00582):
 
     @ARTICLE{2021arXiv210800582C,
            author = {{Chontos}, Ashley and {Huber}, Daniel and {Sayeed}, Maryum and {Yamsiri}, Pavadol},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pysyd Version: 6.10.0 Summary: automated
+Metadata-Version: 2.1 Name: pysyd Version: 6.10.5 Summary: automated
 measurements of global asteroseismic parameters Home-page: https://github.com/
 ashleychontos/pysyd Author: Ashley Chontos Author-email: achontos@hawaii.edu
 License: MIT Project-URL: Documentation, https://pysyd.readthedocs.io Project-
 URL: Source, https://github.com/ashleychontos/pySYD Project-URL: Bug Tracker,
 https://github.com/ashleychontos/pySYD/issues Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -21,15 +21,15 @@
 b31b1b.svg)](https://arxiv.org/abs/2108.00582) [![JOSS](https://joss.theoj.org/
  papers/6465a9dd3141c207175f200c7f891f1e/status.svg)](https://joss.theoj.org/
      papers/6465a9dd3141c207175f200c7f891f1e) [![PyPI downloads](https://
   img.shields.io/pypi/dm/pysyd?color=purple)](https://pypistats.org/packages/
  pysyd) [ascl:2111.017] [https://contrib.rocks/image?repo=ashleychontos/pySYD]
 -------------------------------------------------------------------------------
 - ## Documentation The documentation for `pySYD` can be found [here](https://
-pysyd.readthedocs.io). ## Attribution If you make use of `pySYD` in your work,
+pysyd.readthedocs.io) ## Attribution If you make use of `pySYD` in your work,
 please cite [Chontos et al. (2021)](https://arxiv.org/abs/2108.00582): @ARTICLE
 {2021arXiv210800582C, author = {{Chontos}, Ashley and {Huber}, Daniel and
 {Sayeed}, Maryum and {Yamsiri}, Pavadol}, title = "{$\texttt{pySYD}$: Automated
 measurements of global asteroseismic parameters}", journal = {arXiv e-prints},
 keywords = {Astrophysics - Solar and Stellar Astrophysics, Astrophysics -
 Instrumentation and Methods for Astrophysics}, year = 2021, month = aug, eid =
 {arXiv:2108.00582}, pages = {arXiv:2108.00582}, archivePrefix = {arXiv}, eprint
```

### Comparing `pysyd-6.10.0/pysyd.egg-info/SOURCES.txt` & `pysyd-6.10.5/pysyd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/setup.py` & `pysyd-6.10.5/setup.py`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/__init__.py` & `pysyd-6.10.5/src/pysyd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 """
 __url__ = "https://pysyd.readthedocs.io"
 __author__ = "Ashley Chontos<ashleychontos@astro.princeton.edu>"
 __license__ = "MIT"
 __description__ = "Automated measurements of global asteroseismic parameters"
-__version__ = '6.10.0'
+__version__ = '6.10.5'
 
 __all__ = ['cli','models','pipeline','plots','target','utils']
 
 import os
 import sys 
 
 # Directory with personal pysyd data & info
```

### Comparing `pysyd-6.10.0/src/pysyd/cli.py` & `pysyd-6.10.5/src/pysyd/cli.py`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/data/dicts/columns.dict` & `pysyd-6.10.5/src/pysyd/data/dicts/columns.dict`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/data/dicts/params.dict` & `pysyd-6.10.5/src/pysyd/data/dicts/params.dict`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/data/dicts/plots.dict` & `pysyd-6.10.5/src/pysyd/data/dicts/plots.dict`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/data/pysyd.mplstyle` & `pysyd-6.10.5/src/pysyd/data/pysyd.mplstyle`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/data/pysyd_results.csv` & `pysyd-6.10.5/src/pysyd/data/pysyd_results.csv`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/data/syd_results.txt` & `pysyd-6.10.5/src/pysyd/data/syd_results.txt`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/data/test.txt` & `pysyd-6.10.5/src/pysyd/data/test.txt`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/models.py` & `pysyd-6.10.5/src/pysyd/models.py`

 * *Files identical despite different names*

### Comparing `pysyd-6.10.0/src/pysyd/pipeline.py` & `pysyd-6.10.5/src/pysyd/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # Package mode
 from . import utils
 from . import plots
 from .target import Target
 
 
 def check(args):
-    """
+    """Check target
     
     This is intended to be a way to check a target before running it by plotting the
     times series data and/or power spectrum. This works in the most basic way  but has
     not been tested otherwise
     
     Parameters
         args : argparse.Namespace
             the command line arguments
     
     .. important::
-        has not been extensively tested
+        has not been extensively tested - also it is exactly the same as "load" so think 
+        through if this is actually needed and decided which is easier to understand
 
-    
     """
     star = load(args)
     plots.check_data(star)
 
 
 def fun(args):
     """Get logo output
@@ -44,41 +44,26 @@
             the command line arguments
     
     """
     utils.get_output(fun=True)
 
 
 def load(args):
-    """
+    """Load target
     
-    Module to load in all relevant information and dictionaries
-    required to run the pipeline
+    Load in a given target to check data or figures
     
     .. note::
         this does *not* load in a target or target data, this is purely
         information that is required to run any ``pySYD`` mode successfully
         (with the exception of ``pysyd.pipeline.setup``)
 
     Parameters
         args : argparse.Namespace
             the command line arguments
-        star : object, optional
-            pretty sure this is only used from jupyter notebook
-        verbose : bool, optional
-            again, this is only used if not using command line
-        command : str, optional
-            which of the 5 ``pysyd.pipeline`` modes to execute from the notebook
-
-    Returns
-        single : target.Target
-            current data available for the provided target
-
-    Deprecated
-        single : target.Target
-            current data available for the provided target
 
     """
     if args.data:
         if args.stars is None:
             print('\nTrying to check data but no target provided.\nPlease provide a star via --star and try again.')
             return
         else:
@@ -87,21 +72,20 @@
             print('\n\nChecking data for target %s:'%args.stars[0])
     # Load in data for a given star
     params = utils.Parameters(args=args)
     # Add target stars
     params.add_targets(stars=args.stars)
     # Load target data
     star = Target(args.stars[0], params)
-    return star
 
 
 def parallel(args):
-    """
+    """Parallel execution
     
-    Run ``pySYD`` in parallel for a large number of stars
+    Run ``pySYD`` concurrently for a large number of stars
 
     Parameters
         args : argparse.Namespace
             the command line arguments
 
     Methods
         pipe
@@ -109,31 +93,31 @@
     .. seealso:: :mod:`pysyd.pipeline.run`
     
     """
     # Load relevant pySYD parameters
     params = utils.Parameters(args=args)
     if args.stars is None:
         try:
-            args.stars = params.load_starlist()
+            args.stars = params._load_starlist()
         except utils.InputError as error:
             print(error.msg)
             return
     # Add target stars
     params.add_targets(stars=args.stars)
     # Creates the separate, asyncrhonous (nthread) processes
     pool = mp.Pool(args.n_threads)
-    result_objects = [pool.apply_async(pipe, args=(group, params)) for group in params.params['groups']]
+    result_objects = [pool.apply_async(_pipe, args=(group, params)) for group in params.params['groups']]
     results = [r.get() for r in result_objects]
     pool.close()
     pool.join()               # postpones execution of the next line until all processes finish
     # Concatenates output into two files
-    utils.scrape_output(params)
+    utils._scrape_output(params)
 
 
-def pipe(group, params, progress=False):
+def _pipe(group, params, progress=False):
     """
 
     This function is called by both :mod:`pysyd.pipeline.run` and :mod:`pysyd.pipeline.parallel`
     to initialize the pipeline for a `'group'` of stars
 
     Parameters
         group : List[str]
@@ -146,15 +130,15 @@
     for name in group:
         star = Target(name, params)
         if star.load_data():
             star.process_star()
 
 
 def plot(args):
-    """
+    """Make plots
     
     Module to load in all relevant information and dictionaries
     required to run the pipeline
     
     .. note::
         this does *not* load in a target or target data, this is purely
         information that is required to run any ``pySYD`` mode successfully
@@ -174,48 +158,49 @@
         else:
             assert len(args.stars) == 1, "No more than one star can be checked at a time."
         if args.verbose:
             print('\n\nPlotting results for target %s:'%args.stars[0])
 
 
 def run(args):
-    """
+    """Run pySYD
     
-    Main function to initiate the pySYD pipeline (consecutively, not
-    in parallel)
+    Main function to initiate the pySYD pipeline for one or many stars (the latter is run
+    consecutively *not* concurrently)
 
     Parameters
         args : argparse.Namespace
             the command line arguments
 
     Methods
-        pipe
+        :mod:`pysyd.utils.Parameters`
+        :mod:`pysyd.pipeline.pipe`
+        :mod:`pysyd.utils._scrape_output`
 
     .. seealso:: :mod:`pysyd.pipeline.parallel`
 
-
     """
     # Load default pySYD parameters
     params = utils.Parameters(args=args)
     if args.stars is None:
         try:
-            args.stars = params.load_starlist()
+            args.stars = params._load_starlist()
         except utils.InputError as error:
             print(error.msg)
             return
     # Update with CL options
     params.add_targets(stars=args.stars)
     # Run single batch of stars
-    pipe(args.stars, params)
+    _pipe(args.stars, params)
     # Concatenates output into two files
-    utils.scrape_output(params)
+    utils._scrape_output(params)
 
 
 def setup(args):
-    """
+    """Quick software setup
     
     Running this after installation will create the appropriate directories in the current working
     directory as well as download example data and files to test your pySYD installation
 
     Parameters
         args : argparse.Namespace
             the command line arguments
```

### Comparing `pysyd-6.10.0/src/pysyd/plots.py` & `pysyd-6.10.5/src/pysyd/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,31 +9,41 @@
 # Package mode
 from . import utils
 from . import models
 from . import PACKAGEDIR
 from .utils import Question
 
 
+
+
+
 MPLSTYLE = os.path.join(PACKAGEDIR,'data','pysyd.mplstyle')
 plt.style.use(MPLSTYLE)
 
 d = utils.get_dict(type='plots')
 
+
+
 def make_plots(star, show_all=False,):
     """Make plots
 
     Function that establishes the default plotting parameters and then calls each
     of the relevant plotting routines
 
     Parameters
         star : pysyd.target.Target
             the pySYD pipeline object
         showall : bool, optional
             option to plot, save and show the different background models (default=`False`)
 
+    Calls
+        :mod:`pysyd.plots.plot_estimates`
+        :mod:`pysyd.plots.plot_parameters`
+        :mod:`pysyd.plots.plot_bgfits` [optional]
+        :mod:`pysyd.plots.plot_samples`
     
     """
     if 'estimates' in star.params['plotting']:
         plot_estimates(star)
     if 'parameters' in star.params['plotting']:
         plot_parameters(star)
         if star.params['show_all']:
@@ -41,29 +51,28 @@
     if 'samples' in star.params['plotting']:
         plot_samples(star)
     if star.params['show']:
         plt.show(block=False)
 
 
 def select_trial(star):
-    """Select trial
+    r"""Select trial
 
-    This is called when ``--ask`` is `True` (i.e. select which trial to use for :math:`\rm \nu_{max}`)
-    This feature used to be called as part of a method in the `pysyd.target.Target` class but left a
+    This is called when ``--ask`` is `True` (i.e. select which trial to use for :math:`\\rm \\nu_{max}`)
+    This feature used to be called as part of a method in the :mod:`pysyd.target.Target` class but left a
     stale figure open -- this way it can be closed after the value is selected
 
     Parameters
-        star : target.Target
+        star : pysyd.target.Target
             the pySYD pipeline object
 
     Returns
         value : int or float
             depending on which `trial` was selected, this can be of integer or float type
 
-    
     """
     x, y = d[star.params['n_trials']]['x'], d[star.params['n_trials']]['y']
     params = star.params['plotting']['estimates']
 
     fig = plt.figure("Numax guesses for %s"%star.name, figsize=d[star.params['n_trials']]['size'])
     # ACF trials to determine numax
     for i in range(star.params['n_trials']):
@@ -79,38 +88,37 @@
                 ymax = max(params[i]['fity'])
             ax.axvline(params[i]['value'], color='lime', linestyle='--', linewidth=0.75)
             ax.set_title(r'$\rm Trial \,\, %d \,\, | \,\, \nu_{max} \sim %.0f \, \mu Hz $'%(i+1, params[i]['value']))
         yran = np.absolute(ymax)
         ax.set_xlim([min(params[i]['x']), max(params[i]['x'])])
         ax.set_ylim([-0.05, ymax+0.15*yran])
         ax.annotate(r'$\rm SNR = %3.2f$' % params[i]['snr'], xy=(min(params[i]['fitx'])+0.05*xran, ymax+0.025*yran), fontsize=18)
-
     plt.tight_layout()
     plt.show()
     value = Question().ask_integer('Which estimate would you like to use? ', special=True, n_trials=star.params['n_trials'])
     if isinstance(value, int):
         star.params['best'] = value
         print('Selecting model %d' % value)
     else:
         star.params['numax'] = value
         star.params['dnu'] = utils.delta_nu(value)
         print('Using numax of %.2f muHz as an initial guess' % value)
     plt.close()
     return star
 
 
-def select_trial2(star):
+def _select_trial2(star):
     """Select trial
 
     This is called when ``--ask`` is `True` (i.e. select which trial to use for :math:`\rm \nu_{max}`)
     This feature used to be called as part of a method in the `pysyd.target.Target` class but left a
     stale figure open -- this way it can be closed after the value is selected
 
     Parameters
-        star : target.Target
+        star : pysyd.target.Target
             the pySYD pipeline object
 
     Returns
         value : int or float
             depending on which `trial` was selected, this can be of integer or float type
 
     
@@ -147,19 +155,20 @@
         star.params['dnu'] = value
         print('Using dnu of %.2f muHz as an initial guess' % value)
     plt.close()
     return star
 
 
 def plot_estimates(star, filename='search_&_estimate.png', highlight=True, n=0):
-    """
+    """Plot estimates
+
     Creates a plot summarizing the results of the find excess routine.
 
     Parameters
-        star : target.Target
+        star : pysyd.target.Target
             the pySYD pipeline object
         filename : str
             the path or extension to save the figure to
         highlight : bool, default=True
             option to highlight the selected estimate
 
     
@@ -232,38 +241,36 @@
             ax.yaxis.label.set_color('lime')
             ax.xaxis.label.set_color('lime')
             ax.title.set_color('lime')
             ax.annotate(r'$\rm SNR = %3.2f$' % params[i]['snr'], xy=(min(params[i]['fitx'])+0.05*xran, ymax+0.025*yran), fontsize=18, color='lime')
         else:
             if params[i]['good_fit']:
                 ax.annotate(r'$\rm SNR = %3.2f$' % params[i]['snr'], xy=(min(params[i]['fitx'])+0.05*xran, ymax+0.025*yran), fontsize=18)
-
     plt.tight_layout()
     if star.params['save']:
         path = os.path.join(star.params['path'],filename)
         if not star.params['overwrite']:
             path = utils._get_next(path)
         plt.savefig(path, dpi=300)
     if not star.params['show']:
         plt.close()
 
 
 def plot_parameters(star, subfilename='background_only.png', filename='global_fit.png', n=0):
-    """
+    """Plot parameters
+
     Creates a plot summarizing all derived parameters
 
     Parameters
-        star : target.Target
+        star : pysyd.target.Target
             the main pipeline Target class object
         subfilename : str
             separate filename in the event that only the background is being fit
         filename : str
             the path or extension to save the figure to
-        n_peaks : int
-            the number of peaks to highlight in the zoomed-in power spectrum
 
     """
     if star.params['background'] and not star.params['globe']:
         n_panels=3
     else:
         n_panels=9
     if not star.lc:
@@ -360,28 +367,28 @@
             plt.close()
         return
 
     n += 1
     # PANEL 4: smoothed power excess 
     ax4 = fig.add_subplot(x, y, n)
     ax4.plot(params['region_freq'], params['region_pow'], 'w-', zorder=3)
-    _, f, p = utils.return_max(params['region_freq'], params['region_pow'])
+    _, f, p = utils._return_max(params['region_freq'], params['region_pow'])
     ax4.axvline([f], color='orange', linestyle='--', linewidth=1.5, zorder=4)
     ax4.scatter([f], [p], s=35.0, edgecolor='orange', marker='X', facecolor='none', linewidths=1.0, zorder=5)
-    _, ff, pp = utils.return_max(params['new_freq'], params['numax_fit'])
+    _, ff, pp = utils._return_max(params['new_freq'], params['numax_fit'])
     ax4.plot(params['new_freq'], params['numax_fit'], 'b-', zorder=0)
     ax4.axvline(ff, color='cyan', linestyle=':', linewidth=1.5, zorder=1)
     ax4.scatter([ff], [pp], s=25.0, edgecolor='cyan', marker='s', facecolor='none', linewidths=1.0, zorder=2)
     ax4.axvline(params['exp_numax'], color='r', linestyle='--', linewidth=1.5, zorder=-1, dashes=(5,5),)
     ax4.set_title(r'$\rm Smoothed \,\, PS$')
     ax4.set_xlabel(r'$\rm Frequency \,\, [\mu Hz]$')
     ax4.set_xlim([min(params['region_freq']), max(params['region_freq'])])
 
     yrange = max(params['zoom_pow'])-min(params['zoom_pow'])
-    peaks_f, peaks_p, _ = utils.max_elements(params['zoom_freq'], params['zoom_pow'], npeaks=10, distance=params['obs_dnu']/4.)
+    peaks_f, peaks_p, _ = utils._max_elements(params['zoom_freq'], params['zoom_pow'], npeaks=10, distance=params['obs_dnu']/4.)
     n += 1
     # PANEL 5: background-corrected power spectrum 
     ax5 = fig.add_subplot(x, y, n)
     ax5.plot(params['zoom_freq'], params['zoom_pow'], 'w-', zorder=0, linewidth=1.0)
     ax5.scatter(peaks_f, peaks_p, s=30.0, edgecolor='orange', marker='o', facecolor='none', linewidths=1.0)
     ax5.set_title(r'$\rm Bg$-$\rm corrected \,\, PS$')
     ax5.set_xlabel(r'$\rm Frequency \,\, [\mu Hz]$')
```

### Comparing `pysyd-6.10.0/src/pysyd/target.py` & `pysyd-6.10.5/src/pysyd/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,22 +69,28 @@
         if name in args.params:
             # load star-specific information
             self.params = args.params[name]
         else:
             # if not available, loads defaults
             self.params = utils.Parameters()
 
+
     def __repr__(self):
+        return "pysyd.target.Target(name=%r, params=%r)" % (self.name, self.params)
+
+
+    def __str__(self):
         return "<Star {}>".format(self.name)
 
 
     def _adjust_parameters(self, adjust=True, defaults=None,):
-        """ 
+        """Adjust low/high numax
     
-        Adjusts default parameters for low vs high numax configurations
+        Adjusts default parameters for low vs high numax configurations (not tested yet -
+        need to do)
 
         Parameters
             star : str
                 individual star ID
             adjust : bool, optional
                 maximum number of resolvable Harvey components
             defaults : str, optional
@@ -114,14 +120,15 @@
                 self.params['boxes'] = np.logspace(np.log10(0.5), np.log10(500.), self.params['n_trials'])
                 self.params['smooth_width'], self.params['ind_width'] = 10., 10.
                 self.params['lower_ex'], self.params['lower_bg'] = 1., 1.
                 self.params['upper_ex'], self.params['upper_bg'] = 8000., 8000.
                 self.params['smooth_ps'] = 1.5           
         """
 
+
     def load_data(self,):
         try:
             self._load_star()
         except utils.InputWarning as warning:
             print(warning.msg)
         except utils.InputError as error:
             print(error.msg)
@@ -129,35 +136,36 @@
                 try:
                     os.rmdir(self.params['outdir'])
                 except OSError:
                     pass
             return False
         return True
 
+
     def process_star(self,):
-        """Run `pySYD`
+        """Run pipeline
 
         Processes a given star with `pySYD`
 
         Methods
-            - :mod:`estimate_parameters`
-            - :mod:`derive_parameters`
-            - :mod:`show_results`
+            - :mod:`pysyd.target.Target.estimate_parameters`
+            - :mod:`pysyd.target.Target.derive_parameters`
+            - :mod:`pysyd.target.Target.show_results`
 
         """
         self.params['results'], self.params['plotting'] = {}, {}
         self.estimate_parameters()
         self.derive_parameters()
         if self.params['test']:
             return self.params['results'].pop('parameters')
         self.show_results()
 
 
     def show_results(self, show=False, verbose=False,):
-        """
+        """Show results
 
         Parameters
             show : bool, optional
                 show output figures and text
             verbose : bool, optional
                 turn on verbose output
 
@@ -179,26 +187,25 @@
         """Input star data
 
         Load data in for a single star by first checking to see if the power spectrum exists
         and then loads in the time series data, which will compute a power spectrum in the
         event that there is not one
 
         Attributes
-            lc : bool, default=False
+            lc : bool
                 `True` if object has light curve
-            ps : bool, default=False
+            ps : bool
                 `True` if object has power spectrum
 
         Methods
-            :mod:`pysyd.target.Target.load_power_spectrum`
-            :mod:`pysyd.target.Target.load_time_series`
-            :mod:`pysyd.target.Target._get_warnings`   
+            - :mod:`pysyd.target.Target.load_power_spectrum`
+            - :mod:`pysyd.target.Target.load_time_series`
 
         Raises
-            PySYDInputError
+            :mod:`pysyd.utils.InputError`
                 if no data is found for a given target   
 
         """
         self.ps, self.lc, self.note, self.note2, self.warnings = False, False, '', '', '\n##### OTHER WARNING(S): #####\n'
         self.params['data'], self.params['plotting'], self.params['results'] = {}, {}, {}
         # Now done at beginning to make sure it only does this once per star
         if glob.glob(os.path.join(self.params['inpdir'],'%s*' % str(self.name))):
@@ -215,15 +222,15 @@
         if self.params['verbose']:
             if self.warnings != '\n##### OTHER WARNING(S): #####\n' and self.params['warnings']:
                 print(self.warnings)
             print(self.note)
 
 
     def load_power_spectrum(self, long=10**6,):
-        """Load power spectrum
+        r"""Load power spectrum
     
         Loads in available power spectrum and computes relevant information -- also checks
         for time series data and will raise a warning if there is none since it will have
         to assume a :term:`critically-sampled power spectrum`
 
         Attributes
             note : str, optional
@@ -239,15 +246,15 @@
             freq_cs, pow_cs : numpy.ndarray, numpy.ndarray
                 copy of the critically-sampled power spectrum (i.e. `frequency` & `power`) 
                 iff the :term:`oversampling_factor<--of, --over, --oversample>` is provided, 
                 otherwise these arrays are just copies of `freq_os` & `pow_os` since this factor
                 isn't known and needs to be assumed
 
         Raises
-            PySYDInputWarning
+            :mod:`pysyd.utils.InputWarning`
                 if no information or time series data is provided (i.e. *has* to assume the PS is critically-sampled) 
 
         """
         # Try loading the power spectrum
         if os.path.exists(os.path.join(self.params['inpdir'], '%s_PS.txt' % str(self.name))):
             self.ps = True
             self.frequency, self.power = self.load_file(os.path.join(self.params['inpdir'], '%s_PS.txt' % str(self.name)))
@@ -272,23 +279,23 @@
                 self.baseline = 1./((self.freq_cs[1]-self.freq_cs[0])*10**-6.)
                 self.tau_upper = self.baseline/2.
                 self.params['data'].update({'freq_over':np.copy(self.freq_os),'pow_over':np.copy(self.pow_os),
                                             'freq_crit':np.copy(self.freq_cs),'pow_crit':np.copy(self.pow_cs),})
 
 
     def load_time_series(self, save=True, stitch=False, oversampling_factor=None,):
-        """Load light curve
+        r"""Load light curve
         
         Loads in time series data and calculates relevant parameters like the 
         cadence and nyquist frequency
 
         Parameters
-            save : bool, default=True
+            save : bool
                 save all data products
-            stitch : bool, default=False
+            stitch : bool
                 "stitches" together time series data with large "gaps"
             oversampling_factor : int, optional
                 oversampling factor of input power spectrum
 
         Attributes
             note : str, optional
                 verbose output
@@ -311,18 +318,18 @@
                 newly-computed frequency array using the time series array (i.e. `time` & `flux`)
             freq_os, pow_os : numpy.ndarray, numpy.ndarray
                 copy of the oversampled power spectrum (i.e. `frequency` & `power`)
             freq_cs, pow_cs : numpy.ndarray, numpy.ndarray
                 copy of the critically-sampled power spectrum (i.e. `frequency` & `power`)
 
         Raises
-            InputWarning
+            :mod:`pysyd.utils.InputWarning`
                 if the oversampling factor provided is different from that computed from the
                 time series data and power spectrum
-            InputError
+            :mod:`pysyd.utils.InputError`
                 if the oversampling factor calculated from the time series data and power 
                 spectrum is not an integer
 
 
         """
         self.nyquist = None
         # Try loading the light curve
@@ -348,23 +355,23 @@
                 self.frequency, self.power = self.compute_spectrum(oversampling_factor=self.params['oversampling_factor'], store=True)
                 if self.params['save']:
                     utils._save_file(self.frequency, self.power, os.path.join(self.params['inpdir'], '%s_PS.txt'%self.name), overwrite=self.params['overwrite'])
                 self.note += '# NEWLY COMPUTED POWER SPECTRUM has length of %d\n'%int(len(self.frequency)/5)
             else:
                 # CASE 1: LIGHT CURVE AND POWER SPECTRUM
                 #     ->  calculate oversampling factor from time series and compare
-                oversampling_factor = (1./((max(self.time)-min(self.time))*0.0864))/(self.frequency[1]-self.frequency[0])
+                oversampling_factor = int(np.ceil((1./((max(self.time)-min(self.time))*0.0864))/(self.frequency[1]-self.frequency[0])))
                 if self.params['oversampling_factor'] is not None:
-                    if int(oversampling_factor) != self.params['oversampling_factor'] and self.params['warnings']:
+                    if oversampling_factor != self.params['oversampling_factor'] and self.params['warnings']:
                         raise utils.InputWarning("\nWARNING: \ncalculated vs. provided oversampling factor do NOT match\n")
                 else:
                     if not float('%.2f'%oversampling_factor).is_integer():
                         raise utils.InputError("\nERROR: \nthe calculated oversampling factor is not an integer\nPlease check the input data and try again\n")
                     else:
-                        self.params['oversampling_factor'] = int(oversampling_factor)   
+                        self.params['oversampling_factor'] = oversampling_factor  
                 self.frequency, self.power = self.fix_data(self.frequency, self.power)
                 self.params['data'].update({'freq_fin':np.copy(self.frequency),'pow_fin':np.copy(self.power)})
             self.note += self.note2
             self.freq_os, self.pow_os = np.copy(self.frequency), np.copy(self.power)
             self.freq_cs = np.array(self.frequency[self.params['oversampling_factor']-1::self.params['oversampling_factor']])
             self.pow_cs = np.array(self.power[self.params['oversampling_factor']-1::self.params['oversampling_factor']])
             self.params['data'].update({'freq_over':np.copy(self.freq_os),'pow_over':np.copy(self.pow_os),
@@ -373,58 +380,57 @@
                 self.note += '# PS oversampled by a factor of %d'%self.params['oversampling_factor']
             else:
                 self.note += '# PS is critically-sampled'
             self.note += '\n# PS resolution: %.6f muHz'%(self.freq_cs[1]-self.freq_cs[0])
 
 
     def load_file(self, path):
-        """Load text file
+        r"""Load text file
     
         Load a light curve or a power spectrum from a basic 2xN txt file
         and stores the data into the `x` (independent variable) and `y`
         (dependent variable) arrays, where N is the length of the series
 
         Parameters
             path : str
                 the file path of the data file
 
         Returns
             x, y : numpy.ndarray, numpy.ndarray
                 the independent and dependent variables, respectively
 
-
         """
         # Open file
         with open(path, "r") as f:
             lines = f.readlines()
         # Set values
         x = np.array([float(line.strip().split()[0]) for line in lines])
         y = np.array([float(line.strip().split()[1]) for line in lines])
         return x, y
 
 
     def stitch_data(self, gap=20):
-        """Stitch light curve
+        r"""Stitch light curve
 
         For computation purposes and for special cases that this does not affect the integrity of the results,
         this module 'stitches' a light curve together for time series data with large gaps. For stochastic p-mode
         oscillations, this is justified if the lifetimes of the modes are smaller than the gap. 
 
         Parameters
-            gap : int, default=20
+            gap : int
                 how many consecutive missing cadences are considered a 'gap'
       
         Attributes
             time : numpy.ndarray
                 original time series array to correct
             new_time : numpy.ndarray
                 the corrected time series array
 
         Raises
-            PySYDInputWarning
+            :mod:`pysyd.utils.InputWarning`
                 when using this method since it's technically not a great thing to do
 
         .. warning::
             USE THIS WITH CAUTION. This is technically not a great thing to do for primarily
             two reasons:
              #. you lose phase information *and* 
              #. can be problematic if mode lifetimes are shorter than gaps (i.e. more evolved stars)
@@ -486,34 +492,39 @@
         frequency, power = self.fix_data(freq, psd)
         if store:
             self.params['data'].update({'freq_orig':np.copy(freq),'pow_orig':np.copy(psd),
                                         'freq_fin':np.copy(frequency),'pow_fin':np.copy(power)})
         return frequency, power
 
 
-    def fix_data(self, frequency, power, kep_corr=False, ech_mask=None,):
-        """Fix frequency domain data
+    def fix_data(self, frequency, power, save=True, kep_corr=False, ech_mask=None, lower_ech=None,
+                 upper_ech=None):
+        r"""Fix frequency domain data
 
         Applies frequency-domain tools to power spectra to "fix" (i.e. manipulate) the data. 
         If no available options are used, it will simply return copies of the original arrays
 
         Parameters
-            save : bool, default=True
+            save : bool
                 save all data products
-            kep_corr : bool, default=False
+            kep_corr : bool
                 correct for known *Kepler* short-cadence artefacts
-            ech_mask : List[lower_ech,upper_ech], default=None
-                corrects for dipole mixed modes if not `None`
+            ech_mask : List[lower_ech,upper_ech]
+                corrects for mixed modes if not `None`
+            lower_ech : float
+                folded lower frequency limit (~[0,dnu])
+            upper_ech : float
+                folded upper frequency limit (~[0,dnu])
             frequency, power : numpy.ndarray, numpy.ndarray
                 input power spectrum to be corrected 
 
         Methods
-            :mod:`pysyd.target.Target.remove_artefact`
+            - :mod:`pysyd.target.Target.remove_artefact`
                 mitigate known *Kepler* artefacts
-            :mod:`pysyd.target.Target.whiten_mixed` 
+            - :mod:`pysyd.target.Target.whiten_mixed` 
                 mitigate mixed modes
 	   
         Returns
             frequency, power : numpy.ndarray, numpy.ndarray
                 copy of the corrected power spectrum
 
         """
@@ -573,14 +584,15 @@
                 idx = len(df)
                 df.loc[idx,'star'], df.loc[idx,'seed'] = str(self.name), int(self.params['seed'])
         else:
             df = pd.DataFrame(columns=['star','seed'])
             df.loc[0,'star'], df.loc[0,'seed'] = str(self.name), int(self.params['seed'])
         df.to_csv(self.params['info'], index=False)
 
+
     def remove_artefact(self, freq, pow, lcp=1.0/(29.4244*60*1e-6), 
                         lf_lower=[240.0,500.0], lf_upper=[380.0,530.0], 
                         hf_lower = [4530.0,5011.0,5097.0,5575.0,7020.0,7440.0,7864.0],
                         hf_upper = [4534.0,5020.0,5099.0,5585.0,7030.0,7450.0,7867.0],):
         """Remove *Kepler* artefacts
     
         Module to remove artefacts found in *Kepler* data by replacing known frequency 
@@ -708,15 +720,14 @@
                 if numax is already known, this will automatically be skipped since it is not needed
 
         Methods
             - :mod:`pysyd.target.Target.initial_estimates`
             - :mod:`pysyd.target.Target.estimate_numax`
             - :mod:`pysyd.utils._save_estimates`
 
-
         """
         if 'results' not in self.params:
             self.params['results'] = {}
         if 'plotting' not in self.params:
             self.params['plotting'] = {}
         if self.params['estimate']:
             # get initial values and fix data
@@ -730,19 +741,19 @@
     def initial_estimates(self, lower_ex=1.0, upper_ex=8000.0, max_trials=6,):
         """Initial estimates
     
         Prepares data and parameters associated with the first module that identifies 
         solar-like oscillations and estimates :term:`numax`
 
         Parameters
-            lower_ex : float, default=1.0
+            lower_ex : float
                 the lower frequency limit of the PS used to estimate numax
-            upper_ex : float, default=8000.0
+            upper_ex : float
                 the upper frequency limit of the PS used to estimate numax
-            max_trials : int, default=6
+            max_trials : int
 	               (arbitrary) maximum number of "guesses" or trials to perform to estimate numax
 
         Attributes
             frequency, power : numpy.ndarray, numpy.ndarray
                 copy of the entire oversampled (or critically-sampled) power spectrum (i.e. `freq_os` & `pow_os`) 
             freq, pow : numpy.ndarray, numpy.ndarray
                 copy of the entire oversampled (or critically-sampled) power spectrum (i.e. `freq_os` & `pow_os`) after applying the mask~[lower_ex,upper_ex]
@@ -784,21 +795,21 @@
     def estimate_numax(self, binning=0.005, bin_mode='mean', smooth_width=20.0, ask=False,):
         """Estimate numax
 
         Automated routine to identify power excess due to solar-like oscillations and estimate
         an initial starting point for :term:`numax` (:math:`\\nu_{\\mathrm{max}}`)
 
         Parameters
-            binning : float, default=0.005
+            binning : float
                 logarithmic binning width (i.e. evenly spaced in log space)
             bin_mode : {'mean', 'median', 'gaussian'}
                 mode to use when binning
-            smooth_width: float, default=20.0
+            smooth_width: float
                 box filter width (in :math:`\\rm \\mu Hz`) to smooth power spectrum
-            ask : bool, default=False
+            ask : bool
                 If `True`, it will ask which trial to use as the estimate for numax
 
         Attributes
             bin_freq, bin_pow : numpy.ndarray, numpy.ndarray
                 copy of the power spectrum (i.e. `freq` & `pow`) binned equally in logarithmic space
             smooth_freq, smooth_pow : numpy.ndarray, numpy.ndarray
                 copy of the binned power spectrum (i.e. `bin_freq` & `bin_pow`) binned equally in linear space -- *yes, this is doubly binned intentionally*
@@ -827,37 +838,37 @@
         self.interp_pow = s(self.freq)
         self.bgcorr_pow = self.pow/self.interp_pow
         self.params['plotting'][self.module].update({'bin_freq':np.copy(self.bin_freq),
                                                      'bin_pow':np.copy(self.bin_pow),
                                                      'interp_pow':np.copy(self.interp_pow),
                                                      'bgcorr_pow':np.copy(self.bgcorr_pow)})
         # Collapsed ACF to find numax
-        self._collapsed_acf()
+        self.collapsed_acf()
         self.params['best'] = self.params['compare'].index(max(self.params['compare']))+1
         # Select trial that resulted with the highest SNR detection
         if not self.params['ask']:
             if self.params['verbose']:
                 print('Selecting model %d' % self.params['best'])
         # Or ask which estimate to use
         else:
             self = plots.select_trial(self)
 
 
-    def _collapsed_acf(self, n_trials=3, step=0.25, max_snr=100.0,):
+    def collapsed_acf(self, n_trials=3, step=0.25, max_snr=100.0,):
         """Collapsed ACF
 
         Computes a collapsed autocorrelation function (ACF) using n different box sizes in
         n different trials (i.e. `n_trials`)
 
         Parameters
-            n_trials : int, default=3
+            n_trials : int
                 the number of trials to run
-            step : float, default=0.25
+            step : float
                 fractional step size to use for the collapsed ACF calculation
-            max_snr : float, default=100.0
+            max_snr : float
                 the maximum signal-to-noise of the estimate (this is primarily for plot formatting)
 
 
         """
         self.params['compare'] = []
         # Computes a collapsed ACF using different "box" (or bin) sizes
         for b, box in enumerate(self.params['boxes']):
@@ -896,15 +907,15 @@
                 if self.params['verbose']:
                     print('Estimate %d: %.2f +/- %.2f'%(b+1, best_vars[2], np.absolute(best_vars[3])/2.0))
                     print('S/N: %.2f' % snr)
             self.params['compare'].append(snr)
 
 
     def check_numax(self, columns=['numax', 'dnu', 'snr']):
-        """Check :math:`\\rm \\nu_{max}`
+        r"""Check :math:`\\rm \\nu_{max}`
     
         Checks if there is an initial starting point or estimate for :term:`numax`
 
         Parameters
             columns : List[str]
                 saved columns if the estimate_numax() function was run
 
@@ -981,36 +992,36 @@
         # if the first step is ok, carry on
         if self.params['mc_iter'] > 1:
             self.get_samples()
         # Save results
         utils._save_parameters(self)
 
 
-    def initial_parameters(self, lower_bg=1.0, upper_bg=8000.0,):
-        """Initial guesses
+    def initial_parameters(self, module='parameters', lower_bg=1.0, upper_bg=8000.0,):
+        r"""Initial guesses
     
         Estimates initial guesses for background components (i.e. timescales and amplitudes) using
         solar scaling relations. This resets the power spectrum and has its own independent filter 
         or bounds (via [lower_bg, upper_bg]) to use for this subroutine
 
         Parameters
-            lower_bg : float, default=1.0
+            lower_bg : float
                 lower frequency limit of PS to use for the background fit
-            upper_bg : float, default=8000.0
+            upper_bg : float
                 upper frequency limit of PS to use for the background fit
 
         Attributes
             frequency, power : numpy.ndarray, numpy.ndarray
                 copy of the entire oversampled (or critically-sampled) power spectrum (i.e. `freq_os` & `pow_os`) 
             frequency, random_pow : numpy.ndarray, numpy.ndarray
                 copy of the entire oversampled (or critically-sampled) power spectrum (i.e. `freq_os` & `pow_os`) after applying the mask~[lower_bg,upper_bg]
-            module : str, default='parameters'
+            module : str
                 which part of the pipeline is currently being used
-            i : int, default=0
-                iteration number
+            i : int
+                iteration number, starts at 0
 
         Methods
             :mod:`pysyd.target.Target.solar_scaling`
                 uses multiple solar scaling relations to determnie accurate initial guesses for
                 many of the derived parameters 
 
         .. warning::
@@ -1119,29 +1130,29 @@
         self.params['nlaws'], self.params['a'] = len(self.params['mnu']), []
         self.params['plotting'][self.module].update({'exp_numax':self.params['numax'],
                                                      'nlaws_orig':len(self.params['mnu']),
                                                      'b_orig':np.copy(self.params['b'])})
 
 
     def first_step(self, background=True, globe=True,):
-        """First step
+        r"""First step
 
         Processes a given target for the first step, which has extra steps for each of the two 
         main parts of this method (i.e. background model and global fit):
          #. **background model:** the automated best-fit model selection is only performed in the
             first step, the results which are saved for future purposes (including the 
             background-corrected power spectrum)
          #. **global fit:** while the :term:`ACF` is computed for every iteration, a mask is
             created in the first step to prevent the estimate for dnu to latch on to a different 
             (i.e. incorrect) peak, since this is a multi-modal parameter space
 
         Parameters
-            background : bool, default=True
+            background : bool
                 run the automated background-fitting routine
-            globe : bool, default=True
+            globe : bool
                 perform global asteroseismic analysis (really only relevant if interested in the background model *only*)
 
         Methods
             :mod:`pysyd.target.Target.estimate_background`
                 estimates the amplitudes/levels of both correlated and frequency-independent noise
                 properties from the input power spectrum
             :mod:`pysyd.target.Target.model_background`
@@ -1161,37 +1172,38 @@
             # global fit
             self.global_fit()
             if self.params['verbose'] and self.params['mc_iter'] > 1:
                 # Set seed for reproducibility
                 self._get_seed()
                 print('-----------------------------------------------------------\nSampling routine (using seed=%d):' % int(self.params['seed']))
 
+
     def single_step(self,):
-        """Single step
+        r"""Single step
 
         Similar to the first step, this function calls the same methods but uses the selected best-fit
         background model from the first step to estimate the parameters
 
         Attributes
             converge : bool
                 removes any saved parameters if any fits did not converge (i.e. `False`)
 
         Returns
             converge : bool
                 returns `True` if all relevant fits converged
 
         Methods
-            :mod:`pysyd.target.Target.estimate_background`
+            - :mod:`pysyd.target.Target.estimate_background`
                 estimates the amplitudes/levels of both correlated and frequency-independent noise
                 properties from the input power spectrum
-            :mod:`pysyd.target.Target.get_background`
+            - :mod:`pysyd.target.Target.get_background`
                 unlike the first step, which iterated through several models and performed a
                 best-fit model comparison, this only fits parameters from the selected model 
                 in the first step
-            :mod:`pysyd.target.Target.global_fit`
+            - :mod:`pysyd.target.Target.global_fit`
                 after correcting for the background model, this derives the :term:`global asteroseismic parameters`
 
         """
         self.converge = True
         self.random_pow = (np.random.chisquare(2, len(self.frequency))*self.power)/2.
         # Background corrections
         self.estimate_background()
@@ -1203,15 +1215,15 @@
             for parameter in self.params['results'][self.module]:
                 if len(self.params['results'][self.module][parameter]) > (self.i+1):
                     p = self.params['results'][self.module][parameter].pop(-1)
         return self.converge
 
 
     def get_samples(self,):
-        """Get samples
+        r"""Get samples
 
         Estimates uncertainties for parameters by randomizing the power spectrum and
         attempting to recover the same parameters by calling the :mod:`pysyd.target.Target.single_step`
 
         Attributes
             frequency, power : numpy.ndarray, numpy.ndarray
                 copy of the critically-sampled power spectrum (i.e. `freq_cs` & `pow_cs`) after applying the mask~[lower_bg,upper_bg]
@@ -1249,21 +1261,22 @@
     def estimate_background(self, ind_width=20.0,):
         """Background estimates
 
         Estimates initial guesses for the stellar background contributions for both the
         red and white noise components
 
         Parameters
-            ind_width : float, default=20.0
+            ind_width : float
                 the independent average smoothing width (:math:`\\rm \\mu Hz`)
 
         Attributes
             bin_freq, bin_pow, bin_err : numpy.ndarray, numpy.ndarray, numpy.ndarray
                 binned power spectrum using the :term:`ind_width<--iw, --indwidth>` bin size   
 
+        Methods
 
         """
         # Bin power spectrum to model stellar background/correlated red noise components
         self.bin_freq, self.bin_pow, self.bin_err = utils._bin_data(self.frequency, self.random_pow, width=self.params['ind_width'], mode=self.params['bin_mode'])
         # Mask out region with power excess
         mask = np.ma.getmask(np.ma.masked_outside(self.bin_freq, self.params['ps_mask'][0], self.params['ps_mask'][1]))
         self.bin_freq, self.bin_pow, self.bin_err = self.bin_freq[mask], self.bin_pow[mask], self.bin_err[mask]
@@ -1287,17 +1300,17 @@
         """Estimate red noise
 
         Estimates amplitudes of red noise components by using a smoothed version of the power
         spectrum with the power excess region masked out -- which will take the mean of a specified 
         number of points (via -nrms, default=20) for each Harvey-like component
 
         Parameters
-            box_filter : float, default=1.0
+            box_filter : float
                 the size of the 1D box smoothing filter
-            n_rms : int, default=20
+            n_rms : int
                 number of data points to average over to estimate red noise amplitudes 
 
         Attributes
             smooth_pow : numpy.ndarray
                 smoothed power spectrum after applying the box filter
 
 
@@ -1328,23 +1341,23 @@
 
         If nothing is fixed, this method iterates through :math:`2\\dot(n_{\\mathrm{laws}}+1)` 
         models to determine the best-fit background model due to stellar granulation processes,
         which uses a solar scaling relation to estimate the number of Harvey-like component(s) 
         (or `n_laws`)
 
         Parameters
-            n_laws : int, default=None
+            n_laws : int
                 specify number of Harvey-like components to use in background fit 
-            fix_wn : bool, default=False
+            fix_wn : bool
                 option to fix the white noise instead of it being an additional free parameter 
-            basis : str, default='tau_sigma'
+            basis : str
                 which basis to use for background fitting, e.g. {a,b} parametrization **TODO: not yet operational**
 
         Methods
-            :mod:`pysyd.models.background`
+            - :mod:`pysyd.models.background`
             - :mod:`scipy.curve_fit`
             - :mod:`pysyd.models._compute_aic`
             - :mod:`pysyd.models._compute_bic`
             - :mod:`pysyd.target.Target.correct_background`
 
         Returns
             converge : bool
@@ -1429,15 +1442,15 @@
             self.bg_corr = np.copy(self.random_pow)/self.params['noise']
             self.params['pars'] = ([self.params['noise']])
         # save final guesses for plotting purposes
         self.params['plotting'][self.module].update({'pars':self.params['pars'],})
 
 
     def correct_background(self, metric='bic'):
-        """Correct background
+        r"""Correct background
 
         Corrects for the stellar background contribution in the power spectrum by *both*
         dividing and subtracting this out, which also saves copies of each (i.e. `bg_div`
         :term:`background-divided power spectrum` to :ref:`ID_BDPS.txt <library-output-files-bdps>`
         and `bg_sub` :term:`background-subtracted power spectrum to 
         :ref:`ID_BSPS.txt <library-output-files-bsps>`). After this is done, a copy of the
         BDPS is saved to `bg_corr` and used for dnu calculations and the echelle diagram.
@@ -1469,18 +1482,18 @@
             self.params['b'] = self.params['b'][:(self.params['nlaws'])]
             self.params['mnu'] = self.params['mnu'][:(self.params['nlaws'])]
         if self.params['verbose'] and len(self.params['models']) > 1:
             print('Based on %s statistic: model %d'%(self.params['metric'].upper(),idx))
         # Save background-corrected power spectrum
         self.bg_div = self.random_pow/models.background(self.frequency, self.params['pars'], noise=self.params['noise'])
         if self.params['save']:
-            utils.save_file(self.frequency, self.bg_div, os.path.join(self.params['path'], '%s_BDPS.txt'%self.name), overwrite=self.params['overwrite'])
+            utils._save_file(self.frequency, self.bg_div, os.path.join(self.params['path'], '%s_BDPS.txt'%self.name), overwrite=self.params['overwrite'])
         self.bg_sub = self.random_pow-models.background(self.frequency, self.params['pars'], noise=self.params['noise'])
         if self.params['save']:
-            utils.save_file(self.frequency, self.bg_sub, os.path.join(self.params['path'], '%s_BSPS.txt'%self.name), overwrite=self.params['overwrite'])
+            utils._save_file(self.frequency, self.bg_sub, os.path.join(self.params['path'], '%s_BSPS.txt'%self.name), overwrite=self.params['overwrite'])
         self.params['plotting'][self.module].update({'models':self.params['models'],
                                                      'model':self.params['selected'],
                                                      'paras':self.params['paras'],
                                                      'aic':self.params['aic'],
                                                      'bic':self.params['bic'],})
         # For the rest of the calculations, we'll use the background-divided power spectrum
         self.bg_corr = np.copy(self.bg_div)
@@ -1536,18 +1549,18 @@
     def global_fit(self):
         """Global fit
 
         Fits global asteroseismic parameters :math:`\\rm \\nu{max}` and :math:`\\Delta\\nu`,
         where the former is estimated two different ways.
 
         Methods
-            :mod:`numax_smooth`
-            :mod:`numax_gaussian`
-            :mod:`compute_acf`
-            :mod:`frequency_spacing`
+            :mod:`pysyd.target.Target.numax_smooth`
+            :mod:`pysyd.target.Target.numax_gaussian`
+            :mod:`pysyd.target.Target.compute_acf`
+            :mod:`pysyd.target.Target.frequency_spacing`
 
 
         """
         # get numax
         self.numax_smooth()
         self.numax_gaussian()
         # get dnu
@@ -1585,15 +1598,15 @@
         if sm_par < 1.:
             sm_par = 1.
         sig = (sm_par*(self.params['dnu']/self.params['resolution']))/np.sqrt(8.0*np.log(2.0))
         self.pssm = convolve_fft(np.copy(self.random_pow), Gaussian1DKernel(int(sig)))
         self.pssm_bgcorr = self.pssm-models.background(self.frequency, self.params['pars'], noise=self.params['noise'])
         mask = np.ma.getmask(np.ma.masked_inside(self.frequency, self.params['ps_mask'][0], self.params['ps_mask'][1]))
         self.region_freq, self.region_pow = self.frequency[mask], self.pssm_bgcorr[mask]
-        idx, max_freq, max_pow = utils.return_max(self.region_freq, self.region_pow)
+        idx, max_freq, max_pow = utils._return_max(self.region_freq, self.region_pow)
         self.params['results'][self.module]['numax_smooth'].append(max_freq)
         self.params['results'][self.module]['A_smooth'].append(max_pow)
         self.params['numax_smoo'] = self.params['results'][self.module]['numax_smooth'][0]
         self.params['exp_dnu'] = utils.delta_nu(self.params['numax_smoo'])
 
 
     def numax_gaussian(self):
@@ -1709,19 +1722,19 @@
            automatically computed and applied by the pipeline to prevent the fit from latching 
            on to a peak that is a harmonic and not the actual spacing
 
 
         """
         if self.i == 0:
             # Get actual peaks from ACF for plotting purposes before any weighting
-            pl, pa, _ = utils.max_elements(self.lag, self.auto, npeaks=self.params['n_peaks'], distance=self.params['exp_dnu']/4.)
+            pl, pa, _ = utils._max_elements(self.lag, self.auto, npeaks=self.params['n_peaks'], distance=self.params['exp_dnu']/4.)
             # Get peaks from ACF by providing dnu to weight the array 
-            peaks_l, peaks_a, weights = utils.max_elements(self.lag, self.auto, npeaks=self.params['n_peaks'], distance=self.params['exp_dnu']/4., exp_dnu=self.params['exp_dnu'])
+            peaks_l, peaks_a, weights = utils._max_elements(self.lag, self.auto, npeaks=self.params['n_peaks'], distance=self.params['exp_dnu']/4., exp_dnu=self.params['exp_dnu'])
             # Pick "best" peak in ACF (i.e. closest to expected dnu)
-            idx , self.params['best_lag'], self.params['best_auto'] = utils.return_max(peaks_l, peaks_a, exp_dnu=self.params['exp_dnu'])
+            idx , self.params['best_lag'], self.params['best_auto'] = utils._return_max(peaks_l, peaks_a, exp_dnu=self.params['exp_dnu'])
             self._acf_cutout()
         self.zoom_lag = self.lag[(self.lag >= self.params['acf_mask'][0]) & (self.lag <= self.params['acf_mask'][1])]
         self.zoom_auto = self.auto[(self.lag >= self.params['acf_mask'][0]) & (self.lag <= self.params['acf_mask'][1])]
         # fit a Gaussian to the peak to estimate dnu
         try:
             gauss, _ = curve_fit(models.gaussian, self.zoom_lag, self.zoom_auto, p0=self.params['acf_guesses'], bounds=self.params['acf_bb'], maxfev=1000)
         # did the fit converge
@@ -1731,15 +1744,15 @@
             # Raise error if it's the first step
                 raise utils.ProcessingError("Gaussian fit for dnu failed to converge.\n\nPlease check your power spectrum and try again.")
         # if fit converged, save appropriate results
         else:
             self.params['results'][self.module]['dnu'].append(gauss[2]) 
             if self.i == 0:
                 self.params['obs_dnu'] = gauss[2]
-                idx, _, _ = utils.return_max(pl, pa, exp_dnu=self.params['obs_dnu'])
+                idx, _, _ = utils._return_max(pl, pa, exp_dnu=self.params['obs_dnu'])
                 l, a = pl.pop(idx), pa.pop(idx)
                 self.params['plotting'][self.module].update({'obs_dnu':gauss[2], 
                   'peaks_l':np.copy(pl),'peaks_a':np.copy(pa),'best_lag':self.params['best_lag'],
                   'best_auto':self.params['best_auto'],'weights':np.copy(weights/max(weights)),
                   'new_lag':np.linspace(min(self.zoom_lag),max(self.zoom_lag),2000), 
                   'dnu_fit':models.gaussian(np.linspace(min(self.zoom_lag),max(self.zoom_lag),2000), *gauss),})
                 self.echelle_diagram()
```

### Comparing `pysyd-6.10.0/src/pysyd/utils.py` & `pysyd-6.10.5/src/pysyd/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,23 +90,19 @@
         return "<Constants>"
 
     def __repr__(self):
         return "utils.Constants()"
 
 
 class Parameters(Constants):
-    """
-
-    Container class for ``pySYD``
+    """Container class for ``pySYD`` parameters
 
     """
-
     def __init__(self, args=None):
         """
-
         Calls super method to inherit all relevant constants and then
         stores the default values for all pysyd modules
 
         Methods
 
         """
         # makes sure to inherit constants
@@ -123,16 +119,16 @@
     def __repr__(self):
         return "utils.Parameters(Constants, params={})"
 
 
     def get_defaults(self):
         """Load defaults
 
-        Gets default pySYD parameters by calling functions analogous to the command-line 
-        parsers 
+        Gets default pySYD parameters by calling functions which are analogous to 
+        available command-line parsers and arguments
 
         Attributes
             params : Dict[str[Dict[,]]]
                 container class for ``pySYD`` parameters
     
         Calls
             - :mod:`pysyd.utils.Parameters.get_parent`
@@ -148,24 +144,24 @@
         self.get_data()
         # Initialize main 'params' dictionary
         self.get_main()
         # Get plotting info
         self.get_plot()
 
 
-    def get_parent(self):
+    def get_parent(self, inpdir='data', infdir='info', outdir='results', save=True, test=False,
+                   verbose=False, overwrite=False, warnings=False, cli=True, notebook=False):
         """Get parent parser
    
         Load parameters available in the parent parser i.e. higher-level software functionality
 
         Attributes
             params : Dict[str,Dict[,]]
                 the updated parameters
 
-
         """
         self.params.update({
             'inpdir' : os.path.join(_ROOT, 'data'),
             'infdir' : os.path.join(_ROOT, 'info'),
             'outdir' : os.path.join(_ROOT, 'results'),
             'save' : True,
             'test' : False,
@@ -173,25 +169,26 @@
             'overwrite' : False,
             'warnings' : False,
             'cli' : True,
             'notebook' : False,
         })
 
 
-    def get_data(self):
+    def get_data(self, info='info/star_info.csv', todo='info/todo.txt', stars=None, mode='run',
+                 gap=20, stitch=False, oversampling_factor=None, kep_corr=False, notching=False,
+                 dnu=None, lower_ech=None, upper_ech=None):
         """Get data parser
    
         Load parameters available in the data parser, which is mostly related to initial
         data loading and manipulation
 
         Attributes
             params : Dict[str,Dict[,]]
                 the updated parameters
 
-
         """
         self.params.update({
             'info' : os.path.join(_ROOT, 'info', 'star_info.csv'),
             'todo' : os.path.join(_ROOT, 'info', 'todo.txt'),
             'stars' : None,
             'mode' : 'run',
             'gap' : 20,
@@ -217,27 +214,27 @@
 
         Calls
             - :mod:`pysyd.utils.Parameters.get_estimate`
             - :mod:`pysyd.utils.Parameters.get_background`
             - :mod:`pysyd.utils.Parameters.get_global`
             - :mod:`pysyd.utils.Parameters.get_sampling`
 
-
         """
         # Initialize parameters for the estimate routine
         self.get_estimate()
         # Initialize parameters for the fit background routine
         self.get_background()
         # Initialize parameters relevant for estimating global parameters
         self.get_global()
         # Estimate parameters
         self.get_sampling()
 
 
-    def get_estimate(self):
+    def get_estimate(self, estimate=True, smooth_width=20.0, binning=0.005, bin_mode='mean', step=0.25,
+                     n_trials=3, ask=False, lower_ex=None, upper_ex=None):
         """Search and estimate parameters
     
         Get parameters relevant for the optional first module that looks for and identifies
         power excess due to solar-like oscillations and then estimates its properties 
 
         Attributes
             params : Dict[str,Dict[,]]
@@ -253,15 +250,16 @@
             'n_trials' : 3,
             'ask' : False,
             'lower_ex' : None,
             'upper_ex' : None,
         })
 
 
-    def get_background(self):
+    def get_background(self, background=True, basis='tau_sigma', box_filter=1.0, ind_width=20.0, n_rms=20,
+                       n_laws=None, fix_wn=False, metric='bic', lower_bg=None, upper_bg=None, functions=None):
         """Background parameters
     
         Gets parameters used during the automated background-fitting analysis 
 
         Attributes
             params : Dict[str,Dict[,]]
                 the updated parameters
@@ -278,15 +276,16 @@
             'metric' : 'bic',
             'lower_bg' : None,
             'upper_bg' : None,
             'functions' : get_dict(type='functions'),
         })
 
 
-    def get_global(self):
+    def get_global(self, globe=True, numax=None, lower_ps=None, upper_ps=None, ex_width=1.0, 
+                   sm_par=None, smooth_ps=2.5, fft=True, threshold=1.0, n_peaks=5):
         """Global fitting parameters
     
         Get default parameters that are relevant for deriving global asteroseismic parameters 
         :math:`\\rm \\nu_{max}` and :math:`\\Delta\\nu`
 
         Attributes
             params : Dict[str,Dict[,]]
@@ -303,34 +302,34 @@
             'smooth_ps' : 2.5,
             'fft' : True,
             'threshold' : 1.0,
             'n_peaks' : 5,
         })
 
 
-    def get_sampling(self):
+    def get_sampling(self, mc_iter=1, seed=None, samples=False, n_threads=0):
         """Sampling parameters
     
         Get parameters relevant for the sampling steps i.e. estimating uncertainties
 
         Attributes
             params : Dict[str,Dict[,]]
                 the updated parameters
 
-
         """
         self.params.update({
             'mc_iter' : 1,
             'seed' : None,
             'samples' : False,
             'n_threads' : 0,
         })
 
 
-    def get_plot(self):
+    def get_plot(self, show_all=False, show=False, cmap='binary', hey=False, clip_value=3.0,
+                 interp_ech=False, nox=None, noy='0+0', npb=10, ridges=False, smooth_ech=None):
         """Get plot parser
     
         Save all parameters related to any of the output figures
 
         Attributes
             params : Dict[str,Dict[,]]
                 the updated parameters
@@ -358,33 +357,32 @@
         in the override columns since those are star specific and have a given length --
         it will come back to this
 
         Parameters
             args : argparse.Namespace
                 the command line arguments
 
-
         """
         self.check_cli(args)
         # CLI options overwrite defaults
         for key, value in args.__dict__.items():
             # Make sure it is not a variable with a >1 length
             if key not in self.override:
                 self.params[key] = value
 
 
-    def check_cli(self, args, max_laws=3):
+    def check_cli(self, args, max_laws=3, override=['numax','dnu','lower_ex','upper_ex','lower_bg','upper_bg','lower_ps','upper_ps','lower_ech','upper_ech']):
         """Check CLI
     
         Make sure that any command-line inputs are the proper lengths, types, etc.
 
         Parameters
             args : argparse.Namespace
                 the command line arguments
-            max_laws : int, default=3
+            max_laws : int
                 maximum number of Harvey laws to be fit
 
         Asserts
             - the length of each array provided (in override) is equal
             - the oversampling factor is an integer (if applicable)
             - the number of Harvey laws to "force" is an integer (if applicable)
 
@@ -398,18 +396,18 @@
             'upper_bg': args.upper_bg,
             'lower_ps': args.lower_ps,
             'upper_ps': args.upper_ps,
             'lower_ech': args.lower_ech,
             'upper_ech': args.upper_ech,
         }
         for each in self.override:
-            if self.override[each] is not None:
-                raise InputError("\nWhen running multiple stars via command line, the number \n of values provided for %s MUST equal the number of stars\n" % each)
+            if self.override[each] and len(self.override[each]) != len(args.stars):
+                raise InputError("\nThe number \n of values provided for %s MUST equal the number of stars\n" % each)
         if args.oversampling_factor is not None and not isinstance(args.oversampling_factor, int):
-            raise InputError("\nThe oversampling factor for the input PS must be an integer\n")
+            raise InputError("\nOversampling factor for input PS must be an integer\n")
         if args.n_laws is not None and args.n_laws > max_laws:
             args.n_laws = max_laws
             raise InputWarning("\nWe probs cannot resolve %d Harvey components. \nnlaws changed to %d\n" % max_laws)
 
 
     def add_targets(self, stars=None):
         """Add targets
@@ -422,24 +420,24 @@
             if stars is not None:
                 if isinstance(stars, list):
                     self.params['stars'] = stars
                 else:
                     self.params['stars'] = [stars]
             else:
                 try:
-                    loadstars = self.load_starlist()
+                    loadstars = self._load_starlist()
                 except InputError as error:
                     print(error.msg)
                     return
                 else:
                     self.params['stars'] = loadstars
-        self.make_dicts()
+        self._make_dicts()
 
 
-    def load_starlist(self):
+    def _load_starlist(self):
         """Load star list
 
         If no stars have been provided yet, it will read in the default text file
         (and if that does not exist, it will raise an error)
 
         """
         if not os.path.exists(self.params['todo']):
@@ -447,35 +445,34 @@
             return None
         else:
             with open(self.params['todo'], "r") as f:
                 stars = [line.strip().split()[0] for line in f.readlines()]
             return stars
 
 
-    def make_dicts(self):
+    def _make_dicts(self):
         """Add star dicts
 
         This routine will load in target stars, sets up "groups" (relevant for parallel
         processing) and then load in all relevant information
 
-
         """
         # Set file paths and make directories if they don't yet exist
         for star in self.params['stars']:
             self.params[star] = {}
             self.params[star]['path'] = os.path.join(self.params['outdir'], str(star))
             if self.params['save'] and not os.path.exists(self.params[star]['path']):
                 os.makedirs(self.params[star]['path'])
-        self.get_groups()
-        self.load_starinfo()
-        self.load_clinfo()
-        self.add_derived()
+        self._get_groups()
+        self._load_starinfo()
+        self._load_clinfo()
+        self._add_derived()
 
 
-    def get_groups(self):
+    def _get_groups(self):
         """Get star groups
     
         Mostly relevant for parallel processing -- which sets up star groups to run 
         in parallel based on the number of threads
 
         """
         if hasattr(self, 'mode') and self.params['mode'] == 'parallel':
@@ -487,15 +484,15 @@
             # divide stars into groups set by number of cpus/nthreads available
             digitized = np.digitize(np.arange(len(todo)) % self.params['n_threads'], np.arange(self.params['n_threads']))
             self.params['groups'] = np.array([todo[digitized == i] for i in range(1, self.params['n_threads']+1)], dtype=object)
         else:
             self.params['groups'] = np.array(self.params['stars'])
 
 
-    def load_starinfo(self):
+    def _load_starinfo(self):
         """Load star info csv
 
         """
         if os.path.exists(self.params['info']):
             columns = get_dict(type='columns')
             df = pd.read_csv(self.params['info'])
             stars = [str(star) for star in df.star.values.tolist()]
@@ -511,15 +508,15 @@
                             self.params[star][column] = df.loc[idx,column]
                         elif not np.isnan(df.loc[idx,column]) and column in columns['str']:
                             self.params[star][column] = str(df.loc[idx,column])
                         else:
                             pass
 
 
-    def load_clinfo(self):
+    def _load_clinfo(self):
         """Load command-line values
 
         """
         columns = get_dict(type='columns')
         # make sure all keys exist, even if they are None
         for star in self.params['stars']:
             for column in columns['all']:
@@ -532,15 +529,15 @@
         if hasattr(self, 'override'):
             for column in columns['override']:
                 if self.override[column] is not None:
                     for i, star in enumerate(self.params['stars']):
                         self.params[star][column] = self.override[column][i]
 
 
-    def add_derived(self):
+    def _add_derived(self):
         """Add derived properties
 
         """
         for star in self.params['stars']:
             if self.params[star]['numax'] is not None:
                 self.params[star]['estimate'] = False
                 if self.params[star]['dnu'] is None:
@@ -712,15 +709,15 @@
                 7: lambda frequency, tau_1, sigma_1, tau_2, sigma_2, tau_3, sigma_3, white_noise : models.harvey_three(frequency, tau_1, sigma_1, tau_2, sigma_2, tau_3, sigma_3, white_noise),
                }
     path = os.path.join(PACKAGEDIR, 'data', 'dicts', '%s.dict'%type)
     with open(path, 'r') as f:
         return ast.literal_eval(f.read())
 
 
-def save_file(x, y, path, overwrite=False, formats=[">15.8f", ">18.10e"]):
+def _save_file(x, y, path, overwrite=False, formats=[">15.8f", ">18.10e"]):
     """Saves basic text files
     
     After determining the best-fit stellar background model, this module
     saved the background-subtracted power spectrum
 
     Parameters
         x : numpy.ndarray
@@ -864,15 +861,15 @@
         line = '\n%s: %.2f %s'
         for idx in df.index.values.tolist():
             note += line%(df.loc[idx,'parameter'], df.loc[idx,'value'], params[df.loc[idx,'parameter']]['unit'])
     note+='\n-----------------------------------------------------------'
     print(note)
 
 
-def scrape_output(args, columns=['star','numax','dnu','snr']):
+def _scrape_output(args, columns=['star','numax','dnu','snr']):
     """Concatenate results
     
     Automatically concatenates and summarizes the results for all processed stars in each
     of the two submodules
 
     Methods
         :mod:`pysyd.utils._sort_table`
@@ -925,15 +922,15 @@
     """
     df.to_csv(os.path.join(outdir,'%s.csv'%type), index=False)
     df_new = pd.read_csv(os.path.join(outdir,'%s.csv'%type))
     df_new.sort_values(by=['star'], ascending=[True], inplace=True)
     df_new.to_csv(os.path.join(outdir,'%s.csv'%type), index=False)
 
 
-def max_elements(x, y, npeaks, distance=None, exp_dnu=None):
+def _max_elements(x, y, npeaks, distance=None, exp_dnu=None):
     """N highest peaks
     
     Module to obtain the x and y values for the n highest peaks in a 2D array 
 
     Parameters
         x, y : numpy.ndarray, numpy.ndarray
             the series of data to identify peaks in
@@ -967,15 +964,15 @@
     # sort by n highest peaks
     s = np.argsort(py)
     peaks_y = py[s][-int(npeaks):][::-1]
     peaks_x = px[s][-int(npeaks):][::-1]
     return list(peaks_x), list(peaks_y), weights
 
 
-def return_max(x, y, exp_dnu=None,):
+def _return_max(x, y, exp_dnu=None,):
     """Return max
     
     Return the peak (and/or the index of the peak) in a given 2D array
 
     Parameters
         x, y : numpy.ndarray, numpy.ndarray
             the independent and dependent axis, respectively
@@ -1110,14 +1107,19 @@
 
     Returns
         dl_dict : Dict[str,str]
             dictionary of files to download for setup
         note : str
             updated verbose output
 
+    Calls
+        - :mod:`pysyd.utils.get_infdir`
+        - :mod:`pysyd.utils.get_inpdir`
+        - :mod:`pysyd.utils.get_outdir`
+
     """
     dl_dict, note = get_infdir(args, dl_dict, note)
     dl_dict, note = get_inpdir(args, dl_dict, note)
     note = get_outdir(args, note)
     # Download files that do not already exist
     if dl_dict:
         # downloading example data will generate output in terminal, so always include this regardless
```

