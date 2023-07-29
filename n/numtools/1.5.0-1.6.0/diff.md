# Comparing `tmp/numtools-1.5.0.tar.gz` & `tmp/numtools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numtools-1.5.0.tar", last modified: Fri May 12 11:26:38 2023, max compression
+gzip compressed data, was "numtools-1.6.0.tar", last modified: Sat Jul 29 09:35:18 2023, max compression
```

## Comparing `numtools-1.5.0.tar` & `numtools-1.6.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.330726 numtools-1.5.0/
--rw-r--r--   0 nic       (1001) nic       (1001)      172 2019-11-19 09:06:07.000000 numtools-1.5.0/AUTHORS.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      221 2019-11-19 09:06:07.000000 numtools-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      285 2019-12-16 06:53:49.000000 numtools-1.5.0/HISTORY.rst
--rw-r--r--   0 nic       (1001) nic       (1001)     1074 2019-12-13 10:28:35.000000 numtools-1.5.0/LICENSE
--rw-r--r--   0 nic       (1001) nic       (1001)      262 2019-11-19 09:06:07.000000 numtools-1.5.0/MANIFEST.in
--rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-05-12 11:26:38.330726 numtools-1.5.0/PKG-INFO
--rw-r--r--   0 nic       (1001) nic       (1001)      681 2019-12-16 06:52:44.000000 numtools-1.5.0/README.rst
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.326726 numtools-1.5.0/docs/
--rw-r--r--   0 nic       (1001) nic       (1001)      609 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/Makefile
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.322725 numtools-1.5.0/docs/_build/
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.322725 numtools-1.5.0/docs/_build/html/
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.330726 numtools-1.5.0/docs/_build/html/_static/
--rw-r--r--   0 nic       (1001) nic       (1001)      286 2019-12-16 16:19:06.000000 numtools-1.5.0/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.5.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.5.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/authors.rst
--rwxr-xr-x   0 nic       (1001) nic       (1001)     4900 2022-10-12 15:49:49.000000 numtools-1.5.0/docs/conf.py
--rw-r--r--   0 nic       (1001) nic       (1001)       33 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/contributing.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/history.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      305 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/index.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      102 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/installation.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      770 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/make.bat
--rw-r--r--   0 nic       (1001) nic       (1001)       61 2020-01-15 10:31:32.000000 numtools-1.5.0/docs/modules.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      136 2020-01-15 10:31:32.000000 numtools-1.5.0/docs/numtools.csyslib.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      133 2020-01-15 10:31:32.000000 numtools-1.5.0/docs/numtools.intzip.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      270 2020-01-15 10:31:32.000000 numtools-1.5.0/docs/numtools.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.5.0/docs/numtools.serializer.rst
--rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.5.0/docs/numtools.vgextended.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       27 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/readme.rst
--rw-r--r--   0 nic       (1001) nic       (1001)       71 2019-11-19 09:06:07.000000 numtools-1.5.0/docs/usage.rst
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.330726 numtools-1.5.0/numtools/
--rw-rw-r--   0 nic       (1001) nic       (1001)      167 2023-05-12 11:25:44.000000 numtools-1.5.0/numtools/__init__.py
--rw-rw-r--   0 nic       (1001) nic       (1001)    18162 2023-05-12 11:23:41.000000 numtools-1.5.0/numtools/csyslib.py
--rw-r--r--   0 nic       (1001) nic       (1001)     5932 2022-10-12 15:49:45.000000 numtools-1.5.0/numtools/intzip.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     4406 2023-05-02 04:11:56.000000 numtools-1.5.0/numtools/pandas_tk.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     9152 2022-10-12 15:49:49.000000 numtools-1.5.0/numtools/serializer.py
--rw-r--r--   0 nic       (1001) nic       (1001)     5315 2023-03-13 09:11:17.000000 numtools-1.5.0/numtools/vgextended.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.330726 numtools-1.5.0/numtools.egg-info/
--rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-05-12 11:26:38.000000 numtools-1.5.0/numtools.egg-info/PKG-INFO
--rw-rw-r--   0 nic       (1001) nic       (1001)      950 2023-05-12 11:26:38.000000 numtools-1.5.0/numtools.egg-info/SOURCES.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-05-12 11:26:38.000000 numtools-1.5.0/numtools.egg-info/dependency_links.txt
--rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-05-12 11:26:38.000000 numtools-1.5.0/numtools.egg-info/not-zip-safe
--rw-rw-r--   0 nic       (1001) nic       (1001)        9 2023-05-12 11:26:38.000000 numtools-1.5.0/numtools.egg-info/top_level.txt
--rw-r--r--   0 nic       (1001) nic       (1001)      483 2023-05-12 11:26:38.330726 numtools-1.5.0/setup.cfg
--rw-rw-r--   0 nic       (1001) nic       (1001)     1229 2023-05-12 11:25:44.000000 numtools-1.5.0/setup.py
-drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-05-12 11:26:38.330726 numtools-1.5.0/tests/
--rw-r--r--   0 nic       (1001) nic       (1001)       63 2019-11-19 09:06:07.000000 numtools-1.5.0/tests/__init__.py
--rw-r--r--   0 nic       (1001) nic       (1001)     2559 2022-10-12 15:49:45.000000 numtools-1.5.0/tests/test_csyslib.py
--rw-rw-r--   0 nic       (1001) nic       (1001)      967 2022-10-12 09:19:37.000000 numtools-1.5.0/tests/test_intzip.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     1469 2023-03-13 09:09:12.000000 numtools-1.5.0/tests/test_matrix.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     2567 2023-01-19 14:44:08.000000 numtools-1.5.0/tests/test_pandas_tk.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3529 2022-10-12 15:49:49.000000 numtools-1.5.0/tests/test_serializer.py
--rw-rw-r--   0 nic       (1001) nic       (1001)     3599 2022-10-12 15:49:45.000000 numtools-1.5.0/tests/test_serializer.py.orig
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.448361 numtools-1.6.0/
+-rw-r--r--   0 nic       (1001) nic       (1001)      172 2019-11-19 09:06:07.000000 numtools-1.6.0/AUTHORS.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      221 2019-11-19 09:06:07.000000 numtools-1.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      285 2019-12-16 06:53:49.000000 numtools-1.6.0/HISTORY.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)     1074 2019-12-13 10:28:35.000000 numtools-1.6.0/LICENSE
+-rw-r--r--   0 nic       (1001) nic       (1001)      262 2019-11-19 09:06:07.000000 numtools-1.6.0/MANIFEST.in
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-07-29 09:35:18.448361 numtools-1.6.0/PKG-INFO
+-rw-r--r--   0 nic       (1001) nic       (1001)      681 2019-12-16 06:52:44.000000 numtools-1.6.0/README.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.444361 numtools-1.6.0/docs/
+-rw-r--r--   0 nic       (1001) nic       (1001)      609 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/Makefile
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.440361 numtools-1.6.0/docs/_build/
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.440361 numtools-1.6.0/docs/_build/html/
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.444361 numtools-1.6.0/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1001) nic       (1001)      286 2019-12-16 16:19:06.000000 numtools-1.6.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.6.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       90 2019-12-16 16:19:06.000000 numtools-1.6.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/authors.rst
+-rwxr-xr-x   0 nic       (1001) nic       (1001)     4900 2022-10-12 15:49:49.000000 numtools-1.6.0/docs/conf.py
+-rw-r--r--   0 nic       (1001) nic       (1001)       33 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/contributing.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       28 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/history.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      305 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/index.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      102 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/installation.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      770 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/make.bat
+-rw-r--r--   0 nic       (1001) nic       (1001)       61 2020-01-15 10:31:32.000000 numtools-1.6.0/docs/modules.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      136 2020-01-15 10:31:32.000000 numtools-1.6.0/docs/numtools.csyslib.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      133 2020-01-15 10:31:32.000000 numtools-1.6.0/docs/numtools.intzip.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      270 2020-01-15 10:31:32.000000 numtools-1.6.0/docs/numtools.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.6.0/docs/numtools.serializer.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)      145 2020-01-15 10:31:32.000000 numtools-1.6.0/docs/numtools.vgextended.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       27 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/readme.rst
+-rw-r--r--   0 nic       (1001) nic       (1001)       71 2019-11-19 09:06:07.000000 numtools-1.6.0/docs/usage.rst
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.444361 numtools-1.6.0/numtools/
+-rw-rw-r--   0 nic       (1001) nic       (1001)      167 2023-07-29 09:35:02.000000 numtools-1.6.0/numtools/__init__.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)    18162 2023-05-12 11:23:41.000000 numtools-1.6.0/numtools/csyslib.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     6348 2023-07-29 09:33:26.000000 numtools-1.6.0/numtools/intzip.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     4406 2023-05-02 04:11:56.000000 numtools-1.6.0/numtools/pandas_tk.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     9152 2022-10-12 15:49:49.000000 numtools-1.6.0/numtools/serializer.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     5315 2023-03-13 09:11:17.000000 numtools-1.6.0/numtools/vgextended.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.444361 numtools-1.6.0/numtools.egg-info/
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1521 2023-07-29 09:35:18.000000 numtools-1.6.0/numtools.egg-info/PKG-INFO
+-rw-rw-r--   0 nic       (1001) nic       (1001)      950 2023-07-29 09:35:18.000000 numtools-1.6.0/numtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-07-29 09:35:18.000000 numtools-1.6.0/numtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nic       (1001) nic       (1001)        1 2023-07-29 09:35:18.000000 numtools-1.6.0/numtools.egg-info/not-zip-safe
+-rw-rw-r--   0 nic       (1001) nic       (1001)        9 2023-07-29 09:35:18.000000 numtools-1.6.0/numtools.egg-info/top_level.txt
+-rw-r--r--   0 nic       (1001) nic       (1001)      483 2023-07-29 09:35:18.448361 numtools-1.6.0/setup.cfg
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1229 2023-07-29 09:35:02.000000 numtools-1.6.0/setup.py
+drwxrwxr-x   0 nic       (1001) nic       (1001)        0 2023-07-29 09:35:18.448361 numtools-1.6.0/tests/
+-rw-r--r--   0 nic       (1001) nic       (1001)       63 2019-11-19 09:06:07.000000 numtools-1.6.0/tests/__init__.py
+-rw-r--r--   0 nic       (1001) nic       (1001)     2559 2022-10-12 15:49:45.000000 numtools-1.6.0/tests/test_csyslib.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)      967 2022-10-12 09:19:37.000000 numtools-1.6.0/tests/test_intzip.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     1469 2023-03-13 09:09:12.000000 numtools-1.6.0/tests/test_matrix.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     2567 2023-01-19 14:44:08.000000 numtools-1.6.0/tests/test_pandas_tk.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3529 2022-10-12 15:49:49.000000 numtools-1.6.0/tests/test_serializer.py
+-rw-rw-r--   0 nic       (1001) nic       (1001)     3599 2022-10-12 15:49:45.000000 numtools-1.6.0/tests/test_serializer.py.orig
```

### Comparing `numtools-1.5.0/LICENSE` & `numtools-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/PKG-INFO` & `numtools-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numtools
-Version: 1.5.0
+Version: 1.6.0
 Summary: numeric-gmbH toolbox
 Home-page: https://framagit.org/numenic/numtools
 Author: numenic
 Author-email: info@numeric-gmbh.ch
 Keywords: numtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `numtools-1.5.0/README.rst` & `numtools-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/docs/Makefile` & `numtools-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/docs/conf.py` & `numtools-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/docs/make.bat` & `numtools-1.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/numtools/csyslib.py` & `numtools-1.6.0/numtools/csyslib.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/numtools/intzip.py` & `numtools-1.6.0/numtools/intzip.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 
 
 def _get_groups(seq):
     for k, g in groupby(enumerate(seq), key=lambda i_x: i_x[0] - i_x[1]):
         yield list(map(itemgetter(1), g))
 
 
-def _cons2str(seq, sep=", ", linkword="to"):
+def _cons2str(seq, sep=", ", linkword="to", strip_linkword=False):
     """transform a sequence of consecutive integers to
     human-friendly string
 
     >>> _cons2str([4])
     '4'
     >>> _cons2str([4, 5])
     '4, 5'
     >>> _cons2str([4, 5, 6 ,7, 8])
     '4 to 8'
+    >>> _cons2str([4, 5, 6 ,7, 8], linkword=":", strip_linkword=True)
+    '4:8'
     """
     tokens = [str(i) for i in seq]
     if len(seq) <= 2:
         ret = sep.join(tokens)
-    else:
+    elif not strip_linkword:
         ret = "%d %s %d" % (seq[0], linkword, seq[-1])
+    else:
+        ret = "%d%s%d" % (seq[0], linkword, seq[-1])
     return ret
 
 
 def _cons2tuple(seq, couple_alone=None, astype=tuple):
     """
     >>> _cons2tuple((4,))
     4
@@ -48,15 +52,17 @@
                 ret = astype((seq[0], couple_alone))
             else:
                 ret = astype((seq[0], seq[0]))
         return ret
     return astype((min(seq), max(seq)))
 
 
-def hzip(seq, sort=True, sep=", ", last_sep=" and ", linkword="to"):
+def hzip(
+    seq, sort=True, sep=", ", last_sep=" and ", linkword="to", strip_linkword=False
+):
     """
     Create a human friendly (hence the ``hzip`` name) string from a
     sorted iterable of integers.
 
     :param seq: iterable to parse
     :type seq: any iterable made of **integers**
     :param sort: if ``True``, sort ``seq`` as a preliminary.
@@ -74,24 +80,29 @@
     >>> hzip(seq, sort=False)
     '1, 2, 6, 5, 11, 7 to 9, 3, 12 and 0'
     >>> hzip(seq, sep='; ', sort=True, linkword='thru', last_sep=' and finally ' )
     '0 thru 3; 5 thru 9; 11 and finally 12'
     >>> # zipping an empty sequence is olso OK
     >>> hzip([])
     ''
+    >>> seq =   (0, 1, 2, 5, 6, 7, 8, 9, 11, 15, 16)
+    >>> hzip(seq, linkword=":", strip_linkword=True, sep=" ", last_sep=" ")
+    '0:2 5:9 11 15 16'
     """
     if sort:
         seq = sorted(list(seq))
-    tokens = [_cons2str(grp, sep=sep, linkword=linkword) for grp in _get_groups(seq)]
+    tokens = [
+        _cons2str(grp, sep=sep, linkword=linkword, strip_linkword=strip_linkword)
+        for grp in _get_groups(seq)
+    ]
     s = sep.join(tokens)
     # replace last occurence of `sep` by `last_sep`
     ix = s.rfind(sep)
     if ix > 0:
         s = s[:ix] + last_sep + s[(ix + len(sep)) :]
-
     return s
 
 
 def hunzip(hseq, sep=",", last_sep="and", linkword=None, sort=True):
     """
     Revert back a hzip to python list.
```

### Comparing `numtools-1.5.0/numtools/pandas_tk.py` & `numtools-1.6.0/numtools/pandas_tk.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/numtools/serializer.py` & `numtools-1.6.0/numtools/serializer.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/numtools/vgextended.py` & `numtools-1.6.0/numtools/vgextended.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/numtools.egg-info/PKG-INFO` & `numtools-1.6.0/numtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numtools
-Version: 1.5.0
+Version: 1.6.0
 Summary: numeric-gmbH toolbox
 Home-page: https://framagit.org/numenic/numtools
 Author: numenic
 Author-email: info@numeric-gmbh.ch
 Keywords: numtools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `numtools-1.5.0/numtools.egg-info/SOURCES.txt` & `numtools-1.6.0/numtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/setup.py` & `numtools-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,11 +39,11 @@
     include_package_data=True,
     keywords="numtools",
     name="numtools",
     packages=find_packages(include=["numtools", "numtools.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
-    version="1.5.0",
+    version="1.6.0",
     zip_safe=False,
     url="https://framagit.org/numenic/numtools",
 )
```

### Comparing `numtools-1.5.0/tests/test_csyslib.py` & `numtools-1.6.0/tests/test_csyslib.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/tests/test_intzip.py` & `numtools-1.6.0/tests/test_intzip.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/tests/test_matrix.py` & `numtools-1.6.0/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/tests/test_pandas_tk.py` & `numtools-1.6.0/tests/test_pandas_tk.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/tests/test_serializer.py` & `numtools-1.6.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `numtools-1.5.0/tests/test_serializer.py.orig` & `numtools-1.6.0/tests/test_serializer.py.orig`

 * *Files identical despite different names*

