# Comparing `tmp/pyflakes-3.0.1.tar.gz` & `tmp/pyflakes-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflakes-3.0.1.tar", last modified: Thu Nov 24 16:53:21 2022, max compression
+gzip compressed data, was "pyflakes-3.1.0.tar", last modified: Sat Jul 29 17:00:24 2023, max compression
```

## Comparing `pyflakes-3.0.1.tar` & `pyflakes-3.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:53:21.689930 pyflakes-3.0.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)      485 2022-11-24 16:02:51.000000 pyflakes-3.0.1/AUTHORS
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1093 2022-11-24 16:02:51.000000 pyflakes-3.0.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-11-24 16:02:51.000000 pyflakes-3.0.1/MANIFEST.in
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12104 2022-11-24 16:52:19.000000 pyflakes-3.0.1/NEWS.rst
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3775 2022-11-24 16:53:21.689930 pyflakes-3.0.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2726 2022-11-24 16:02:51.000000 pyflakes-3.0.1/README.rst
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:53:21.685932 pyflakes-3.0.1/bin/
--rwxr-xr-x   0 asottile  (1000) asottile  (1000)       72 2022-11-24 16:02:51.000000 pyflakes-3.0.1/bin/pyflakes
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:53:21.689930 pyflakes-3.0.1/pyflakes/
--rw-r--r--   0 asottile  (1000) asottile  (1000)       22 2022-11-24 16:52:30.000000 pyflakes-3.0.1/pyflakes/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      105 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5550 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/api.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    76607 2022-11-24 16:51:58.000000 pyflakes-3.0.1/pyflakes/checker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    10426 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/messages.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3053 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/reporter.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:53:21.689930 pyflakes-3.0.1/pyflakes/scripts/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/scripts/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      248 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/scripts/pyflakes.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:53:21.689930 pyflakes-3.0.1/pyflakes/test/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      891 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/harness.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    26904 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_api.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      582 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_builtin.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4496 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_code_segment.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_dict.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12856 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_doctests.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    33703 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4573 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_is_literal.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2097 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_match.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    51817 2022-11-24 16:51:58.000000 pyflakes-3.0.1/pyflakes/test/test_other.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    17439 2022-11-24 16:02:51.000000 pyflakes-3.0.1/pyflakes/test/test_type_annotations.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    23488 2022-11-24 16:18:39.000000 pyflakes-3.0.1/pyflakes/test/test_undefined_names.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-11-24 16:53:21.689930 pyflakes-3.0.1/pyflakes.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3775 2022-11-24 16:53:21.000000 pyflakes-3.0.1/pyflakes.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      816 2022-11-24 16:53:21.000000 pyflakes-3.0.1/pyflakes.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-11-24 16:53:21.000000 pyflakes-3.0.1/pyflakes.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       47 2022-11-24 16:53:21.000000 pyflakes-3.0.1/pyflakes.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2022-11-24 16:53:21.000000 pyflakes-3.0.1/pyflakes.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      102 2022-11-24 16:53:21.689930 pyflakes-3.0.1/setup.cfg
--rwxr-xr-x   0 asottile  (1000) asottile  (1000)     2024 2022-11-24 16:02:51.000000 pyflakes-3.0.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 17:00:24.935112 pyflakes-3.1.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      485 2022-11-23 18:37:38.000000 pyflakes-3.1.0/AUTHORS
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1093 2022-11-23 18:37:38.000000 pyflakes-3.1.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-11-23 18:37:38.000000 pyflakes-3.1.0/MANIFEST.in
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12577 2023-07-29 16:57:43.000000 pyflakes-3.1.0/NEWS.rst
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3486 2023-07-29 17:00:24.935112 pyflakes-3.1.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2688 2023-01-31 18:28:24.000000 pyflakes-3.1.0/README.rst
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 17:00:24.919112 pyflakes-3.1.0/bin/
+-rwxr-xr-x   0 asottile  (1000) asottile  (1000)       72 2022-11-23 18:37:38.000000 pyflakes-3.1.0/bin/pyflakes
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 17:00:24.923112 pyflakes-3.1.0/pyflakes/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       22 2023-07-29 16:58:22.000000 pyflakes-3.1.0/pyflakes/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      105 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5550 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/api.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    75643 2023-07-29 16:51:35.000000 pyflakes-3.1.0/pyflakes/checker.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    10227 2023-01-31 18:28:24.000000 pyflakes-3.1.0/pyflakes/messages.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3001 2023-06-13 01:11:44.000000 pyflakes-3.1.0/pyflakes/reporter.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 17:00:24.923112 pyflakes-3.1.0/pyflakes/scripts/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/scripts/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      248 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/scripts/pyflakes.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 17:00:24.935112 pyflakes-3.1.0/pyflakes/test/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      891 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/harness.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    26526 2023-06-13 01:50:05.000000 pyflakes-3.1.0/pyflakes/test/test_api.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      582 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/test_builtin.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4496 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/test_code_segment.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5271 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/test_dict.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12600 2023-01-31 18:28:24.000000 pyflakes-3.1.0/pyflakes/test/test_doctests.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    33703 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/test_imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4573 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/test_is_literal.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2393 2023-06-13 00:24:07.000000 pyflakes-3.1.0/pyflakes/test/test_match.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    50635 2023-01-31 18:28:24.000000 pyflakes-3.1.0/pyflakes/test/test_other.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    19664 2023-07-29 16:51:35.000000 pyflakes-3.1.0/pyflakes/test/test_type_annotations.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    23488 2022-11-23 18:37:38.000000 pyflakes-3.1.0/pyflakes/test/test_undefined_names.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 17:00:24.923112 pyflakes-3.1.0/pyflakes.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3486 2023-07-29 17:00:24.000000 pyflakes-3.1.0/pyflakes.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      816 2023-07-29 17:00:24.000000 pyflakes-3.1.0/pyflakes.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-29 17:00:24.000000 pyflakes-3.1.0/pyflakes.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       47 2023-07-29 17:00:24.000000 pyflakes-3.1.0/pyflakes.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        9 2023-07-29 17:00:24.000000 pyflakes-3.1.0/pyflakes.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      102 2023-07-29 17:00:24.935112 pyflakes-3.1.0/setup.cfg
+-rwxr-xr-x   0 asottile  (1000) asottile  (1000)     1778 2023-01-31 18:28:24.000000 pyflakes-3.1.0/setup.py
```

### Comparing `pyflakes-3.0.1/LICENSE` & `pyflakes-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/NEWS.rst` & `pyflakes-3.1.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+3.1.0 (2023-07-29)
+
+- Drop support for EOL python 3.6 / 3.7
+- Remove ``ContinueInFinally`` check (only relevant in python < 3.8)
+- Fix forward annotations inside a nested scope
+- Produce an error when a definition shadows an unused variable
+- Fix accessed global annotation being redefined in a local scope
+- Allow redefinition of functions across ``match`` arms
+- Fix potential ``None`` for ``lineno`` during tokenization errors
+- Add support for PEP 695 and python 3.12
+
 3.0.1 (2022-11-24)
 
 - Fix crash on augmented assign to ``print`` builtin
 
 3.0.0 (2022-11-23)
 
 - Detect undefined name in variable defined by an annotated assignment
```

### Comparing `pyflakes-3.0.1/PKG-INFO` & `pyflakes-3.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: pyflakes
-Version: 3.0.1
+Version: 3.1.0
 Summary: passive checker of Python programs
 Home-page: https://github.com/PyCQA/pyflakes
 Author: A lot of people
 Author-email: code-quality@python.org
 License: MIT
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ========
 Pyflakes
 ========
 
 A simple program which checks Python source files for errors.
@@ -85,16 +80,16 @@
 <https://mail.python.org/mailman/listinfo/code-quality>`_
 
 Contributing
 ------------
 
 Issues are tracked on `GitHub <https://github.com/PyCQA/pyflakes/issues>`_.
 
-Patches may be submitted via a `GitHub pull request`_ or via the mailing list
-if you prefer. If you are comfortable doing so, please `rebase your changes`_
+Patches may be submitted via a `GitHub pull request`_.
+If you are comfortable doing so, please `rebase your changes`_
 so they may be applied to main with a fast-forward merge, and each commit is
 a coherent unit of work with a well-written log message.  If you are not
 comfortable with this rebase workflow, the project maintainers will be happy to
 rebase your commits for you.
 
 All changes should include tests and pass flake8_.
```

### Comparing `pyflakes-3.0.1/README.rst` & `pyflakes-3.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 <https://mail.python.org/mailman/listinfo/code-quality>`_
 
 Contributing
 ------------
 
 Issues are tracked on `GitHub <https://github.com/PyCQA/pyflakes/issues>`_.
 
-Patches may be submitted via a `GitHub pull request`_ or via the mailing list
-if you prefer. If you are comfortable doing so, please `rebase your changes`_
+Patches may be submitted via a `GitHub pull request`_.
+If you are comfortable doing so, please `rebase your changes`_
 so they may be applied to main with a fast-forward merge, and each commit is
 a coherent unit of work with a well-written log message.  If you are not
 comfortable with this rebase workflow, the project maintainers will be happy to
 rebase your commits for you.
 
 All changes should include tests and pass flake8_.
```

### Comparing `pyflakes-3.0.1/pyflakes/api.py` & `pyflakes-3.1.0/pyflakes/api.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes/checker.py` & `pyflakes-3.1.0/pyflakes/checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,70 +3,61 @@
 
 Implement the central Checker class.
 Also, it models the Bindings and Scopes.
 """
 import __future__
 import builtins
 import ast
+import collections
 import contextlib
 import doctest
 import functools
 import os
 import re
 import string
 import sys
 import warnings
 
 from pyflakes import messages
 
-PY38_PLUS = sys.version_info >= (3, 8)
 PYPY = hasattr(sys, 'pypy_version_info')
 
 builtin_vars = dir(builtins)
 
 parse_format_string = string.Formatter().parse
 
 
 def getAlternatives(n):
     if isinstance(n, ast.If):
         return [n.body]
-    if isinstance(n, ast.Try):
+    elif isinstance(n, ast.Try):
         return [n.body + n.orelse] + [[hdl] for hdl in n.handlers]
+    elif sys.version_info >= (3, 10) and isinstance(n, ast.Match):
+        return [mc.body for mc in n.cases]
 
 
 FOR_TYPES = (ast.For, ast.AsyncFor)
 
-if PY38_PLUS:
-    def _is_singleton(node):  # type: (ast.AST) -> bool
-        return (
-            isinstance(node, ast.Constant) and
-            isinstance(node.value, (bool, type(Ellipsis), type(None)))
-        )
-else:
-    def _is_singleton(node):  # type: (ast.AST) -> bool
-        return isinstance(node, (ast.NameConstant, ast.Ellipsis))
+
+def _is_singleton(node):  # type: (ast.AST) -> bool
+    return (
+        isinstance(node, ast.Constant) and
+        isinstance(node.value, (bool, type(Ellipsis), type(None)))
+    )
 
 
 def _is_tuple_constant(node):  # type: (ast.AST) -> bool
     return (
         isinstance(node, ast.Tuple) and
         all(_is_constant(elt) for elt in node.elts)
     )
 
 
-if PY38_PLUS:
-    def _is_constant(node):
-        return isinstance(node, ast.Constant) or _is_tuple_constant(node)
-else:
-    def _is_constant(node):
-        return (
-            isinstance(node, (ast.Str, ast.Num, ast.Bytes)) or
-            _is_singleton(node) or
-            _is_tuple_constant(node)
-        )
+def _is_constant(node):
+    return isinstance(node, ast.Constant) or _is_tuple_constant(node)
 
 
 def _is_const_non_singleton(node):  # type: (ast.AST) -> bool
     return _is_constant(node) and not _is_singleton(node)
 
 
 def _is_name_or_attr(node, name):  # type: (ast.AST, str) -> bool
@@ -205,35 +196,20 @@
         elif isinstance(field, list):
             for item in field:
                 if isinstance(item, ast.AST):
                     yield item
 
 
 def convert_to_value(item):
-    if isinstance(item, ast.Str):
-        return item.s
-    elif hasattr(ast, 'Bytes') and isinstance(item, ast.Bytes):
-        return item.s
+    if isinstance(item, ast.Constant):
+        return item.value
     elif isinstance(item, ast.Tuple):
         return tuple(convert_to_value(i) for i in item.elts)
-    elif isinstance(item, ast.Num):
-        return item.n
     elif isinstance(item, ast.Name):
-        result = VariableKey(item=item)
-        constants_lookup = {
-            'True': True,
-            'False': False,
-            'None': None,
-        }
-        return constants_lookup.get(
-            result.name,
-            result,
-        )
-    elif isinstance(item, ast.NameConstant):
-        return item.value
+        return VariableKey(item=item)
     else:
         return UnhandledKeyType()
 
 
 def is_notimplemented_name_node(node):
     return isinstance(node, ast.Name) and getNodeName(node) == 'NotImplemented'
 
@@ -270,14 +246,19 @@
         return isinstance(other, Definition) and self.name == other.name
 
 
 class Definition(Binding):
     """
     A binding that defines a function or a class.
     """
+    def redefines(self, other):
+        return (
+            super().redefines(other) or
+            (isinstance(other, Assignment) and self.name == other.name)
+        )
 
 
 class Builtin(Definition):
     """A definition created for all Python builtins."""
 
     def __init__(self, name):
         super().__init__(name, None)
@@ -517,16 +498,16 @@
         if '__all__' in scope and isinstance(source, ast.AugAssign):
             self.names = list(scope['__all__'].names)
         else:
             self.names = []
 
         def _add_to_names(container):
             for node in container.elts:
-                if isinstance(node, ast.Str):
-                    self.names.append(node.s)
+                if isinstance(node, ast.Constant) and isinstance(node.value, str):
+                    self.names.append(node.value)
 
         if isinstance(source.value, (ast.List, ast.Tuple)):
             _add_to_names(source.value)
         # If concatenating lists or tuples
         elif isinstance(source.value, ast.BinOp):
             currentValue = source.value
             while isinstance(currentValue.right, (ast.List, ast.Tuple)):
@@ -592,14 +573,18 @@
         Return a generator for the annotations which have not been used.
         """
         for name, binding in self.items():
             if not binding.used and isinstance(binding, Annotation):
                 yield name, binding
 
 
+class TypeScope(Scope):
+    pass
+
+
 class GeneratorScope(Scope):
     pass
 
 
 class ModuleScope(Scope):
     """Scope for a module."""
     _futures_allowed = True
@@ -726,25 +711,15 @@
     def in_annotation_func(self, *args, **kwargs):
         with self._enter_annotation(AnnotationState.STRING):
             return func(self, *args, **kwargs)
     return in_annotation_func
 
 
 class Checker:
-    """
-    I check the cleanliness and sanity of Python code.
-
-    @ivar _deferredFunctions: Tracking list used by L{deferFunction}.  Elements
-        of the list are two-tuples.  The first element is the callable passed
-        to L{deferFunction}.  The second element is a copy of the scope stack
-        at the time L{deferFunction} was called.
-
-    @ivar _deferredAssignments: Similar to C{_deferredFunctions}, but for
-        callables which are deferred assignment checks.
-    """
+    """I check the cleanliness and sanity of Python code."""
 
     _ast_node_scope = {
         ast.Module: ModuleScope,
         ast.ClassDef: ClassScope,
         ast.FunctionDef: FunctionScope,
         ast.AsyncFunctionDef: FunctionScope,
         ast.Lambda: FunctionScope,
@@ -753,53 +728,46 @@
         ast.GeneratorExp: GeneratorScope,
         ast.DictComp: GeneratorScope,
     }
 
     nodeDepth = 0
     offset = None
     _in_annotation = AnnotationState.NONE
-    _in_deferred = False
 
     builtIns = set(builtin_vars).union(_MAGIC_GLOBALS)
     _customBuiltIns = os.environ.get('PYFLAKES_BUILTINS')
     if _customBuiltIns:
         builtIns.update(_customBuiltIns.split(','))
     del _customBuiltIns
 
     def __init__(self, tree, filename='(none)', builtins=None,
                  withDoctest='PYFLAKES_DOCTEST' in os.environ, file_tokens=()):
         self._nodeHandlers = {}
-        self._deferredFunctions = []
-        self._deferredAssignments = []
+        self._deferred = collections.deque()
         self.deadScopes = []
         self.messages = []
         self.filename = filename
         if builtins:
             self.builtIns = self.builtIns.union(builtins)
         self.withDoctest = withDoctest
+        self.exceptHandlers = [()]
+        self.root = tree
+
+        self.scopeStack = []
         try:
-            self.scopeStack = [Checker._ast_node_scope[type(tree)]()]
+            scope_tp = Checker._ast_node_scope[type(tree)]
         except KeyError:
             raise RuntimeError('No scope implemented for the node %r' % tree)
-        self.exceptHandlers = [()]
-        self.root = tree
-        for builtin in self.builtIns:
-            self.addBinding(None, Builtin(builtin))
-        self.handleChildren(tree)
-        self._in_deferred = True
-        self.runDeferred(self._deferredFunctions)
-        # Set _deferredFunctions to None so that deferFunction will fail
-        # noisily if called after we've run through the deferred functions.
-        self._deferredFunctions = None
-        self.runDeferred(self._deferredAssignments)
-        # Set _deferredAssignments to None so that deferAssignment will fail
-        # noisily if called after we've run through the deferred assignments.
-        self._deferredAssignments = None
-        del self.scopeStack[1:]
-        self.popScope()
+
+        with self.in_scope(scope_tp):
+            for builtin in self.builtIns:
+                self.addBinding(None, Builtin(builtin))
+            self.handleChildren(tree)
+            self._run_deferred()
+
         self.checkDeadScopes()
 
         if file_tokens:
             warnings.warn(
                 '`file_tokens` will be removed in a future version',
                 stacklevel=2,
             )
@@ -809,32 +777,26 @@
         Schedule a function handler to be called just before completion.
 
         This is used for handling function bodies, which must be deferred
         because code later in the file might modify the global scope. When
         `callable` is called, the scope at the time this is called will be
         restored, however it will contain any new bindings added to it.
         """
-        self._deferredFunctions.append((callable, self.scopeStack[:], self.offset))
+        self._deferred.append((callable, self.scopeStack[:], self.offset))
 
-    def deferAssignment(self, callable):
-        """
-        Schedule an assignment handler to be called just after deferred
-        function handlers.
-        """
-        self._deferredAssignments.append((callable, self.scopeStack[:], self.offset))
+    def _run_deferred(self):
+        orig = (self.scopeStack, self.offset)
 
-    def runDeferred(self, deferred):
-        """
-        Run the callables in C{deferred} using their associated scope stack.
-        """
-        for handler, scope, offset in deferred:
-            self.scopeStack = scope
-            self.offset = offset
+        while self._deferred:
+            handler, scope, offset = self._deferred.popleft()
+            self.scopeStack, self.offset = scope, offset
             handler()
 
+        self.scopeStack, self.offset = orig
+
     def _in_doctest(self):
         return (len(self.scopeStack) >= 2 and
                 isinstance(self.scopeStack[1], DoctestScope))
 
     @property
     def futuresAllowed(self):
         if not all(isinstance(scope, ModuleScope)
@@ -862,27 +824,38 @@
         assert isinstance(self.scope, ModuleScope)
         self.scope._annotations_future_enabled = True
 
     @property
     def scope(self):
         return self.scopeStack[-1]
 
-    def popScope(self):
-        self.deadScopes.append(self.scopeStack.pop())
+    @contextlib.contextmanager
+    def in_scope(self, cls):
+        self.scopeStack.append(cls())
+        try:
+            yield
+        finally:
+            self.deadScopes.append(self.scopeStack.pop())
 
     def checkDeadScopes(self):
         """
         Look at scopes which have been fully examined and report names in them
         which were imported but unused.
         """
         for scope in self.deadScopes:
             # imports in classes are public members
             if isinstance(scope, ClassScope):
                 continue
 
+            if isinstance(scope, FunctionScope):
+                for name, binding in scope.unused_assignments():
+                    self.report(messages.UnusedVariable, binding.source, name)
+                for name, binding in scope.unused_annotations():
+                    self.report(messages.UnusedAnnotation, binding.source, name)
+
             all_binding = scope.get('__all__')
             if all_binding and not isinstance(all_binding, ExportBinding):
                 all_binding = None
 
             if all_binding:
                 all_names = set(all_binding.names)
                 undefined = [
@@ -925,17 +898,14 @@
                             messg = messages.ImportShadowedByLoopVar
                         elif used:
                             continue
                         else:
                             messg = messages.RedefinedWhileUnused
                         self.report(messg, node, value.name, value.source)
 
-    def pushScope(self, scopeClass=FunctionScope):
-        self.scopeStack.append(scopeClass())
-
     def report(self, messageClass, *args, **kwargs):
         self.messages.append(messageClass(self.filename, *args, **kwargs))
 
     def getParent(self, node):
         # Lookup the first parent which is not Tuple, List or Starred
         while True:
             node = node._pyflakes_parent
@@ -1069,31 +1039,36 @@
         return handler
 
     def handleNodeLoad(self, node, parent):
         name = getNodeName(node)
         if not name:
             return
 
-        in_generators = None
+        # only the following can access class scoped variables (since classes
+        # aren't really a scope)
+        # - direct accesses (not within a nested scope)
+        # - generators
+        # - type annotations (for generics, etc.)
+        can_access_class_vars = None
         importStarred = None
 
         # try enclosing function scopes and global scope
         for scope in self.scopeStack[-1::-1]:
             if isinstance(scope, ClassScope):
                 if name == '__class__':
                     return
-                elif in_generators is False:
+                elif can_access_class_vars is False:
                     # only generators used in a class scope can access the
                     # names of the class. this is skipped during the first
                     # iteration
                     continue
 
             binding = scope.get(name, None)
             if isinstance(binding, Annotation) and not self._in_postponed_annotation:
-                scope[name].used = True
+                scope[name].used = (self.scope, node)
                 continue
 
             if name == 'print' and isinstance(binding, Builtin):
                 if (isinstance(parent, ast.BinOp) and
                         isinstance(parent.op, ast.RShift)):
                     self.report(messages.InvalidPrintSyntax, node)
 
@@ -1112,16 +1087,18 @@
             except KeyError:
                 pass
             else:
                 return
 
             importStarred = importStarred or scope.importStarred
 
-            if in_generators is not False:
-                in_generators = isinstance(scope, GeneratorScope)
+            if can_access_class_vars is not False:
+                can_access_class_vars = isinstance(
+                    scope, (TypeScope, GeneratorScope),
+                )
 
         if importStarred:
             from_list = []
 
             for scope in self.scopeStack[-1::-1]:
                 for binding in scope.values():
                     if isinstance(binding, StarImportation):
@@ -1177,15 +1154,15 @@
                 isinstance(self.scope, ModuleScope) and
                 isinstance(
                     node._pyflakes_parent,
                     (ast.Assign, ast.AugAssign, ast.AnnAssign)
                 )
         ):
             binding = ExportBinding(name, node._pyflakes_parent, self.scope)
-        elif PY38_PLUS and isinstance(parent_stmt, ast.NamedExpr):
+        elif isinstance(parent_stmt, ast.NamedExpr):
             binding = NamedExprAssignment(name, node)
         else:
             binding = Assignment(name, node)
         self.addBinding(node, binding)
 
     def handleNodeDelete(self, node):
 
@@ -1244,39 +1221,42 @@
             return True
 
     def isDocstring(self, node):
         """
         Determine if the given node is a docstring, as long as it is at the
         correct place in the node tree.
         """
-        return isinstance(node, ast.Str) or (isinstance(node, ast.Expr) and
-                                             isinstance(node.value, ast.Str))
+        return (
+            isinstance(node, ast.Expr) and
+            isinstance(node.value, ast.Constant) and
+            isinstance(node.value.value, str)
+        )
 
     def getDocstring(self, node):
-        if isinstance(node, ast.Expr):
-            node = node.value
-        if not isinstance(node, ast.Str):
-            return (None, None)
-
-        if PYPY or PY38_PLUS:
-            doctest_lineno = node.lineno - 1
+        if (
+                isinstance(node, ast.Expr) and
+                isinstance(node.value, ast.Constant) and
+                isinstance(node.value.value, str)
+        ):
+            return node.value.value, node.lineno - 1
         else:
-            # Computed incorrectly if the docstring has backslash
-            doctest_lineno = node.lineno - node.s.count('\n') - 1
-
-        return (node.s, doctest_lineno)
+            return None, None
 
     def handleNode(self, node, parent):
         if node is None:
             return
         if self.offset and getattr(node, 'lineno', None) is not None:
             node.lineno += self.offset[0]
             node.col_offset += self.offset[1]
-        if self.futuresAllowed and not (isinstance(node, ast.ImportFrom) or
-                                        self.isDocstring(node)):
+        if (
+                self.futuresAllowed and
+                self.nodeDepth == 0 and
+                not isinstance(node, ast.ImportFrom) and
+                not self.isDocstring(node)
+        ):
             self.futuresAllowed = False
         self.nodeDepth += 1
         node._pyflakes_depth = self.nodeDepth
         node._pyflakes_parent = parent
         try:
             handler = self.getNodeHandler(node.__class__)
             handler(node)
@@ -1296,30 +1276,29 @@
         if not examples:
             return
 
         # Place doctest in module scope
         saved_stack = self.scopeStack
         self.scopeStack = [self.scopeStack[0]]
         node_offset = self.offset or (0, 0)
-        self.pushScope(DoctestScope)
-        if '_' not in self.scopeStack[0]:
-            self.addBinding(None, Builtin('_'))
-        for example in examples:
-            try:
-                tree = ast.parse(example.source, "<doctest>")
-            except SyntaxError as e:
-                position = (node_lineno + example.lineno + e.lineno,
-                            example.indent + 4 + (e.offset or 0))
-                self.report(messages.DoctestSyntaxError, node, position)
-            else:
-                self.offset = (node_offset[0] + node_lineno + example.lineno,
-                               node_offset[1] + example.indent + 4)
-                self.handleChildren(tree)
-                self.offset = node_offset
-        self.popScope()
+        with self.in_scope(DoctestScope):
+            if '_' not in self.scopeStack[0]:
+                self.addBinding(None, Builtin('_'))
+            for example in examples:
+                try:
+                    tree = ast.parse(example.source, "<doctest>")
+                except SyntaxError as e:
+                    position = (node_lineno + example.lineno + e.lineno,
+                                example.indent + 4 + (e.offset or 0))
+                    self.report(messages.DoctestSyntaxError, node, position)
+                else:
+                    self.offset = (node_offset[0] + node_lineno + example.lineno,
+                                   node_offset[1] + example.indent + 4)
+                    self.handleChildren(tree)
+                    self.offset = node_offset
         self.scopeStack = saved_stack
 
     @in_string_annotation
     def handleStringAnnotation(self, s, node, ref_lineno, ref_col_offset, err):
         try:
             tree = ast.parse(s)
         except SyntaxError:
@@ -1338,29 +1317,35 @@
                     'col_offset' in descendant._attributes
             ):
                 descendant.lineno = ref_lineno
                 descendant.col_offset = ref_col_offset
 
         self.handleNode(parsed_annotation, node)
 
+    def handle_annotation_always_deferred(self, annotation, parent):
+        fn = in_annotation(Checker.handleNode)
+        self.deferFunction(lambda: fn(self, annotation, parent))
+
     @in_annotation
     def handleAnnotation(self, annotation, node):
-        if isinstance(annotation, ast.Str):
+        if (
+                isinstance(annotation, ast.Constant) and
+                isinstance(annotation.value, str)
+        ):
             # Defer handling forward annotation.
             self.deferFunction(functools.partial(
                 self.handleStringAnnotation,
-                annotation.s,
+                annotation.value,
                 node,
                 annotation.lineno,
                 annotation.col_offset,
                 messages.ForwardAnnotationSyntaxError,
             ))
         elif self.annotationsFutureEnabled:
-            fn = in_annotation(Checker.handleNode)
-            self.deferFunction(lambda: fn(self, annotation, node))
+            self.handle_annotation_always_deferred(annotation, node)
         else:
             self.handleNode(annotation, node)
 
     def ignore(self, node):
         pass
 
     # "stmt" type nodes
@@ -1409,15 +1394,15 @@
                 with self._enter_annotation():
                     self.handleChildren(node)
             else:
                 self.handleChildren(node)
 
     def _handle_string_dot_format(self, node):
         try:
-            placeholders = tuple(parse_format_string(node.func.value.s))
+            placeholders = tuple(parse_format_string(node.func.value.value))
         except ValueError as e:
             self.report(messages.StringDotFormatInvalidFormat, node, e)
             return
 
         auto = None
         next_auto = 0
 
@@ -1525,15 +1510,16 @@
                 node,
                 ', '.join(sorted(str(x) for x in missing_arguments)),
             )
 
     def CALL(self, node):
         if (
                 isinstance(node.func, ast.Attribute) and
-                isinstance(node.func.value, ast.Str) and
+                isinstance(node.func.value, ast.Constant) and
+                isinstance(node.func.value.value, str) and
                 node.func.attr == 'format'
         ):
             self._handle_string_dot_format(node)
 
         omit = []
         annotated = []
         not_annotated = []
@@ -1606,15 +1592,15 @@
                 for annotated_node in annotated:
                     self.handleNode(annotated_node, node)
         else:
             self.handleChildren(node)
 
     def _handle_percent_format(self, node):
         try:
-            placeholders = parse_percent_format(node.left.s)
+            placeholders = parse_percent_format(node.left.value)
         except ValueError:
             self.report(
                 messages.PercentFormatInvalidFormat,
                 node,
                 'incomplete format',
             )
             return
@@ -1685,21 +1671,24 @@
                     substitution_count,
                 )
             elif not positional:
                 self.report(messages.PercentFormatExpectedMapping, node)
 
         if (
                 isinstance(node.right, ast.Dict) and
-                all(isinstance(k, ast.Str) for k in node.right.keys)
+                all(
+                    isinstance(k, ast.Constant) and isinstance(k.value, str)
+                    for k in node.right.keys
+                )
         ):
             if positional and positional_count > 1:
                 self.report(messages.PercentFormatExpectedSequence, node)
                 return
 
-            substitution_keys = {k.s for k in node.right.keys}
+            substitution_keys = {k.value for k in node.right.keys}
             extra_keys = substitution_keys - named
             missing_keys = named - substitution_keys
             if not positional and extra_keys:
                 self.report(
                     messages.PercentFormatExtraNamedArguments,
                     node,
                     ', '.join(sorted(extra_keys)),
@@ -1710,40 +1699,31 @@
                     node,
                     ', '.join(sorted(missing_keys)),
                 )
 
     def BINOP(self, node):
         if (
                 isinstance(node.op, ast.Mod) and
-                isinstance(node.left, ast.Str)
+                isinstance(node.left, ast.Constant) and
+                isinstance(node.left.value, str)
         ):
             self._handle_percent_format(node)
         self.handleChildren(node)
 
-    def STR(self, node):
-        if self._in_annotation:
+    def CONSTANT(self, node):
+        if isinstance(node.value, str) and self._in_annotation:
             fn = functools.partial(
                 self.handleStringAnnotation,
-                node.s,
+                node.value,
                 node,
                 node.lineno,
                 node.col_offset,
                 messages.ForwardAnnotationSyntaxError,
             )
-            if self._in_deferred:
-                fn()
-            else:
-                self.deferFunction(fn)
-
-    if PY38_PLUS:
-        def CONSTANT(self, node):
-            if isinstance(node.value, str):
-                return self.STR(node)
-    else:
-        NUM = BYTES = ELLIPSIS = CONSTANT = ignore
+            self.deferFunction(fn)
 
     # "slice" type nodes
     SLICE = EXTSLICE = INDEX = handleChildren
 
     # expression contexts are node instances too, though being constants
     LOAD = STORE = DEL = AUGLOAD = AUGSTORE = PARAM = ignore
 
@@ -1863,17 +1843,16 @@
                 node_value.used = (global_scope, node)
                 for scope in self.scopeStack[global_scope_index + 1:]:
                     scope[node_name] = node_value
 
     NONLOCAL = GLOBAL
 
     def GENERATOREXP(self, node):
-        self.pushScope(GeneratorScope)
-        self.handleChildren(node)
-        self.popScope()
+        with self.in_scope(GeneratorScope):
+            self.handleChildren(node)
 
     LISTCOMP = DICTCOMP = SETCOMP = GENERATOREXP
 
     def NAME(self, node):
         """
         Handle occurrence of Name (which can be a load/store/delete access.)
         """
@@ -1901,19 +1880,14 @@
             n, n_child = n._pyflakes_parent, n
             if isinstance(n, (ast.While, ast.For, ast.AsyncFor)):
                 # Doesn't apply unless it's in the loop itself
                 if n_child not in n.orelse:
                     return
             if isinstance(n, (ast.FunctionDef, ast.ClassDef)):
                 break
-            # Handle Try/TryFinally difference in Python < and >= 3.3
-            if hasattr(n, 'finalbody') and isinstance(node, ast.Continue):
-                if n_child in n.finalbody and not PY38_PLUS:
-                    self.report(messages.ContinueInFinally, node)
-                    return
         if isinstance(node, ast.Continue):
             self.report(messages.ContinueOutsideLoop, node)
         else:  # ast.Break
             self.report(messages.BreakOutsideLoop, node)
 
     BREAK = CONTINUE
 
@@ -1938,33 +1912,35 @@
         self.handleNode(node.value, node)
 
     AWAIT = YIELDFROM = YIELD
 
     def FUNCTIONDEF(self, node):
         for deco in node.decorator_list:
             self.handleNode(deco, node)
-        self.LAMBDA(node)
+
+        with self._type_param_scope(node):
+            self.LAMBDA(node)
+
         self.addBinding(node, FunctionDefinition(node.name, node))
         # doctest does not process doctest within a doctest,
         # or in nested functions.
         if (self.withDoctest and
                 not self._in_doctest() and
                 not isinstance(self.scope, FunctionScope)):
             self.deferFunction(lambda: self.handleDoctests(node))
 
     ASYNCFUNCTIONDEF = FUNCTIONDEF
 
     def LAMBDA(self, node):
         args = []
         annotations = []
 
-        if PY38_PLUS:
-            for arg in node.args.posonlyargs:
-                args.append(arg.arg)
-                annotations.append(arg.annotation)
+        for arg in node.args.posonlyargs:
+            args.append(arg.arg)
+            annotations.append(arg.annotation)
         for arg in node.args.args + node.args.kwonlyargs:
             args.append(arg.arg)
             annotations.append(arg.annotation)
         defaults = node.args.defaults + node.args.kw_defaults
 
         has_annotations = not isinstance(node, ast.Lambda)
 
@@ -1987,37 +1963,19 @@
         for annotation in annotations:
             self.handleAnnotation(annotation, node)
 
         for default in defaults:
             self.handleNode(default, node)
 
         def runFunction():
-
-            self.pushScope()
-
-            self.handleChildren(node, omit=['decorator_list', 'returns'])
-
-            def check_unused_assignments():
-                """
-                Check to see if any assignments have not been used.
-                """
-                for name, binding in self.scope.unused_assignments():
-                    self.report(messages.UnusedVariable, binding.source, name)
-
-            def check_unused_annotations():
-                """
-                Check to see if any annotations have not been used.
-                """
-                for name, binding in self.scope.unused_annotations():
-                    self.report(messages.UnusedAnnotation, binding.source, name)
-
-            self.deferAssignment(check_unused_assignments)
-            self.deferAssignment(check_unused_annotations)
-
-            self.popScope()
+            with self.in_scope(FunctionScope):
+                self.handleChildren(
+                    node,
+                    omit=('decorator_list', 'returns', 'type_params'),
+                )
 
         self.deferFunction(runFunction)
 
     def ARGUMENTS(self, node):
         self.handleChildren(node, omit=('defaults', 'kw_defaults'))
 
     def ARG(self, node):
@@ -2027,28 +1985,30 @@
         """
         Check names used in a class definition, including its decorators, base
         classes, and the body of its definition.  Additionally, add its name to
         the current scope.
         """
         for deco in node.decorator_list:
             self.handleNode(deco, node)
-        for baseNode in node.bases:
-            self.handleNode(baseNode, node)
-        for keywordNode in node.keywords:
-            self.handleNode(keywordNode, node)
-        self.pushScope(ClassScope)
-        # doctest does not process doctest within a doctest
-        # classes within classes are processed.
-        if (self.withDoctest and
-                not self._in_doctest() and
-                not isinstance(self.scope, FunctionScope)):
-            self.deferFunction(lambda: self.handleDoctests(node))
-        for stmt in node.body:
-            self.handleNode(stmt, node)
-        self.popScope()
+
+        with self._type_param_scope(node):
+            for baseNode in node.bases:
+                self.handleNode(baseNode, node)
+            for keywordNode in node.keywords:
+                self.handleNode(keywordNode, node)
+            with self.in_scope(ClassScope):
+                # doctest does not process doctest within a doctest
+                # classes within classes are processed.
+                if (self.withDoctest and
+                        not self._in_doctest() and
+                        not isinstance(self.scope, FunctionScope)):
+                    self.deferFunction(lambda: self.handleDoctests(node))
+                for stmt in node.body:
+                    self.handleNode(stmt, node)
+
         self.addBinding(node, ClassDefinition(node.name, node))
 
     def AUGASSIGN(self, node):
         self.handleNodeLoad(node.target, node)
         self.handleNode(node.value, node)
         self.handleNode(node.target, node)
 
@@ -2214,7 +2174,25 @@
     MATCHSINGLETON = MATCHVALUE = handleChildren
 
     def _match_target(self, node):
         self.handleNodeStore(node)
         self.handleChildren(node)
 
     MATCHAS = MATCHMAPPING = MATCHSTAR = _match_target
+
+    @contextlib.contextmanager
+    def _type_param_scope(self, node):
+        with contextlib.ExitStack() as ctx:
+            if sys.version_info >= (3, 12):
+                ctx.enter_context(self.in_scope(TypeScope))
+                for param in node.type_params:
+                    self.handleNode(param, node)
+            yield
+
+    def TYPEVAR(self, node):
+        self.handleNodeStore(node)
+        self.handle_annotation_always_deferred(node.bound, node)
+
+    def TYPEALIAS(self, node):
+        self.handleNode(node.name, node)
+        with self._type_param_scope(node):
+            self.handle_annotation_always_deferred(node.value, node)
```

### Comparing `pyflakes-3.0.1/pyflakes/messages.py` & `pyflakes-3.1.0/pyflakes/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,21 +194,14 @@
 class BreakOutsideLoop(Message):
     """
     Indicates a break statement outside of a while or for loop.
     """
     message = '\'break\' outside loop'
 
 
-class ContinueInFinally(Message):
-    """
-    Indicates a continue statement in a finally block in a while or for loop.
-    """
-    message = '\'continue\' not supported inside \'finally\' clause'
-
-
 class DefaultExceptNotLast(Message):
     """
     Indicates an except: block as not the last exception handler.
     """
     message = 'default \'except:\' must be last'
```

### Comparing `pyflakes-3.0.1/pyflakes/reporter.py` & `pyflakes-3.1.0/pyflakes/reporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,20 +52,19 @@
         @ptype text: C{unicode}
         """
         if text is None:
             line = None
         else:
             line = text.splitlines()[-1]
 
+        # lineno might be None if the error was during tokenization
         # lineno might be 0 if the error came from stdin
-        lineno = max(lineno, 1)
+        lineno = max(lineno or 0, 1)
 
         if offset is not None:
-            if sys.version_info < (3, 8) and text is not None:
-                offset = offset - (len(text) - len(line)) + 1
             # some versions of python emit an offset of -1 for certain encoding errors
             offset = max(offset, 1)
             self._stderr.write('%s:%d:%d: %s\n' %
                                (filename, lineno, offset, msg))
         else:
             self._stderr.write('%s:%d: %s\n' % (filename, lineno, msg))
```

### Comparing `pyflakes-3.0.1/pyflakes/test/harness.py` & `pyflakes-3.1.0/pyflakes/test/harness.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes/test/test_api.py` & `pyflakes-3.1.0/pyflakes/test/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,17 +229,15 @@
         C{syntaxError} reports that there was a syntax error in the source
         file.  It reports to the error stream and includes the filename, line
         number, error message, actual line of source and a caret pointing to
         where the error is.
         """
         err = io.StringIO()
         reporter = Reporter(None, err)
-        reporter.syntaxError('foo.py', 'a problem', 3,
-                             8 if sys.version_info >= (3, 8) else 7,
-                             'bad line of source')
+        reporter.syntaxError('foo.py', 'a problem', 3, 8, 'bad line of source')
         self.assertEqual(
             ("foo.py:3:8: a problem\n"
              "bad line of source\n"
              "       ^\n"),
             err.getvalue())
 
     def test_syntaxErrorNoOffset(self):
@@ -277,19 +275,18 @@
         lines = [
             'bad line of source',
             'more bad lines of source',
         ]
         reporter = Reporter(None, err)
         reporter.syntaxError('foo.py', 'a problem', 3, len(lines[0]) + 7,
                              '\n'.join(lines))
-        column = 25 if sys.version_info >= (3, 8) else 7
         self.assertEqual(
-            ("foo.py:3:%d: a problem\n" % column +
+            ("foo.py:3:25: a problem\n" +
              lines[-1] + "\n" +
-             " " * (column - 1) + "^\n"),
+             " " * 24 + "^\n"),
             err.getvalue())
 
     def test_unexpectedError(self):
         """
         C{unexpectedError} reports an error processing a source file.
         """
         err = io.StringIO()
@@ -413,18 +410,16 @@
             elif sys.version_info >= (3, 10):
                 message = 'unterminated triple-quoted string literal (detected at line 8)'  # noqa: E501
             else:
                 message = 'invalid syntax'
 
             if PYPY or sys.version_info >= (3, 10):
                 column = 12
-            elif sys.version_info >= (3, 8):
-                column = 8
             else:
-                column = 11
+                column = 8
             self.assertHasErrors(
                 sourcePath,
                 ["""\
 %s:8:%d: %s
     '''quux'''
 %s^
 """ % (sourcePath, column, message, ' ' * (column - 1))])
@@ -475,48 +470,51 @@
         exceptions do not include an offset.
         """
         source = """\
 def foo(bar=baz, bax):
     pass
 """
         with self.makeTempFile(source) as sourcePath:
+            if sys.version_info >= (3, 12):
+                msg = 'parameter without a default follows parameter with a default'  # noqa: E501
+            else:
+                msg = 'non-default argument follows default argument'
+
             if PYPY and sys.version_info >= (3, 9):
                 column = 18
             elif PYPY:
                 column = 8
             elif sys.version_info >= (3, 10):
                 column = 18
             elif sys.version_info >= (3, 9):
                 column = 21
-            elif sys.version_info >= (3, 8):
-                column = 9
             else:
-                column = 8
+                column = 9
             last_line = ' ' * (column - 1) + '^\n'
-            columnstr = '%d:' % column
             self.assertHasErrors(
                 sourcePath,
-                ["""\
-{}:1:{} non-default argument follows default argument
+                [f"""\
+{sourcePath}:1:{column}: {msg}
 def foo(bar=baz, bax):
-{}""".format(sourcePath, columnstr, last_line)])
+{last_line}"""]
+            )
 
     def test_nonKeywordAfterKeywordSyntaxError(self):
         """
         Source which has a non-keyword argument after a keyword argument should
         include the line number of the syntax error.  However these exceptions
         do not include an offset.
         """
         source = """\
 foo(bar=baz, bax)
 """
         with self.makeTempFile(source) as sourcePath:
             if sys.version_info >= (3, 9):
                 column = 17
-            elif not PYPY and sys.version_info >= (3, 8):
+            elif not PYPY:
                 column = 14
             else:
                 column = 13
             last_line = ' ' * (column - 1) + '^\n'
             columnstr = '%d:' % column
 
             message = 'positional argument follows keyword argument'
@@ -535,15 +533,15 @@
         # ValueError: invalid \x escape
         with self.makeTempFile(r"foo = '\xyz'") as sourcePath:
             position_end = 1
             if PYPY and sys.version_info >= (3, 9):
                 column = 7
             elif PYPY:
                 column = 6
-            elif sys.version_info >= (3, 9):
+            elif (3, 9) <= sys.version_info < (3, 12):
                 column = 13
             else:
                 column = 7
 
             last_line = '%s^\n' % (' ' * (column - 1))
 
             decoding_error = """\
@@ -624,16 +622,20 @@
         """
         SNOWMAN = chr(0x2603)
         source = ("""\
 # coding: ascii
 x = "%s"
 """ % SNOWMAN).encode('utf-16')
         with self.makeTempFile(source) as sourcePath:
-            self.assertHasErrors(
-                sourcePath, [f"{sourcePath}: problem decoding source\n"])
+            if sys.version_info < (3, 11, 4):
+                expected = f"{sourcePath}: problem decoding source\n"
+            else:
+                expected = f"{sourcePath}:1: source code string cannot contain null bytes\n"  # noqa: E501
+
+            self.assertHasErrors(sourcePath, [expected])
 
     def test_checkRecursive(self):
         """
         L{checkRecursive} descends into each directory, finding Python files
         and reporting problems.
         """
         tempdir = tempfile.mkdtemp()
@@ -675,26 +677,18 @@
             ]
         elif PYPY:
             expected_error = [
                 "<stdin>:1:4: Generator expression must be parenthesized if not sole argument",  # noqa: E501
                 "max(1 for i in range(10), key=lambda x: x+1)",
                 "   ^",
             ]
-        elif sys.version_info >= (3, 8):
+        else:
             expected_error = [
                 "<stdin>:1:5: Generator expression must be parenthesized",
             ]
-        elif sys.version_info >= (3, 7):
-            expected_error = [
-                "<stdin>:1:4: Generator expression must be parenthesized",
-            ]
-        elif sys.version_info >= (3, 6):
-            expected_error = [
-                "<stdin>:1:4: Generator expression must be parenthesized if not sole argument",  # noqa: E501
-            ]
 
         self.assertEqual(errlines, expected_error)
 
 
 class IntegrationTests(TestCase):
     """
     Tests of the pyflakes script that actually spawn the script.
```

### Comparing `pyflakes-3.0.1/pyflakes/test/test_builtin.py` & `pyflakes-3.1.0/pyflakes/test/test_builtin.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes/test/test_code_segment.py` & `pyflakes-3.1.0/pyflakes/test/test_code_segment.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes/test/test_dict.py` & `pyflakes-3.1.0/pyflakes/test/test_dict.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes/test/test_doctests.py` & `pyflakes-3.1.0/pyflakes/test/test_doctests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 import textwrap
 
 from pyflakes import messages as m
 from pyflakes.checker import (
     PYPY,
     DoctestScope,
     FunctionScope,
@@ -319,15 +318,15 @@
                 """
             ''',
             m.DoctestSyntaxError,
             m.DoctestSyntaxError,
             m.DoctestSyntaxError).messages
         exc = exceptions[0]
         self.assertEqual(exc.lineno, 4)
-        if not PYPY and sys.version_info >= (3, 8):
+        if not PYPY:
             self.assertEqual(exc.col, 18)
         else:
             self.assertEqual(exc.col, 26)
 
         # PyPy error column offset is 0,
         # for the second and third line of the doctest
         # i.e. at the beginning of the line
@@ -335,32 +334,26 @@
         self.assertEqual(exc.lineno, 5)
         if PYPY:
             self.assertEqual(exc.col, 13)
         else:
             self.assertEqual(exc.col, 16)
         exc = exceptions[2]
         self.assertEqual(exc.lineno, 6)
-        if PYPY or sys.version_info >= (3, 8):
-            self.assertEqual(exc.col, 13)
-        else:
-            self.assertEqual(exc.col, 18)
+        self.assertEqual(exc.col, 13)
 
     def test_indentationErrorInDoctest(self):
         exc = self.flakes('''
         def doctest_stuff():
             """
                 >>> if True:
                 ... pass
             """
         ''', m.DoctestSyntaxError).messages[0]
         self.assertEqual(exc.lineno, 5)
-        if PYPY or sys.version_info >= (3, 8):
-            self.assertEqual(exc.col, 13)
-        else:
-            self.assertEqual(exc.col, 16)
+        self.assertEqual(exc.col, 13)
 
     def test_offsetWithMultiLineArgs(self):
         (exc1, exc2) = self.flakes(
             '''
             def doctest_stuff(arg1,
                               arg2,
                               arg3):
```

### Comparing `pyflakes-3.0.1/pyflakes/test/test_imports.py` & `pyflakes-3.1.0/pyflakes/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes/test/test_is_literal.py` & `pyflakes-3.1.0/pyflakes/test/test_is_literal.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes/test/test_match.py` & `pyflakes-3.1.0/pyflakes/test/test_match.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,7 +77,18 @@
     def test_match_double_star(self):
         self.flakes('''
             x = {'foo': 'bar', 'baz': 'womp'}
             match x:
                 case {'foo': k1, **rest}:
                     print(f'{k1=} {rest=}')
         ''')
+
+    def test_defined_in_different_branches(self):
+        self.flakes('''
+            def f(x):
+                match x:
+                    case 1:
+                        def y(): pass
+                    case _:
+                        def y(): print(1)
+                return y
+        ''')
```

### Comparing `pyflakes-3.0.1/pyflakes/test/test_other.py` & `pyflakes-3.1.0/pyflakes/test/test_other.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,20 @@
         warning.
         """
         self.flakes('''
         def a(): pass
         def a(): pass
         ''', m.RedefinedWhileUnused)
 
+    def test_redefined_function_shadows_variable(self):
+        self.flakes('''
+        x = 1
+        def x(): pass
+        ''', m.RedefinedWhileUnused)
+
     def test_redefinedUnderscoreFunction(self):
         """
         Test that shadowing a function definition named with underscore doesn't
         raise anything.
         """
         self.flakes('''
         def _(): pass
@@ -441,44 +447,14 @@
             try:
                 pass
             finally:
                 while True:
                     continue
         ''')
 
-    @skipIf(version_info > (3, 8), "Python <= 3.8 only")
-    def test_continueInFinally(self):
-        # 'continue' inside 'finally' is a special syntax error
-        # that is removed in 3.8
-        self.flakes('''
-        while True:
-            try:
-                pass
-            finally:
-                continue
-        ''', m.ContinueInFinally)
-
-        self.flakes('''
-        while True:
-            try:
-                pass
-            finally:
-                if 1:
-                    if 2:
-                        continue
-        ''', m.ContinueInFinally)
-
-        # Even when not in a loop, this is the error Python gives
-        self.flakes('''
-        try:
-            pass
-        finally:
-            continue
-        ''', m.ContinueInFinally)
-
     def test_breakOutsideLoop(self):
         self.flakes('''
         break
         ''', m.BreakOutsideLoop)
 
         self.flakes('''
         def f():
@@ -1712,32 +1688,29 @@
     def test_f_string(self):
         """Test PEP 498 f-strings are treated as a usage."""
         self.flakes('''
         baz = 0
         print(f'\x7b4*baz\N{RIGHT CURLY BRACKET}')
         ''')
 
-    @skipIf(version_info < (3, 8), 'new in Python 3.8')
     def test_assign_expr(self):
         """Test PEP 572 assignment expressions are treated as usage / write."""
         self.flakes('''
         from foo import y
         print(x := y)
         print(x)
         ''')
 
-    @skipIf(version_info < (3, 8), 'new in Python 3.8')
     def test_assign_expr_generator_scope(self):
         """Test assignment expressions in generator expressions."""
         self.flakes('''
         if (any((y := x[0]) for x in [[True]])):
             print(y)
         ''')
 
-    @skipIf(version_info < (3, 8), 'new in Python 3.8')
     def test_assign_expr_nested(self):
         """Test assignment expressions in nested expressions."""
         self.flakes('''
         if ([(y:=x) for x in range(4) if [(z:=q) for q in range(4)]]):
             print(y)
             print(z)
         ''')
@@ -1968,27 +1941,14 @@
             async for row in db.cursor():
                 output.append(row)
             else:
                 break
             return output
         ''', m.BreakOutsideLoop)
 
-    @skipIf(version_info > (3, 8), "Python <= 3.8 only")
-    def test_continueInAsyncForFinally(self):
-        self.flakes('''
-        async def read_data(db):
-            output = []
-            async for row in db.cursor():
-                try:
-                    output.append(row)
-                finally:
-                    continue
-            return output
-        ''', m.ContinueInFinally)
-
     def test_asyncWith(self):
         self.flakes('''
         async def commit(session, data):
             async with session.transaction():
                 await session.update(data)
         ''')
```

### Comparing `pyflakes-3.0.1/pyflakes/test/test_type_annotations.py` & `pyflakes-3.1.0/pyflakes/test/test_type_annotations.py`

 * *Files 12% similar despite different names*

```diff
@@ -363,27 +363,33 @@
         # This should only print one UnusedVariable message
         self.flakes('''
         def f():
             x: int
             x = 3
         ''', m.UnusedVariable)
 
+    def test_unused_annotation_in_outer_scope_reassigned_in_local_scope(self):
+        self.flakes('''
+        x: int
+        x.__dict__
+        def f(): x = 1
+        ''', m.UndefinedName, m.UnusedVariable)
+
     def test_unassigned_annotation_is_undefined(self):
         self.flakes('''
         name: str
         print(name)
         ''', m.UndefinedName)
 
     def test_annotated_async_def(self):
         self.flakes('''
         class c: pass
         async def func(c: c) -> None: pass
         ''')
 
-    @skipIf(version_info < (3, 7), 'new in Python 3.7')
     def test_postponed_annotations(self):
         self.flakes('''
         from __future__ import annotations
         def f(a: A) -> A: pass
         class A:
             b: B
         class B: pass
@@ -430,15 +436,14 @@
         self.flakes("""
         class Test:
             def t(self) -> Y:
                 Y = 2
                 return Y
         """, m.UndefinedName)
 
-    @skipIf(version_info < (3, 8), 'new in Python 3.8')
     def test_positional_only_argument_annotations(self):
         self.flakes("""
         from x import C
 
         def f(c: C, /): ...
         """)
 
@@ -580,27 +585,40 @@
             from typing import Optional
 
 
             def f() -> "Optional['Queue[str]']":
                 return None
         """)
 
-    @skipIf(version_info < (3, 7), 'new in Python 3.7')
     def test_partial_string_annotations_with_future_annotations(self):
         self.flakes("""
             from __future__ import annotations
 
             from queue import Queue
             from typing import Optional
 
 
             def f() -> Optional['Queue[str]']:
                 return None
         """)
 
+    def test_forward_annotations_for_classes_in_scope(self):
+        # see #749
+        self.flakes("""
+        from typing import Optional
+
+        def f():
+            class C:
+                a: "D"
+                b: Optional["D"]
+                c: "Optional[D]"
+
+            class D: pass
+        """)
+
     def test_idomiatic_typing_guards(self):
         # typing.TYPE_CHECKING: python3.5.3+
         self.flakes("""
             from typing import TYPE_CHECKING
 
             if TYPE_CHECKING:
                 from t import T
@@ -691,7 +709,74 @@
 
             class Shape(Generic[*Ts]): pass
 
             def f(*args: *Ts) -> None: ...
 
             def g(x: Shape[*Ts]) -> Shape[*Ts]: ...
         """)
+
+    @skipIf(version_info < (3, 12), 'new in Python 3.12')
+    def test_type_statements(self):
+        self.flakes("""
+            type ListOrSet[T] = list[T] | set[T]
+
+            def f(x: ListOrSet[str]) -> None: ...
+
+            type RecursiveType = int | list[RecursiveType]
+
+            type ForwardRef = int | C
+
+            type ForwardRefInBounds[T: C] = T
+
+            class C: pass
+        """)
+
+    @skipIf(version_info < (3, 12), 'new in Python 3.12')
+    def test_type_parameters_functions(self):
+        self.flakes("""
+            def f[T](t: T) -> T: return t
+
+            async def g[T](t: T) -> T: return t
+
+            def with_forward_ref[T: C](t: T) -> T: return t
+
+            def can_access_inside[T](t: T) -> T:
+                print(T)
+                return t
+
+            class C: pass
+        """)
+
+    @skipIf(version_info < (3, 12), 'new in Python 3.12')
+    def test_type_parameters_do_not_escape_function_scopes(self):
+        self.flakes("""
+            from x import g
+
+            @g(T)  # not accessible in decorators
+            def f[T](t: T) -> T: return t
+
+            T  # not accessible afterwards
+        """, m.UndefinedName, m.UndefinedName)
+
+    @skipIf(version_info < (3, 12), 'new in Python 3.12')
+    def test_type_parameters_classes(self):
+        self.flakes("""
+            class C[T](list[T]): pass
+
+            class UsesForward[T: Forward](list[T]): pass
+
+            class Forward: pass
+
+            class WithinBody[T](list[T]):
+                t = T
+        """)
+
+    @skipIf(version_info < (3, 12), 'new in Python 3.12')
+    def test_type_parameters_do_not_escape_class_scopes(self):
+        self.flakes("""
+            from x import g
+
+            @g(T)  # not accessible in decorators
+            class C[T](list[T]): pass
+
+            T  # not accessible afterwards
+        """, m.UndefinedName, m.UndefinedName)
```

### Comparing `pyflakes-3.0.1/pyflakes/test/test_undefined_names.py` & `pyflakes-3.1.0/pyflakes/test/test_undefined_names.py`

 * *Files identical despite different names*

### Comparing `pyflakes-3.0.1/pyflakes.egg-info/PKG-INFO` & `pyflakes-3.1.0/pyflakes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: pyflakes
-Version: 3.0.1
+Version: 3.1.0
 Summary: passive checker of Python programs
 Home-page: https://github.com/PyCQA/pyflakes
 Author: A lot of people
 Author-email: code-quality@python.org
 License: MIT
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 ========
 Pyflakes
 ========
 
 A simple program which checks Python source files for errors.
@@ -85,16 +80,16 @@
 <https://mail.python.org/mailman/listinfo/code-quality>`_
 
 Contributing
 ------------
 
 Issues are tracked on `GitHub <https://github.com/PyCQA/pyflakes/issues>`_.
 
-Patches may be submitted via a `GitHub pull request`_ or via the mailing list
-if you prefer. If you are comfortable doing so, please `rebase your changes`_
+Patches may be submitted via a `GitHub pull request`_.
+If you are comfortable doing so, please `rebase your changes`_
 so they may be applied to main with a fast-forward merge, and each commit is
 a coherent unit of work with a well-written log message.  If you are not
 comfortable with this rebase workflow, the project maintainers will be happy to
 rebase your commits for you.
 
 All changes should include tests and pass flake8_.
```

### Comparing `pyflakes-3.0.1/pyflakes.egg-info/SOURCES.txt` & `pyflakes-3.1.0/pyflakes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

