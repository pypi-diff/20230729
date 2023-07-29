# Comparing `tmp/CFXplorer-0.0.dev7.tar.gz` & `tmp/CFXplorer-0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CFXplorer-0.0.dev7.tar", last modified: Thu Jul 27 22:10:35 2023, max compression
+gzip compressed data, was "CFXplorer-0.0b1.tar", last modified: Sat Jul 29 14:15:55 2023, max compression
```

## Comparing `CFXplorer-0.0.dev7.tar` & `CFXplorer-0.0b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:10:35.564056 CFXplorer-0.0.dev7/
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:10:35.558921 CFXplorer-0.0.dev7/CFXplorer.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 22:10:35.000000 CFXplorer-0.0.dev7/CFXplorer.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      338 2023-07-27 22:10:35.000000 CFXplorer-0.0.dev7/CFXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-27 22:10:35.000000 CFXplorer-0.0.dev7/CFXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-27 22:10:35.000000 CFXplorer-0.0.dev7/CFXplorer.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev7/LICENSE
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 22:10:35.564227 CFXplorer-0.0.dev7/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-27 21:45:55.000000 CFXplorer-0.0.dev7/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:10:35.562150 CFXplorer-0.0.dev7/cfxplorer/
--rw-r--r--   0 kyosuke    (501) staff       (20)      607 2023-07-27 22:09:50.000000 CFXplorer-0.0.dev7/cfxplorer/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)    18439 2023-07-27 22:09:50.000000 CFXplorer-0.0.dev7/cfxplorer/focus.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 22:10:35.563449 CFXplorer-0.0.dev7/cfxplorer/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev7/cfxplorer/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev7/cfxplorer/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-27 22:10:18.000000 CFXplorer-0.0.dev7/cfxplorer/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4633 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev7/cfxplorer/utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      580 2023-07-27 22:09:50.000000 CFXplorer-0.0.dev7/cfxplorer/version.py
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-27 22:10:35.564695 CFXplorer-0.0.dev7/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1381 2023-07-27 22:09:50.000000 CFXplorer-0.0.dev7/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.169748 CFXplorer-0.0b1/
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.164272 CFXplorer-0.0b1/CFXplorer.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5158 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      338 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-29 14:15:55.000000 CFXplorer-0.0b1/CFXplorer.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/LICENSE
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5158 2023-07-29 14:15:55.169941 CFXplorer-0.0b1/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4388 2023-07-28 20:06:02.000000 CFXplorer-0.0b1/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.167355 CFXplorer-0.0b1/cfxplorer/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      607 2023-07-27 22:09:50.000000 CFXplorer-0.0b1/cfxplorer/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)    18439 2023-07-27 22:09:50.000000 CFXplorer-0.0b1/cfxplorer/focus.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-29 14:15:55.169037 CFXplorer-0.0b1/cfxplorer/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/cfxplorer/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/cfxplorer/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-27 22:10:18.000000 CFXplorer-0.0b1/cfxplorer/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4633 2023-07-26 21:33:17.000000 CFXplorer-0.0b1/cfxplorer/utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      577 2023-07-29 13:39:03.000000 CFXplorer-0.0b1/cfxplorer/version.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-29 14:15:55.170627 CFXplorer-0.0b1/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1381 2023-07-27 22:09:50.000000 CFXplorer-0.0b1/setup.py
```

### Comparing `CFXplorer-0.0.dev7/CFXplorer.egg-info/PKG-INFO` & `CFXplorer-0.0b1/CFXplorer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFXplorer
-Version: 0.0.dev7
+Version: 0.0b1
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -17,35 +17,36 @@
 License-File: LICENSE
 
 CFXplorer
 =========
 
 **Deployment & Documentation & Stats & License**
 
-.. image:: https://img.shields.io/pypi/v/focus-cfe.svg?color=brightgreen
-   :target: https://pypi.org/project/focus-cfe/
+.. image:: https://img.shields.io/pypi/v/CFXplorer.svg?color=brightgreen
+   :target: https://pypi.org/project/CFXplorer/
    :alt: PyPI version
 
-.. image:: https://readthedocs.org/projects/focus-cfe/badge/?version=latest
-   :target: https://focus-cfe.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/CFXplorer/badge/?version=latest
+   :target: https://CFXplorer.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
-.. image:: https://pepy.tech/badge/focus-cfe
-   :target: https://pepy.tech/project/focus-cfe
+.. image:: https://pepy.tech/badge/CFXplorer
+   :target: https://pepy.tech/project/CFXplorer
    :alt: Downloads
 
 .. image:: https://codecov.io/gh/kyosek/CFXplorer/branch/master/graph/badge.svg?token=G5I7TJR0JQ
     :target: https://codecov.io/gh/kyosek/CFXplorer
+    :alt: Code Coverage
 
 .. image:: https://dl.circleci.com/status-badge/img/gh/kyosek/CFXplorer/tree/master.svg?style=svg
     :target: https://dl.circleci.com/status-badge/redirect/gh/kyosek/CFXplorer/tree/master
     :alt: Circle CI
 
 .. image:: https://api.codeclimate.com/v1/badges/93840d29606abb212051/maintainability
-   :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
+   :target: https://codeclimate.com/github/kyosek/CFXplorer/maintainability
    :alt: Maintainability
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/kyosek/CFXplorer
    :alt: pre-commit
 
 .. image:: https://img.shields.io/github/license/kyosek/CFXplorer.svg
@@ -90,34 +91,33 @@
     from cfxplorer import Focus
     # Initialize Focus instance with default values
     focus = Focus()
 
     # Generate counterfactual explanations for given tree model and features
     pertubed = focus.generate(tree_model, X)
 
-
 Examples
 --------
 
-- Comprehensive examples can be found in the `examples folder <https://github.com/kyosek/CFXplorer/blob/master/examples/focus_example.py>`_.
-- Kaggle notebook example can be found `here <https://www.kaggle.com/code/kyosukemorita/focus-example>`__.
+- Comprehensive examples can be found in the `examples folder <https://github.com/kyosek/CFXplorer/blob/master/examples>`_.
+- Kaggle notebook example can be found `here <https://www.kaggle.com/code/kyosukemorita/cfxplorer-example>`__.
 - Below is demonstrated a comparison of before and after Focus is applied to feature set from the example given above.
 
 .. image:: https://raw.githubusercontent.com/kyosek/focus/master/docs/plot.png
     :width: 800px
     :height: 400px
     :scale: 100 %
     :alt: Before and After FOCUS was applied to the features from above example.
 
 Limitations of Focus class
 --------------------------
 
 - Currently, Focus class can only be applied to scikit-learn ``DecisionTreeClassifier``, ``RandomForestClassifier`` and ``AdaBoostClassifier``.
 - While categorical features may be included in the feature set, it is important to note that the interpretation of changes in categorical features, such as transitioning from age 40 to 20, may not provide meaningful insights.
-- The input features should be scaled to the range of 0 and 1 before applying Focus-cfe. Therefore, it is necessary to transform the features prior to using Focus. However, this scaling process may introduce some additional complexity when interpreting the features after applying Focus.
+- The input features should be scaled to the range of 0 and 1 before applying Focus. Therefore, it is necessary to transform the features prior to using Focus. However, this scaling process may introduce some additional complexity when interpreting the features after applying Focus.
 
 Documentation
 -------------
 
 The documentation can be found `here <https://cfxplorer.readthedocs.io/en/latest/>`__.
 
 Contributing
```

### Comparing `CFXplorer-0.0.dev7/LICENSE` & `CFXplorer-0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev7/PKG-INFO` & `CFXplorer-0.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFXplorer
-Version: 0.0.dev7
+Version: 0.0b1
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -17,35 +17,36 @@
 License-File: LICENSE
 
 CFXplorer
 =========
 
 **Deployment & Documentation & Stats & License**
 
-.. image:: https://img.shields.io/pypi/v/focus-cfe.svg?color=brightgreen
-   :target: https://pypi.org/project/focus-cfe/
+.. image:: https://img.shields.io/pypi/v/CFXplorer.svg?color=brightgreen
+   :target: https://pypi.org/project/CFXplorer/
    :alt: PyPI version
 
-.. image:: https://readthedocs.org/projects/focus-cfe/badge/?version=latest
-   :target: https://focus-cfe.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/CFXplorer/badge/?version=latest
+   :target: https://CFXplorer.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
-.. image:: https://pepy.tech/badge/focus-cfe
-   :target: https://pepy.tech/project/focus-cfe
+.. image:: https://pepy.tech/badge/CFXplorer
+   :target: https://pepy.tech/project/CFXplorer
    :alt: Downloads
 
 .. image:: https://codecov.io/gh/kyosek/CFXplorer/branch/master/graph/badge.svg?token=G5I7TJR0JQ
     :target: https://codecov.io/gh/kyosek/CFXplorer
+    :alt: Code Coverage
 
 .. image:: https://dl.circleci.com/status-badge/img/gh/kyosek/CFXplorer/tree/master.svg?style=svg
     :target: https://dl.circleci.com/status-badge/redirect/gh/kyosek/CFXplorer/tree/master
     :alt: Circle CI
 
 .. image:: https://api.codeclimate.com/v1/badges/93840d29606abb212051/maintainability
-   :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
+   :target: https://codeclimate.com/github/kyosek/CFXplorer/maintainability
    :alt: Maintainability
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/kyosek/CFXplorer
    :alt: pre-commit
 
 .. image:: https://img.shields.io/github/license/kyosek/CFXplorer.svg
@@ -90,34 +91,33 @@
     from cfxplorer import Focus
     # Initialize Focus instance with default values
     focus = Focus()
 
     # Generate counterfactual explanations for given tree model and features
     pertubed = focus.generate(tree_model, X)
 
-
 Examples
 --------
 
-- Comprehensive examples can be found in the `examples folder <https://github.com/kyosek/CFXplorer/blob/master/examples/focus_example.py>`_.
-- Kaggle notebook example can be found `here <https://www.kaggle.com/code/kyosukemorita/focus-example>`__.
+- Comprehensive examples can be found in the `examples folder <https://github.com/kyosek/CFXplorer/blob/master/examples>`_.
+- Kaggle notebook example can be found `here <https://www.kaggle.com/code/kyosukemorita/cfxplorer-example>`__.
 - Below is demonstrated a comparison of before and after Focus is applied to feature set from the example given above.
 
 .. image:: https://raw.githubusercontent.com/kyosek/focus/master/docs/plot.png
     :width: 800px
     :height: 400px
     :scale: 100 %
     :alt: Before and After FOCUS was applied to the features from above example.
 
 Limitations of Focus class
 --------------------------
 
 - Currently, Focus class can only be applied to scikit-learn ``DecisionTreeClassifier``, ``RandomForestClassifier`` and ``AdaBoostClassifier``.
 - While categorical features may be included in the feature set, it is important to note that the interpretation of changes in categorical features, such as transitioning from age 40 to 20, may not provide meaningful insights.
-- The input features should be scaled to the range of 0 and 1 before applying Focus-cfe. Therefore, it is necessary to transform the features prior to using Focus. However, this scaling process may introduce some additional complexity when interpreting the features after applying Focus.
+- The input features should be scaled to the range of 0 and 1 before applying Focus. Therefore, it is necessary to transform the features prior to using Focus. However, this scaling process may introduce some additional complexity when interpreting the features after applying Focus.
 
 Documentation
 -------------
 
 The documentation can be found `here <https://cfxplorer.readthedocs.io/en/latest/>`__.
 
 Contributing
```

### Comparing `CFXplorer-0.0.dev7/README.rst` & `CFXplorer-0.0b1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 CFXplorer
 =========
 
 **Deployment & Documentation & Stats & License**
 
-.. image:: https://img.shields.io/pypi/v/focus-cfe.svg?color=brightgreen
-   :target: https://pypi.org/project/focus-cfe/
+.. image:: https://img.shields.io/pypi/v/CFXplorer.svg?color=brightgreen
+   :target: https://pypi.org/project/CFXplorer/
    :alt: PyPI version
 
-.. image:: https://readthedocs.org/projects/focus-cfe/badge/?version=latest
-   :target: https://focus-cfe.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/CFXplorer/badge/?version=latest
+   :target: https://CFXplorer.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
-.. image:: https://pepy.tech/badge/focus-cfe
-   :target: https://pepy.tech/project/focus-cfe
+.. image:: https://pepy.tech/badge/CFXplorer
+   :target: https://pepy.tech/project/CFXplorer
    :alt: Downloads
 
 .. image:: https://codecov.io/gh/kyosek/CFXplorer/branch/master/graph/badge.svg?token=G5I7TJR0JQ
     :target: https://codecov.io/gh/kyosek/CFXplorer
+    :alt: Code Coverage
 
 .. image:: https://dl.circleci.com/status-badge/img/gh/kyosek/CFXplorer/tree/master.svg?style=svg
     :target: https://dl.circleci.com/status-badge/redirect/gh/kyosek/CFXplorer/tree/master
     :alt: Circle CI
 
 .. image:: https://api.codeclimate.com/v1/badges/93840d29606abb212051/maintainability
-   :target: https://codeclimate.com/github/kyosek/focus-cfe/maintainability
+   :target: https://codeclimate.com/github/kyosek/CFXplorer/maintainability
    :alt: Maintainability
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/kyosek/CFXplorer
    :alt: pre-commit
 
 .. image:: https://img.shields.io/github/license/kyosek/CFXplorer.svg
@@ -72,34 +73,33 @@
     from cfxplorer import Focus
     # Initialize Focus instance with default values
     focus = Focus()
 
     # Generate counterfactual explanations for given tree model and features
     pertubed = focus.generate(tree_model, X)
 
-
 Examples
 --------
 
-- Comprehensive examples can be found in the `examples folder <https://github.com/kyosek/CFXplorer/blob/master/examples/focus_example.py>`_.
-- Kaggle notebook example can be found `here <https://www.kaggle.com/code/kyosukemorita/focus-example>`__.
+- Comprehensive examples can be found in the `examples folder <https://github.com/kyosek/CFXplorer/blob/master/examples>`_.
+- Kaggle notebook example can be found `here <https://www.kaggle.com/code/kyosukemorita/cfxplorer-example>`__.
 - Below is demonstrated a comparison of before and after Focus is applied to feature set from the example given above.
 
 .. image:: https://raw.githubusercontent.com/kyosek/focus/master/docs/plot.png
     :width: 800px
     :height: 400px
     :scale: 100 %
     :alt: Before and After FOCUS was applied to the features from above example.
 
 Limitations of Focus class
 --------------------------
 
 - Currently, Focus class can only be applied to scikit-learn ``DecisionTreeClassifier``, ``RandomForestClassifier`` and ``AdaBoostClassifier``.
 - While categorical features may be included in the feature set, it is important to note that the interpretation of changes in categorical features, such as transitioning from age 40 to 20, may not provide meaningful insights.
-- The input features should be scaled to the range of 0 and 1 before applying Focus-cfe. Therefore, it is necessary to transform the features prior to using Focus. However, this scaling process may introduce some additional complexity when interpreting the features after applying Focus.
+- The input features should be scaled to the range of 0 and 1 before applying Focus. Therefore, it is necessary to transform the features prior to using Focus. However, this scaling process may introduce some additional complexity when interpreting the features after applying Focus.
 
 Documentation
 -------------
 
 The documentation can be found `here <https://cfxplorer.readthedocs.io/en/latest/>`__.
 
 Contributing
```

### Comparing `CFXplorer-0.0.dev7/cfxplorer/__init__.py` & `CFXplorer-0.0b1/cfxplorer/__init__.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev7/cfxplorer/focus.py` & `CFXplorer-0.0b1/cfxplorer/focus.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev7/cfxplorer/tests/test_focus.py` & `CFXplorer-0.0b1/cfxplorer/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev7/cfxplorer/tests/test_utils.py` & `CFXplorer-0.0b1/cfxplorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev7/cfxplorer/utils.py` & `CFXplorer-0.0b1/cfxplorer/utils.py`

 * *Files identical despite different names*

### Comparing `CFXplorer-0.0.dev7/cfxplorer/version.py` & `CFXplorer-0.0b1/cfxplorer/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev7"  # pragma: no cover
+__version__ = "0.0b1"  # pragma: no cover
```

### Comparing `CFXplorer-0.0.dev7/setup.py` & `CFXplorer-0.0b1/setup.py`

 * *Files identical despite different names*

