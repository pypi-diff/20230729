# Comparing `tmp/CFXplorer-0.0b1.tar.gz` & `tmp/CFXplorer-0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CFXplorer-0.0b1.tar", last modified: Sat Jul 29 14:15:55 2023, max compression
+gzip compressed data, was "CFXplorer-0.0b2.tar", last modified: Sat Jul 29 16:02:47 2023, max compression
```

## Comparing `CFXplorer-0.0b1.tar` & `CFXplorer-0.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.169748 CFXplorer-0.0b1/
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.164272 CFXplorer-0.0b1/CFXplorer.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     5158 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      338 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/LICENSE
--rw-r--r--   0 kyosuke    (501) staff       (20)     5158 2023-07-29 14:15:55.169941 CFXplorer-0.0b1/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     4388 2023-07-28 20:06:02.000000 CFXplorer-0.0b1/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.167355 CFXplorer-0.0b1/cfxplorer/
--rw-r--r--   0 kyosuke    (501) staff       (20)      607 2023-07-27 22:09:50.000000 CFXplorer-0.0b1/cfxplorer/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)    18439 2023-07-27 22:09:50.000000 CFXplorer-0.0b1/cfxplorer/focus.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.169037 CFXplorer-0.0b1/cfxplorer/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/cfxplorer/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/cfxplorer/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-27 22:10:18.000000 CFXplorer-0.0b1/cfxplorer/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4633 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/cfxplorer/utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      577 2023-07-29 13:39:03.000000 CFXplorer-0.0b1/cfxplorer/version.py
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-29 14:15:55.170627 CFXplorer-0.0b1/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1381 2023-07-27 22:09:50.000000 CFXplorer-0.0b1/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 16:02:47.986942 CFXplorer-0.0b2/
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 16:02:47.980782 CFXplorer-0.0b2/CFXplorer.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5158 2023-07-29 16:02:47.000000 CFXplorer-0.0b2/CFXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      338 2023-07-29 16:02:47.000000 CFXplorer-0.0b2/CFXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-29 16:02:47.000000 CFXplorer-0.0b2/CFXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-29 16:02:47.000000 CFXplorer-0.0b2/CFXplorer.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-07-26 21:33:17.000000 CFXplorer-0.0b2/LICENSE
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5158 2023-07-29 16:02:47.987142 CFXplorer-0.0b2/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4388 2023-07-28 20:06:02.000000 CFXplorer-0.0b2/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 16:02:47.984493 CFXplorer-0.0b2/cfxplorer/
+-rw-r--r--   0 kyosuke    (501) staff       (20)       46 2023-07-29 15:55:11.000000 CFXplorer-0.0b2/cfxplorer/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)    18439 2023-07-27 22:09:50.000000 CFXplorer-0.0b2/cfxplorer/focus.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 16:02:47.986206 CFXplorer-0.0b2/cfxplorer/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:33:17.000000 CFXplorer-0.0b2/cfxplorer/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:33:17.000000 CFXplorer-0.0b2/cfxplorer/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-27 22:10:18.000000 CFXplorer-0.0b2/cfxplorer/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4633 2023-07-26 21:33:17.000000 CFXplorer-0.0b2/cfxplorer/utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      577 2023-07-29 15:57:33.000000 CFXplorer-0.0b2/cfxplorer/version.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-29 16:02:47.987933 CFXplorer-0.0b2/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1381 2023-07-27 22:09:50.000000 CFXplorer-0.0b2/setup.py
```

### Comparing `CFXplorer-0.0b1/CFXplorer.egg-info/PKG-INFO` & `CFXplorer-0.0b2/CFXplorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFXplorer
-Version: 0.0b1
+Version: 0.0b2
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CFXplorer-0.0b1/LICENSE` & `CFXplorer-0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0b1/PKG-INFO` & `CFXplorer-0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFXplorer
-Version: 0.0b1
+Version: 0.0b2
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CFXplorer-0.0b1/README.rst` & `CFXplorer-0.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0b1/cfxplorer/focus.py` & `CFXplorer-0.0b2/cfxplorer/focus.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0b1/cfxplorer/tests/test_focus.py` & `CFXplorer-0.0b2/cfxplorer/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0b1/cfxplorer/tests/test_utils.py` & `CFXplorer-0.0b2/cfxplorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0b1/cfxplorer/utils.py` & `CFXplorer-0.0b2/cfxplorer/utils.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0b1/cfxplorer/version.py` & `CFXplorer-0.0b2/cfxplorer/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0b1"  # pragma: no cover
+__version__ = "0.0b2"  # pragma: no cover
```

### Comparing `CFXplorer-0.0b1/setup.py` & `CFXplorer-0.0b2/setup.py`

 * *Files identical despite different names*

