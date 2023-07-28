# Comparing `tmp/pygetsource-0.1.0.tar.gz` & `tmp/pygetsource-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygetsource-0.1.0.tar", last modified: Sun Jul 23 22:00:58 2023, max compression
+gzip compressed data, was "pygetsource-0.1.1.tar", last modified: Fri Jul 28 23:34:23 2023, max compression
```

## Comparing `pygetsource-0.1.0.tar` & `pygetsource-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-23 22:00:43.000000 pygetsource-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-23 22:00:58.184706 pygetsource-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-23 22:00:43.000000 pygetsource-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/pygetsource/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75980 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/decompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pygetsource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/pygetsource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-23 22:00:58.000000 pygetsource-0.1.0/pygetsource.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-23 22:00:43.000000 pygetsource-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 22:00:58.184706 pygetsource-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 22:00:58.184706 pygetsource-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-23 22:00:43.000000 pygetsource-0.1.0/tests/test_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-07-23 22:00:43.000000 pygetsource-0.1.0/tests/test_py37.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-23 22:00:43.000000 pygetsource-0.1.0/tests/test_rebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 23:34:13.000000 pygetsource-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-28 23:34:23.655079 pygetsource-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-28 23:34:13.000000 pygetsource-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/pygetsource/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67241 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/decompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/pygetsource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:34:23.655079 pygetsource-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 23:34:13.000000 pygetsource-0.1.1/tests/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-07-28 23:34:13.000000 pygetsource-0.1.1/tests/test_py37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-28 23:34:13.000000 pygetsource-0.1.1/tests/test_rebuild.py
```

### Comparing `pygetsource-0.1.0/LICENSE` & `pygetsource-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygetsource-0.1.0/PKG-INFO` & `pygetsource-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygetsource
-Version: 0.1.0
+Version: 0.1.1
 Summary: Decompiler written in Python for Python
 Author-email: Perceval Wajsburt <perceval.wajsburt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Perceval Wajsburt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,22 +28,24 @@
 Project-URL: homepage, https://github.com/perceval/pygetsource/
 Project-URL: repository, https://github.com/perceval/pygetsource/
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-<a href="https://github.com/psf/black/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
-<a href="https://pypi.org/project/pygetsource/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pygetsource"></a>
-<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+[![Codecov](https://img.shields.io/codecov/c/github/percevalw/pygetsource?logo=codecov&style=flat-square)](https://codecov.io/gh/percevalw/pygetsource)
+[![PyPI](https://img.shields.io/pypi/v/pygetsource?color=blue&style=flat-square)](https://pypi.org/project/pygetsource/)
+![Tests](https://img.shields.io/github/actions/workflow/status/percevalw/pygetsource/tests.yml?branch=main&label=tests&style=flat-square)
+[![Code style: black](https://img.shields.io/badge/code_style-black-black?style=flat-square)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 
 
 # pygetsource
 
-`pygetsource` is a Python decompiler, aiming to convert bytecode instructions back into Python code. This is useful when trying to recover the source code of a function from its bytecode instructions.
+`pygetsource` is a Python decompiler, aiming to convert compiled bytecode instructions back into Python code.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
 
 ```python
 a = 2
@@ -56,15 +58,17 @@
 STORE_FAST 0
 ```
 
 The latter form is typically stored in `.pyc` files and in the `__code__` attribute of function objects. The goal of `pygetsource` is to reverse this process.
 
 The project takes its name from the `inspect.getsource` function, which returns the source code of a function, but it is not always applicable, as explained above.
 
-`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+
+Finally, this software is distributed under the permissive MIT license.
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
 pip install pygetsource
@@ -93,34 +97,34 @@
 
 
 print(pygetsource.getsource(func.__code__))
 ```
 
 produces the following output:
 
-```
+```python
 a = 5
 while i < 10:
     if a == 2:
         break
     elif a == 4:
         return 3
     else:
         a = i // 5
 d = 3
 e = 4
 return e + d
 ```
 
-Notice how the `else` statement is added to the `elif` statement, yet the two programs are functionally equivalent.
+Notice how the `else` statement was added to the `elif` statement, yet the two programs are functionally equivalent.
 
 
 ## When is this useful ?
 
-`pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when a function is created through an eval statement or lambda syntax, since for the latter, Python versions earlier than 3.11 do not store the exact character offset of the function in the source code, making it hard to retrieve the lambda source code.
+`pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when you want to get the source code of a function created through an eval statement or a lambda syntax. Indeed, running `inspect.getsource` fail in the latter case since the origin file of the function is either not available, or Python does not provide the exact boundaries, which are required in the case of lambda functions.
 
 ## Alternatives
 
 [uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above.
 It is also licensed under a copyleft GPL license, making it less suitable for larger projects with permissive licenses.
 
 [decompyle++ (pycdc)](https://github.com/zrax/pycdc) uses a state machine approach to build an AST iteratively by processing bytecode instructions. It's written in C++ and supports more Python versions than uncompyle6, but has more trouble decompiling  complex control structures like nested loops, break patterns, comprehensions, or the example given above. It also uses the copyleft GPL license.
@@ -132,16 +136,14 @@
 In constrast with [uncompyle6](https://github.com/rocky/python-uncompyle6) and [pycdc](https://github.com/zrax/pycdc), `pygetsource` uses the `ast` and `astunparse` libraries to generate the source code from the generated AST.
 
 Here is an example of a graph being reduced:
 
 ![Graph reduction](./docs/graph-example.svg)
 
 
-Finally, this software is distributed under the permissive MIT license, making it ideal for use as a dependency in larger projects.
-
 ## When is a decompilation successful ?
 
 Since the compilation process is injective, it's impossible to recover the exact original source code. Multiple Python programs can yield the same bytecode instructions. Also, the original source code is typically unavailable for comparison (why would you use this software otherwise ?).
 
 If we recompile the generated program, we can compare the two sets of bytecode instructions to ensure functional equivalence. However, Python may introduce no-op codes (like 'NOP') that might cause this verification to fail despite the two code objects being functionally equivalent.
 
 Instead, `pygetsource` compares the graph of the original code object with the graph of the recovered code object, after a pruning step. During this step, no-op codes are removed, jump instructions are pruned (while maintaining edges between source and target nodes), and dead-code is eliminated.
```

### Comparing `pygetsource-0.1.0/README.md` & `pygetsource-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-<a href="https://github.com/psf/black/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
-<a href="https://pypi.org/project/pygetsource/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pygetsource"></a>
-<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+[![Codecov](https://img.shields.io/codecov/c/github/percevalw/pygetsource?logo=codecov&style=flat-square)](https://codecov.io/gh/percevalw/pygetsource)
+[![PyPI](https://img.shields.io/pypi/v/pygetsource?color=blue&style=flat-square)](https://pypi.org/project/pygetsource/)
+![Tests](https://img.shields.io/github/actions/workflow/status/percevalw/pygetsource/tests.yml?branch=main&label=tests&style=flat-square)
+[![Code style: black](https://img.shields.io/badge/code_style-black-black?style=flat-square)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 
 
 # pygetsource
 
-`pygetsource` is a Python decompiler, aiming to convert bytecode instructions back into Python code. This is useful when trying to recover the source code of a function from its bytecode instructions.
+`pygetsource` is a Python decompiler, aiming to convert compiled bytecode instructions back into Python code.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
 
 ```python
 a = 2
@@ -22,15 +24,17 @@
 STORE_FAST 0
 ```
 
 The latter form is typically stored in `.pyc` files and in the `__code__` attribute of function objects. The goal of `pygetsource` is to reverse this process.
 
 The project takes its name from the `inspect.getsource` function, which returns the source code of a function, but it is not always applicable, as explained above.
 
-`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+
+Finally, this software is distributed under the permissive MIT license.
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
 pip install pygetsource
@@ -59,34 +63,34 @@
 
 
 print(pygetsource.getsource(func.__code__))
 ```
 
 produces the following output:
 
-```
+```python
 a = 5
 while i < 10:
     if a == 2:
         break
     elif a == 4:
         return 3
     else:
         a = i // 5
 d = 3
 e = 4
 return e + d
 ```
 
-Notice how the `else` statement is added to the `elif` statement, yet the two programs are functionally equivalent.
+Notice how the `else` statement was added to the `elif` statement, yet the two programs are functionally equivalent.
 
 
 ## When is this useful ?
 
-`pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when a function is created through an eval statement or lambda syntax, since for the latter, Python versions earlier than 3.11 do not store the exact character offset of the function in the source code, making it hard to retrieve the lambda source code.
+`pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when you want to get the source code of a function created through an eval statement or a lambda syntax. Indeed, running `inspect.getsource` fail in the latter case since the origin file of the function is either not available, or Python does not provide the exact boundaries, which are required in the case of lambda functions.
 
 ## Alternatives
 
 [uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above.
 It is also licensed under a copyleft GPL license, making it less suitable for larger projects with permissive licenses.
 
 [decompyle++ (pycdc)](https://github.com/zrax/pycdc) uses a state machine approach to build an AST iteratively by processing bytecode instructions. It's written in C++ and supports more Python versions than uncompyle6, but has more trouble decompiling  complex control structures like nested loops, break patterns, comprehensions, or the example given above. It also uses the copyleft GPL license.
@@ -98,16 +102,14 @@
 In constrast with [uncompyle6](https://github.com/rocky/python-uncompyle6) and [pycdc](https://github.com/zrax/pycdc), `pygetsource` uses the `ast` and `astunparse` libraries to generate the source code from the generated AST.
 
 Here is an example of a graph being reduced:
 
 ![Graph reduction](./docs/graph-example.svg)
 
 
-Finally, this software is distributed under the permissive MIT license, making it ideal for use as a dependency in larger projects.
-
 ## When is a decompilation successful ?
 
 Since the compilation process is injective, it's impossible to recover the exact original source code. Multiple Python programs can yield the same bytecode instructions. Also, the original source code is typically unavailable for comparison (why would you use this software otherwise ?).
 
 If we recompile the generated program, we can compare the two sets of bytecode instructions to ensure functional equivalence. However, Python may introduce no-op codes (like 'NOP') that might cause this verification to fail despite the two code objects being functionally equivalent.
 
 Instead, `pygetsource` compares the graph of the original code object with the graph of the recovered code object, after a pruning step. During this step, no-op codes are removed, jump instructions are pruned (while maintaining edges between source and target nodes), and dead-code is eliminated.
```

### Comparing `pygetsource-0.1.0/pygetsource/ast_utils.py` & `pygetsource-0.1.1/pygetsource/ast_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import ast
 
-from astunparse.unparser import Unparser
-
 
 class Unpacking(ast.AST):
     _attributes = ()
     _fields = ("value",)
 
     def __init__(self, value, counter, starred=False):
         self.value = value
@@ -14,21 +12,14 @@
 
 
 class ForTargetPlaceholder(ast.AST):
     _attributes = ()
     _fields = ()
 
 
-def unparse_ForTargetPlaceholder(self, node):
-    self.write("[...]")
-
-
-Unparser._ForTargetPlaceholder = unparse_ForTargetPlaceholder
-
-
 class ExceptionMatch(ast.AST):
     _attributes = ()
     _fields = ("value",)
 
     def __init__(self, value):
         self.value = value
 
@@ -48,29 +39,18 @@
     _fields = ("value", "collection")
 
     def __init__(self, value, collection):
         self.collection = collection
         self.value = value
 
 
-def unparse_ComprehensionBody(self, node):
-    """Produced by LIST_APPEND or SET_ADD and unparsed as collection.append/add(value)"""
-    self.fill()
-    self.write("append/add(")
-    self.dispatch(node.value)
-    self.write(")")
-
-
-Unparser._ComprehensionBody = unparse_ComprehensionBody
-
-
 class RewriteComprehensionArgs(ast.NodeTransformer):
-    def __init__(self, args, cls):
+    def __init__(self, args):
         self.args = args
-        self.cls = cls
+        self.cls = None
 
     def visit_Name(self, node):
         if node.id.startswith("."):
             var_idx = int(node.id[1:])
             return self.args[var_idx]
         return node
 
@@ -103,35 +83,35 @@
         # if not isinstance(elt, ast.IfExp):
         #    raise Exception("Expected IfExp instead of " + ast.dump(elt))
         # TODO handle DictComp
         if self.cls and isinstance(elt, self.cls):
             generators = generators + elt.generators
             elt = elt.elt
         elif isinstance(elt, ComprehensionBody):
-            cls = {
+            self.cls = {
                 ast.List: ast.ListComp,
                 ast.Set: ast.SetComp,
                 ast.Dict: ast.DictComp,
             }[type(elt.collection)]
             elt = elt.value
         elif isinstance(elt, ast.Expr) and isinstance(elt.value, ast.Yield):
-            cls = ast.GeneratorExp
+            self.cls = ast.GeneratorExp
             elt = elt.value.value
         else:
-            raise Exception("Unexpected " + ast.dump(elt) + ", cls:" + str(cls))
+            raise Exception("Unexpected " + ast.dump(elt) + ", cls:" + str(self.cls))
 
-        if issubclass(cls, ast.DictComp):
+        if issubclass(self.cls, ast.DictComp):
             return ast.DictComp(
                 key=elt[0],
                 value=elt[1],
                 generators=generators,
                 ifs=[],
             )
         else:
-            return cls(
+            return self.cls(
                 elt=elt,
                 generators=generators,
                 ifs=[],
             )
 
 
 class RemoveLastContinue(ast.NodeTransformer):
```

### Comparing `pygetsource-0.1.0/pygetsource/decompiler.py` & `pygetsource-0.1.1/pygetsource/decompiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import ast
 import dis
-import io
 import sys
 import textwrap
 from types import CodeType
-from typing import List, Optional, Set, Tuple, Type
+from typing import List, Optional, Set, Tuple
 
-from astunparse.unparser import Unparser
 from IPython.display import display
 
-from .ast_utils import RemoveLastContinue
+from .ast_utils import (
+    ComprehensionBody,
+    ExceptionMatch,
+    ExceptionPlaceholder,
+    ForTargetPlaceholder,
+    RemoveLastContinue,
+    Reraise,
+    RewriteComprehensionArgs,
+    Unpacking,
+    WhileBreakFixer,
+)
 from .utils import (
     binop_to_ast,
     compareop_to_ast,
     get_origin,
     graph_sort,
     hasjabs,
     inplace_to_ast,
@@ -21,19 +29,17 @@
     unaryop_to_ast,
 )
 
 try:
     import ast as astunparse
 
     assert hasattr(astunparse, "unparse")
-    print("Using ast.unparse")
 except AssertionError:
     import astunparse
 
-INDENT = 0
 DEBUG = False
 DRAW_PROG = "dot"
 
 
 class set_debug:
     def __init__(self, value=True, prog="dot"):
         global DEBUG, DRAW_PROG
@@ -45,94 +51,25 @@
         pass
 
     def __exit__(self, *args):
         global DEBUG, DRAW_PROG
         DEBUG, DRAW_PROG = self.old
 
 
-def debug(*args, **kwargs):
-    if DEBUG:
-        buffer = io.StringIO()
-        print(*args, **kwargs, file=buffer)
-        print(textwrap.indent(buffer.getvalue(), "  " * INDENT), end="")
-
-
 def warn(*args):
-    # debug but in red
+    # print but in red
     print("\033[91m", *args, "\033[0m")
 
 
-class Unpacking(ast.AST):
-    _attributes = ()
-    _fields = ("value",)
-
-    def __init__(self, value, counter, starred=False):
-        self.value = value
-        self.counter = counter
-        self.starred = starred
-
-
-class ForTargetPlaceholder(ast.AST):
-    _attributes = ()
-    _fields = ()
-
-
-def unparse_ForTargetPlaceholder(self, node):
-    self.write("[...]")
-
-
-Unparser._ForTargetPlaceholder = unparse_ForTargetPlaceholder
-
-
-class ExceptionMatch(ast.AST):
-    _attributes = ()
-    _fields = ("value",)
-
-    def __init__(self, value):
-        self.value = value
-
-
-class ExceptionPlaceholder(ast.AST):
-    _attributes = ()
-    _fields = ()
-
-
-class Reraise(ast.AST):
-    _attributes = ()
-    _fields = ()
-
-
-class ComprehensionBody(ast.AST):
-    _attributes = ()
-    _fields = ("value", "collection")
-
-    def __init__(self, value, collection):
-        self.collection = collection
-        self.value = value
-
-
-def unparse_ComprehensionBody(self, node):
-    """Produced by LIST_APPEND or SET_ADD and unparsed as collection.append/add(value)"""
-    self.fill()
-    self.write("append/add(")
-    self.dispatch(node.value)
-    self.write(")")
-
-
-Unparser._ComprehensionBody = unparse_ComprehensionBody
-
-
 class Node:
     def __init__(self, code: CodeType, op_idx: int, offset: int, opname: str, arg: int):
         # Two choices when walking the graph, either go to the next node or
         # jump to a different node in case of a (un)conditional jump
         self.next: Optional[Node] = None
-        self.next_is_virtual: bool = False
         self.jumps: Set[Node] = set()
-        self.virtual = None
 
         # Previous nodes
         self.prev: Set[Node] = set()
 
         # The node's code
         self.code = code
         self.opname = opname
@@ -155,71 +92,50 @@
     def container(self):
         if self._container is not self:
             self._container = self._container.container
         return self._container
 
     def add_stmt(self, stmt):
         if DEBUG:
-            debug("Add stmt", self, ":", stmt)
+            print("Add stmt", self, ":", stmt)
         try:
             if DEBUG:
-                debug(
+                print(
                     textwrap.indent(
                         astunparse.unparse(ast.fix_missing_locations(stmt)), "  "
                     )
                 )
         except Exception:
             warn("Could not unparse", stmt, "in", self)
         self.stmts.append(stmt)
 
     def add_stack(self, item):
-        if self.stack is None:
-            self.stack = []
         if DEBUG:
-            debug("Add stack", self, ":", item)
+            print("Add stack", self, ":", item)
         self.stack.append(item)
 
     def pop_stack(self):
         return self.stack.pop()
 
     def contract_backward(self):
         """
         Merge the node with its predecessor
         """
 
         # If the node has a single predecessor, merge it with that node
 
         prev_node = next((n for n in self.prev if n.next is self), None)
-        if not self.prev:
-            self.loops = frozenset()
-        if not (
-            prev_node
-            and (
-                (len(self.prev) == 1)
-                or prev_node.opname in ("NOP",)  # and not prev_node.jumps) or
-            )
-        ):
-            if DEBUG:
-                debug(
-                    "Could not contract",
-                    prev_node,
-                    "!<<<!",
-                    self,
-                    "| next:",
-                    self.next,
-                    "jumps:",
-                    self.jumps,
-                    "| prev:",
-                    self.prev,
-                )
-            return None
+        assert prev_node and (
+            (len(self.prev) == 1)
+            or prev_node.opname in ("NOP",)  # and not prev_node.jumps) or
+        )
 
         prev_node._container = self._container
         if DEBUG:
-            debug(
+            print(
                 "Contract backward",
                 prev_node,
                 "<<<",
                 self,
                 "|",
                 self.next,
                 self.jumps,
@@ -244,15 +160,15 @@
                 continue
             if prev_node in succ.prev:
                 succ.prev.remove(prev_node)
                 succ.prev.add(self)
 
         self.stmts = prev_node.stmts + self.stmts
         if DEBUG:
-            debug("After contraction", self, "|", self.next, self.jumps, "|", self.prev)
+            print("After contraction", self, "|", self.next, self.jumps, "|", self.prev)
 
         return prev_node
 
     @classmethod
     def from_code(cls, code: CodeType, prune: bool = False):
         bytes = code.co_code
         offset = 0
@@ -308,54 +224,22 @@
                     block.jumps.add(graph[block.offset + arg + 2])
                 else:
                     block.jumps.add(graph[block.offset + arg])
             else:
                 if block.offset in graph:
                     block.next = graph[block.offset]
 
-            if (
-                # sys.version_info <= (3, 9)
-                block.offset in graph
-                and not block.next
-                and graph[block.offset] not in block.jumps
-                and not prune
-                and False
-            ):
-                block.next = graph[block.offset]
-                block.next_is_virtual = True
-
             if block.next:
                 block.next.prev.add(block)
             for jump in block.jumps:
                 jump.prev.add(block)
 
-            # block.is_virtual = True
-
         root = graph[0]
         root = rewire_break_loop(root)
 
-        if not prune:
-            prune_virtual_edges(root)
-        # seen = set()
-        # def unset_virtual(x):
-        #     if x in seen:
-        #         return
-        #     x.is_virtual = False
-        #     #for prev in tuple(x.prev):
-        #     #    if prev.next_is_virtual and prev.next is x:
-        #     #        prev.next = None
-        #     #        x.prev.remove(prev)
-        #     #        print("Removing prev from", x, ":", prev)
-        #     seen.add(x)
-        #     if not x.is_virtual:
-        #         for n in (x.next if not x.next_is_virtual else None, *x.jumps):
-        #             if n:
-        #                 unset_virtual(n)
-        # unset_virtual(graph[0])
-
         index = 0
         sorted_nodes = []
         for node in graph_sort(root):
             if (
                 node.opname == "NOP"
                 or node.opname == "RERAISE"
                 and node.arg == 0
@@ -426,35 +310,30 @@
             try:
                 source = node.to_source().split("\n")
             except Exception:
                 source = ["!ERROR!"]
             max_line = max(len(line) for line in source)
             label = "\n".join(
                 [
-                    ("~({})".format(node.virtual) if node.virtual else "")
-                    + f"[{node.op_idx}]{'✓' if node.visited else ''}|"
+                    f"[{node.op_idx}]{'✓' if node.visited else ''}|"
                     f"{len(node.stack) if node.stack else 0}☰|{len(node.prev)}↣",
                     # f"↺({','.join(str(i) for i in sorted(node.loops))})",
                     f"{node.opname}({node.arg_value})",
                     "------------",
                     *[line.ljust(max_line) for line in source],
                 ]
             )
             g.add_node(
                 node,
                 pos=",".join(map(str, pos)) + "!",
                 label=label,
                 fontsize=10,
                 color="red" if node is self else "black",
             )
-            # positions[node] = pos
-            if node.next and not node.next_is_virtual:
-                g.add_edge(node, node.next, label="next", fontsize=10)
-                rec(node.next, (pos[0], pos[1] + 1))
-            elif node.next:
+            if node.next:
                 g.add_edge(node, node.next, label="(next)", fontsize=10, style="dashed")
                 rec(node.next, (pos[0], pos[1] + 1))
 
             for jump in node.jumps:
                 g.add_edge(node, jump, label="jump", fontsize=10)
                 rec(jump, (pos[0], pos[1] + 1))
 
@@ -472,19 +351,20 @@
         return HTML(
             f'<div style="max-height: 100%; max-width: initial">{svg.decode()}</div>'
         )
 
     def to_source(self):
         res = []
         for stmt in self.stmts:
+            stmt = ast.fix_missing_locations(stmt)
             try:
-                stmt = ast.fix_missing_locations(stmt)
-            except AttributeError:
-                pass
-            res.append(astunparse.unparse(stmt).strip("\n"))
+                res.append(astunparse.unparse(stmt).strip("\n"))
+            except Exception:
+                raise ValueError("Could not unparse", ast.dump(stmt))
+
         return "\n".join(res)
 
     def last_stmts(self):
         if self.stmts:
             return self.stmts
         prev_visited = [n for n in self.prev if n.visited]
         if len(prev_visited) != 1:
@@ -505,36 +385,30 @@
         """
         root = node
 
         if node.visited or node in stop_nodes:
             return None
 
         while True:
-            if node.visited:
-                if DEBUG:
-                    debug("::: Already visited", node)
-                break
             if DEBUG:
-                debug(
+                print(
                     "::: Processing",
                     node,
                     "|",
                     node.next,
                     node.jumps,
                     "|",
                     node.prev,
                     "Ø",
                     loop_heads,
                 )
             node.visited = True
             prev_visited = [n for n in node.prev if n.visited]
             if len(prev_visited) > 1:
-                if DEBUG:
-                    debug("Too many prev visited", prev_visited, "for", node)
-                raise Exception("Too many prev visited")
+                raise Exception(f"Too many visited predecessors for {node}")
             if node.stack is None:
                 if prev_visited and prev_visited[0].stack is not None:
                     node.stack = list(prev_visited[0].stack)
                 else:
                     node.stack = []
 
             prev_unvisited = [n for n in node.prev if not n.visited]
@@ -567,35 +441,14 @@
                     if same_context:
                         node.add_stmt(ast.Continue(_loop_node=jump))
                     else:
                         node.add_stmt(ast.Break(_loop_node=jump))
                 else:
                     if not same_context:
                         node.add_stmt(ast.Break(_loop_node=jump))
-
-                if node.next and node.next_is_virtual:
-                    next_node = node.next
-                    print("NEXT VIRTUAL NODE", node, "->", next_node, next_node.virtual)
-                    if next_node.virtual:
-                        next_node = next_node._run(
-                            stop_nodes={*stop_nodes, *node.jumps},
-                            loop_heads=loop_heads,
-                            while_fusions=while_fusions,
-                        )
-                        if next_node is None:
-                            next_node = node.next
-                    print("...NEXT VIRTUAL NODE", node, "->", next_node)
-                    node.next = None
-                    next_node.prev.discard(node)
-                    node.stmts.extend(next_node.stmts)
-                    for succ in (next_node.next, *next_node.jumps):
-                        if succ and next_node in succ.prev:
-                            succ.prev.discard(next_node)
-                            succ.prev.add(node)
-                    node.jumps |= {next_node.next, *next_node.jumps} - {None}
             elif node.opname in (
                 "POP_JUMP_IF_TRUE",
                 "POP_JUMP_IF_FALSE",
                 "JUMP_IF_NOT_EXC_MATCH",
             ):
                 if node.opname == "JUMP_IF_NOT_EXC_MATCH":
                     test = ExceptionMatch(node.pop_stack())
@@ -609,15 +462,15 @@
 
                 old_if_node = if_node
 
                 ################
                 # SPECIAL CASE #
                 ################
                 if DEBUG:
-                    debug(
+                    print(
                         "IF/ELSE BLOCK",
                         node,
                         "LOOP HEADS",
                         loop_heads,
                         "IF",
                         if_node,
                         "ELSE",
@@ -642,15 +495,15 @@
                         else "POP_JUMP_IF_TRUE"
                     )
                     and ast.dump(real_branch.jump_test) == ast.dump(test)
                 ):
                     real_head = get_origin(real_branch.jump_test)[0].container
 
                     if DEBUG:
-                        debug("THIS SHOULD BE A CONDITIONAL WHILE LOOP", ast.dump(test))
+                        print("THIS SHOULD BE A CONDITIONAL WHILE LOOP", ast.dump(test))
                     # node.add_stmt(ast.Continue())
                     node.next.prev.discard(node)
                     node.next = None
                     node.jumps = {real_head}
                     node.add_stmt(ast.Continue())
                     else_node.prev.remove(node)
                     real_head.prev.add(node)
@@ -663,15 +516,15 @@
                 else:
                     meet_nodes = lowest_common_successors(
                         if_node,
                         else_node,
                         stop_nodes={*stop_nodes, node},
                     )
                     if DEBUG:
-                        debug(
+                        print(
                             "IF/ELSE BLOCK",
                             node,
                             "MEET",
                             meet_nodes,
                             "(STOP at",
                             {*stop_nodes, node},
                             ")",
@@ -693,17 +546,17 @@
                     )
                     else_node = else_node._run(
                         stop_nodes={*stop_nodes, *meet_nodes, node},
                         loop_heads=loop_heads,
                         while_fusions=while_fusions,
                     )
                     if DEBUG:
-                        debug("IF/ELSE", node, "MEET", meet_nodes)
+                        print("IF/ELSE", node, "MEET", meet_nodes)
                     if DEBUG:
-                        debug(
+                        print(
                             "IF/ELSE",
                             node,
                             "BEFORE succ",
                             before,
                             "-> AFTER succ",
                             if_node,
                             else_node,
@@ -720,42 +573,27 @@
                         else_node.pop_stack()
                         if else_node and len(else_node.stack) > len(node.stack)
                         else None
                     )
 
                     test_origin = get_origin(test)[0].container
                     has_been_unparsed = False
-                    if DEBUG:
-                        debug(
-                            "IS THIS A WHILE X LOOP ?",
-                            node,
-                            "LH",
-                            loop_heads,
-                            "IF NEXT",
-                            (if_node or old_if_node).next,
-                            "IF LOOP HEAD",
-                            if_loop_head,
-                            "TEST",
-                            test_origin,
-                            "ELSE LOOP HEAD",
-                            else_loop_head,
-                        )
                     was_a_loop = False
                     if (
                         loop_heads
                         and if_loop_head is loop_heads[-1]
                         and test_origin is if_loop_head
                         and (
                             (if_node or old_if_node).next is if_loop_head
                             or old_if_node.next is if_loop_head
                         )
                         and else_loop_head is not loop_heads[-1]
                     ) or node.is_conditional_while:
                         if DEBUG:
-                            debug(
+                            print(
                                 "THIS IS A WHILE X LOOP",
                                 node,
                                 "LOOP HEAD",
                                 if_loop_head,
                             )
                         # while node.contract_backward():
                         #     print("NODE IS CONTRACTED", node, "==?", if_node.next)
@@ -864,28 +702,28 @@
                     discarded_successors = {
                         n
                         for n in (if_node, else_node)
                         + ((test_origin,) if was_a_loop else ())
                         if n and n.visited
                     }
                     if DEBUG:
-                        debug(
+                        print(
                             "IF/ELSE SUCC BEFORE CONTRACT",
                             successors,
                             "-",
                             discarded_successors,
                         )
                     if DEBUG:
-                        debug("IF/ELSE PREV BEFORE CONTRACT", node.prev)
+                        print("IF/ELSE PREV BEFORE CONTRACT", node.prev)
                     successors = successors - discarded_successors
 
                     jump_nodes = successors
                     for succ in successors:
                         if DEBUG:
-                            debug(
+                            print(
                                 "IF/ELSE",
                                 node,
                                 ": REBINDING SUCCESSOR",
                                 succ,
                                 "=>",
                                 succ.prev,
                                 "->",
@@ -900,19 +738,19 @@
                                 node if j in discarded_successors else j
                                 for j in p.jumps
                             }
                         n.prev = n.prev - discarded_successors
                     node.next = None
                     node.jumps = jump_nodes
                     if DEBUG:
-                        debug("IF/ELSE", node, node.stack)
+                        print("IF/ELSE", node, node.stack)
                     if DEBUG:
-                        debug("IF/ELSE SUCC AFTER CONTRACT", successors)
+                        print("IF/ELSE SUCC AFTER CONTRACT", successors)
                     if DEBUG:
-                        debug(
+                        print(
                             "IF/ELSE PREV AFTER CONTRACT",
                             node.prev,
                             "prevs successor:",
                             [(n.next, *n.jumps) for n in node.prev],
                         )
 
                     if DEBUG:
@@ -950,17 +788,17 @@
                     loop_heads=loop_heads,
                     while_fusions=while_fusions,
                 )
                 body_loop_head = explore_until(
                     body_node, (node, jump_node, *stop_nodes)
                 )
                 if DEBUG:
-                    debug("FOR LOOP HEAD", body_loop_head)
+                    print("FOR LOOP HEAD", body_loop_head)
                 if DEBUG:
-                    debug("BODY", [ast.dump(x) for x in body_node.stmts])
+                    print("BODY", [ast.dump(x) for x in body_node.stmts])
                 target = body_node.stmts.pop(0).targets[0]
 
                 body_stmts = (body_node.stmts if body_node else []) + (
                     [ast.Break()] if body_loop_head is not node else []
                 )
                 node.add_stmt(
                     ast.For(
@@ -972,17 +810,17 @@
                     )
                 )
                 successors = {body_node.next, *body_node.jumps, *node.jumps} - {None}
                 discarded_successors = {
                     n for n in (body_node, old_body_node, node) if n and n.visited
                 }
                 if DEBUG:
-                    debug("FOR SUCC", successors, "-", discarded_successors)
+                    print("FOR SUCC", successors, "-", discarded_successors)
                 if DEBUG:
-                    debug("FOR PREV", node.prev)
+                    print("FOR PREV", node.prev)
                 successors = successors - discarded_successors
                 jump_nodes = successors
                 for succ in successors:
                     succ.prev = (succ.prev - discarded_successors) | {node}
                 for n in discarded_successors:
                     for p in n.prev:
                         if p.next in discarded_successors:
@@ -1081,40 +919,82 @@
             elif node.opname == "LIST_TO_TUPLE":
                 value = node.pop_stack()
                 node.add_stack(ast.Tuple(value.elts))
             elif node.opname == "UNPACK_SEQUENCE":
                 value = node.pop_stack()
                 for i in reversed(range(node.arg)):
                     node.add_stack(Unpacking(value, counter=i))
+            elif node.opname in (
+                "BUILD_LIST_UNPACK",
+                "BUILD_SET_UNPACK",
+                "BUILD_TUPLE_UNPACK",
+                "BUILD_TUPLE_UNPACK_WITH_CALL",
+            ):
+                values = []
+                for _ in range(node.arg):
+                    value = node.pop_stack()
+                    if isinstance(value, ast.Constant):
+                        value = [ast.Constant(x, kind=None) for x in value.value]
+                    elif hasattr(value, "elts"):
+                        value = value.elts
+                    else:
+                        value = [ast.Starred(value)]
+                    values.append(value)
+                if node.opname == "BUILD_LIST_UNPACK":
+                    node.add_stack(ast.List(values[::-1]))
+                elif node.opname == "BUILD_SET_UNPACK":
+                    node.add_stack(ast.Set(values[::-1]))
+                else:
+                    node.add_stack(ast.Tuple(values[::-1]))
+            elif node.opname in ("BUILD_MAP_UNPACK", "BUILD_MAP_UNPACK_WITH_CALL"):
+                unpacked = []
+                for _ in range(node.arg):
+                    value = node.pop_stack()
+                    if isinstance(value, ast.Dict) and all(
+                        key.value is not None
+                        and isinstance(key.value, str)
+                        and key.value.isidentifier()
+                        for key in value.keys
+                        if key is not None and isinstance(key, ast.Constant)
+                    ):
+                        # check for valid python keywords identifiers
+                        unpacked.extend(zip(value.keys, value.values))
+                    else:
+                        unpacked.extend([(None, value)])
+                unpacked = unpacked[::-1]
+                keys = [k for k, v in unpacked]
+                values = [v for k, v in unpacked]
+                node.add_stack(ast.Dict(keys, values))
             elif node.opname == "UNPACK_EX":
                 # FROM Python's doc:
                 # The low byte of counts is the number of values before the list value,
                 # the high byte of counts the number of values after it. The resulting
                 # values are put onto the stack right-to-left.
                 value = node.pop_stack()
                 before, after = node.arg & 0xFF, node.arg >> 8
 
                 for i in reversed(range(before + after + 1)):
                     node.add_stack(Unpacking(value, counter=i, starred=i == before))
             elif node.opname in ("LIST_EXTEND", "SET_UPDATE"):
                 items = node.pop_stack()
                 if isinstance(items, ast.Constant):
-                    items = [ast.Constant(x) for x in items.value]
+                    items = [ast.Constant(x, kind=None) for x in items.value]
                 elif hasattr(items, "elts"):
                     items = items.elts
                 else:
                     items = [ast.Starred(items)]
                 obj = node.stack[-node.arg]
                 obj = type(obj)(elts=[*obj.elts, *items])
                 node.stack[-node.arg] = obj
             elif node.opname in ("DICT_UPDATE", "DICT_MERGE"):
                 items = node.pop_stack()
                 if isinstance(items, ast.Constant):
                     items = [
-                        (ast.Name(n), ast.Constant(v)) for n, v in items.value.items()
+                        (ast.Name(n), ast.Constant(v, kind=None))
+                        for n, v in items.value.items()
                     ]
                 # elif hasattr(items, 'keys'):
                 #    items = [(k, v) for k, v in zip(items.keys, items.values)]
                 else:
                     items = [(None, items)]
                 obj = node.stack[-node.arg]
                 assert isinstance(obj, ast.Dict)
@@ -1136,14 +1016,19 @@
                 else:
                     assert hasattr(collection, "elts")
                     collection = type(collection)(elts=[*collection.elts, value])
                     node.stack[-node.arg] = collection
             elif node.opname == "MAP_ADD":
                 value = node.pop_stack()
                 key = node.pop_stack()
+                # From https://docs.python.org/3.10/library/dis.html#opcode-MAP_ADD
+                # Changed in version 3.8: Map value is TOS and map key is TOS1.
+                # Before, those were reversed.
+                if sys.version_info < (3, 8):
+                    key, value = value, key
                 collection = node.stack[-node.arg]
                 # if we can loop to the collection beginning
                 if (
                     loop_heads
                     and explore_until(node, {*loop_heads, collection}) is loop_heads[-1]
                 ):
                     node.add_stmt(ComprehensionBody((key, value), collection))
@@ -1190,87 +1075,16 @@
                     )
                 )
             elif node.opname in ("CALL_FUNCTION", "CALL_METHOD"):
                 args = [node.pop_stack() for _ in range(node.arg)][::-1]
                 func = node.pop_stack()
                 if isinstance(func, ast.FunctionDef):
 
-                    class RewriteComprehensionArgs(ast.NodeTransformer):
-                        def visit_Name(self, node):
-                            if node.id.startswith("."):
-                                var_idx = int(node.id[1:])
-                                return args[var_idx]
-                            return node
-
-                        def visit_For(self, node: ast.For):
-                            nonlocal cls
-                            assert (
-                                len(node.body) == 1
-                                or len(node.body) == 2
-                                and isinstance(node.body[1], ast.Continue)
-                            )
-                            target = self.visit(node.target)
-                            elt = self.visit(node.body[0])
-                            iter = self.visit(node.iter)
-                            condition = None
-                            if isinstance(elt, ast.If):
-                                condition = elt.test
-                                assert (
-                                    len(elt.body) == 1
-                                    or len(elt.body) == 2
-                                    and isinstance(elt.body[1], ast.Continue)
-                                )
-                                elt = elt.body[0]
-                            generators = [
-                                ast.comprehension(
-                                    target=target,
-                                    iter=iter,
-                                    ifs=[condition]
-                                    if condition is not None
-                                    else [],  # TODO
-                                    is_async=False,  # TODO
-                                )
-                            ]
-                            if cls and isinstance(elt, cls):
-                                generators = generators + elt.generators
-                                elt = elt.elt
-                            elif isinstance(elt, ComprehensionBody):
-                                cls = {
-                                    ast.List: ast.ListComp,
-                                    ast.Set: ast.SetComp,
-                                    ast.Dict: ast.DictComp,
-                                }[type(elt.collection)]
-                                elt = elt.value
-                            elif isinstance(elt, ast.Expr) and isinstance(
-                                elt.value, ast.Yield
-                            ):
-                                cls = ast.GeneratorExp
-                                elt = elt.value.value
-                            else:
-                                raise Exception(
-                                    "Unexpected " + ast.dump(elt) + ", cls:" + str(cls)
-                                )
-
-                            if issubclass(cls, ast.DictComp):
-                                return ast.DictComp(
-                                    key=elt[0],
-                                    value=elt[1],
-                                    generators=generators,
-                                    ifs=[],
-                                )
-                            else:
-                                return cls(
-                                    elt=elt,
-                                    generators=generators,
-                                    ifs=[],
-                                )
-
                     assert len(func.body) == 2
-                    cls: Optional[Type[ast.AST]] = None
-                    tree = RewriteComprehensionArgs().visit(func)
+                    tree = RewriteComprehensionArgs(args=args).visit(func)
 
                     if len(func.body) == 1 or isinstance(func.body[1], ast.Return):
                         tree = func.body[0]
                     node.add_stack(tree)
                 else:
                     node.add_stack(
                         ast.Call(
@@ -1291,20 +1105,16 @@
                         keywords=[
                             ast.keyword(arg=key, value=value)
                             for key, value in zip(keys, values)
                         ],
                     ),
                 )
             elif node.opname == "CALL_FUNCTION_EX":
-                if node.arg & 0x01:
-                    kwargs = node.pop_stack()
-                    args = node.pop_stack()
-                else:
-                    kwargs = None
-                    args = node.pop_stack()
+                kwargs = node.pop_stack() if node.arg & 0x01 else None
+                args = node.pop_stack()
                 func = node.pop_stack()
                 if isinstance(kwargs, ast.Dict):
                     keywords = [
                         ast.keyword(
                             arg=key.value if key is not None else None, value=value
                         )
                         for key, value in zip(kwargs.keys, kwargs.values)
@@ -1312,24 +1122,22 @@
                 else:
                     keywords = [ast.keyword(arg=None, value=kwargs)]
                 if hasattr(args, "elts"):
                     args = args.elts
                 elif isinstance(args, ast.Constant) and isinstance(
                     args.value, (tuple, list)
                 ):
-                    args = [ast.Constant(value=elt, kind=True) for elt in args.value]
+                    args = [ast.Constant(value=elt, kind=None) for elt in args.value]
                 node.add_stack(
                     ast.Call(
                         func=func,
                         args=args,
                         keywords=keywords,
                     ),
                 )
-            elif node.opname == "NOP":
-                pass
             elif node.opname == "DUP_TOP":
                 node.add_stack(node.stack[-1])
             elif node.opname == "ROT_TWO":
                 s = node.stack
                 s[-1], s[-2] = s[-2], s[-1]
             elif node.opname == "ROT_THREE":
                 s = node.stack
@@ -1383,45 +1191,33 @@
                 # of generator or coroutine. The legal kinds are 0 for generator, 1 f
                 # or coroutine, and 2 for async generator."
                 # However, there are no item in the stack (from the bytecode
                 # perspective) at the start of a generator comprehension function
                 # if node.index > 0:
                 #    node.pop_stack()
                 pass
-            elif node.opname == "SETUP_LOOP":
-                # Python 3.7
-                raise Exception(
-                    "SETUP_LOOP code should have been removed during the "
-                    "graph initialization"
-                )
-            elif node.opname == "BREAK_LOOP":
-                # Python 3.7
-                raise Exception(
-                    "BREAK_LOOP code should have been removed during the "
-                    "graph initialization"
-                )
             else:
                 raise NotImplementedError(node.opname)
 
             # Handle while loops by detecting cycles of length 1
             prev_visited = [n for n in node.prev if n.visited]
             if DEBUG:
-                debug(
+                print(
                     "STACKS",
                     "node",
                     node,
                     len(node.stack),
                     node.stack,
                     "prev",
                     prev_visited,
                     len(prev_visited[-1].stack) if prev_visited else 0,
                     prev_visited[-1].stack if prev_visited else None,
                 )
             if DEBUG:
-                debug("LOOP HEADS", "node", node, "PREV", node.prev, "=>", loop_heads)
+                print("LOOP HEADS", "node", node, "PREV", node.prev, "=>", loop_heads)
             while not prev_visited or len(node.stack) <= len(prev_visited[-1].stack):
                 if root.container is not node:
                     prev = node.contract_backward()
                 else:
                     prev = None
                 if not prev and not node.prev == {node}:
                     break
@@ -1447,53 +1243,53 @@
                     prev_unvisited = [n for n in node.prev if not n.visited]
                     if len(prev_unvisited):
                         loop_heads = (*loop_heads, node)
                 prev_visited = [n for n in node.prev if n.visited]
                 if DEBUG:
                     display(node.draw())
                 if DEBUG:
-                    debug(
+                    print(
                         "STACKS",
                         "node",
                         node,
                         len(node.stack),
                         "prev",
                         prev_visited,
                         len(prev_visited[-1].stack) if prev_visited else 0,
                     )
 
             if DEBUG:
                 display(node.draw())
 
             if DEBUG:
-                debug("::: done", node, "|", node.next, node.jumps, "|", node.prev)
+                print("::: done", node, "|", node.next, node.jumps, "|", node.prev)
 
             if not node.next and not stop_on_jump:
                 if loop_heads:
                     jump_to_head = {
                         n: explore_until(n, (*loop_heads, *stop_nodes))
                         for n in node.jumps
                     }
                     if DEBUG:
-                        debug(
+                        print(
                             "CANDIDATE JUMPS",
                             node,
                             "=>",
                             jump_to_head,
                             "LOOP HEADS",
                             loop_heads,
                         )
                     same_level_jumps = [
                         jump
                         for jump, head in jump_to_head.items()
                         if head is loop_heads[-1]
                         or (head is None and len(jump.prev) == 1)
                     ]
                     if DEBUG:
-                        debug(
+                        print(
                             "SAME LEVEL JUMPS",
                             node,
                             "=>",
                             same_level_jumps,
                             "LOOP HEADS",
                             loop_heads,
                         )
@@ -1543,25 +1339,16 @@
 
         return node
 
     def run(self) -> "Node":
         """Decompile a code object"""
         while_fusions = {}
         node = self._run(while_fusions=while_fusions)
-
-        class WhileBreakFixer(ast.NodeTransformer):
-            def visit_Break(self, node):
-                if hasattr(node, "_loop_node") and node._loop_node in while_fusions:
-                    if DEBUG:
-                        debug("NODE BREAK", node, node._loop_node)
-                    return ast.Continue()
-                return node
-
         node.stmts = [
-            WhileBreakFixer().visit(RemoveLastContinue().visit(stmt))
+            WhileBreakFixer(while_fusions).visit(RemoveLastContinue().visit(stmt))
             for stmt in node.stmts
         ]
 
         return node
 
 
 def getsource(code: CodeType, debug: bool = False) -> str:
@@ -1727,25 +1514,25 @@
         try:
             is_multi_assignment = (
                 len(last_stmts)
                 and isinstance(last_stmts[-1], ast.Assign)
                 and get_origin(value)[1] <= get_origin(last_stmts[-1].targets)[1]
             )
             if DEBUG:
-                debug(
+                print(
                     f"ORIGIN of {ast.dump(value)}",
                     get_origin(value)[1],
                     f"vs ORIGIN of last {ast.dump(last_stmts[-1])}",
                     get_origin(last_stmts[-1].targets)[1],
                 )
         except Exception:
             is_multi_assignment = False
 
         if DEBUG:
-            debug(
+            print(
                 "VALUE",
                 value,
                 "LAST",
                 last_stmts,
                 "MULTI",
                 multi_targets,
                 "UNPACKING",
@@ -1815,15 +1602,15 @@
         lowest_common_successors(
             next_node,
             jump_node,
             stop_nodes={*stop_nodes, node},
         )
     )
     if DEBUG:
-        debug(
+        print(
             "TRY BLOCK", node, "MEET", meet_nodes, "(STOP at", {*stop_nodes, node}, ")"
         )
     assert len(meet_nodes) <= 1
 
     before = (next_node, jump_node)
     next_node = next_node._run(
         stop_nodes={*stop_nodes, *meet_nodes, node},
@@ -1851,17 +1638,17 @@
             stop_on_jump=True,
         )
         finally_node.prev = old_prev
     else:
         finally_node = old_finally_node = None
 
     if DEBUG:
-        debug("TRY", node, "MEET", meet_nodes)
+        print("TRY", node, "MEET", meet_nodes)
     if DEBUG:
-        debug("TRY", node, "BEFORE succ", before, "-> AFTER succ", next_node, jump_node)
+        print("TRY", node, "BEFORE succ", before, "-> AFTER succ", next_node, jump_node)
 
     handlers = []
     finalbody = []
     if (
         jump_node.stmts
         and isinstance(jump_node.stmts[0], ast.If)
         and isinstance(jump_node.stmts[0].test, ExceptionMatch)
@@ -1939,23 +1726,23 @@
             old_jump_node,
             finally_node,
             old_finally_node,
         )
         if n and n.visited
     }
     if DEBUG:
-        debug("TRY SUCC", successors, "-", discarded_successors)
+        print("TRY SUCC", successors, "-", discarded_successors)
     if DEBUG:
-        debug("TRY PREV", node.prev)
+        print("TRY PREV", node.prev)
     successors = successors - discarded_successors
 
     jump_nodes = successors
     for succ in successors:
         if DEBUG:
-            debug(
+            print(
                 "TRY",
                 node,
                 ": REBINDING SUCCESSOR",
                 succ,
                 "=>",
                 succ.prev,
                 "->",
@@ -1967,64 +1754,20 @@
             if p.next in discarded_successors:
                 p.next = node
             p.jumps = {node if j in discarded_successors else j for j in p.jumps}
         n.prev = n.prev - discarded_successors
     node.next = None
     node.jumps = jump_nodes
     if DEBUG:
-        debug("TRY", node, node.stack)
+        print("TRY", node, node.stack)
 
     if DEBUG:
         display(node.draw())
 
 
-def prune_virtual_edges(root):
-    queue = [(root, 0)]
-    graph = set()
-
-    while queue:
-        node, level = queue.pop(0)
-        graph.add(node)
-
-        if node.virtual is None:
-            node.virtual = level
-        else:
-            new_level = min(node.virtual, level)
-            if new_level == node.virtual:
-                continue
-            node.virtual = new_level
-        if node.next and node.next_is_virtual:
-            queue.append((node.next, level + 1))
-        elif node.next:
-            queue.append((node.next, level))
-        for succ in node.jumps:
-            queue.append((succ, level))
-
-    for node in graph:
-        for prev in tuple(node.prev):
-            if (
-                prev.virtual
-                and node.virtual
-                and prev.virtual > node.virtual
-                and prev.next is node
-            ):
-                node.prev.discard(prev)
-                prev.next = None
-            if (
-                prev.virtual
-                and node.virtual
-                and prev.virtual
-                and prev.virtual == node.virtual
-                and prev.next_is_virtual
-                and prev.next is node
-            ):
-                node.prev.discard(prev)
-                prev.next = None
-
-
 def contract_jumps(root):
     queue = [root]
     seen = set()
 
     while queue:
         node = queue.pop(0)
 
@@ -2061,15 +1804,14 @@
             # jump_node = next(iter(node.jumps))
             jump_node = node.jumps.pop()
             jump_node.prev.discard(node)
             queue.append((node.next, [*loop_jumps, jump_node]))
             queue.append((jump_node, loop_jumps))
         elif node.opname == "BREAK_LOOP":
             node.opname = "JUMP_ABSOLUTE"
-            # node.next_is_virtual = True
             if node.next:
                 node.next.prev.discard(node)
                 node.next = None
             node.arg = None
             loop_jumps[-1].prev.add(node)
             node.jumps = {loop_jumps[-1]}
             queue.append((node.next, loop_jumps))
```

### Comparing `pygetsource-0.1.0/pygetsource/factory.py` & `pygetsource-0.1.1/pygetsource/factory.py`

 * *Files identical despite different names*

### Comparing `pygetsource-0.1.0/pygetsource/utils.py` & `pygetsource-0.1.1/pygetsource/utils.py`

 * *Files identical despite different names*

### Comparing `pygetsource-0.1.0/pygetsource.egg-info/PKG-INFO` & `pygetsource-0.1.1/pygetsource.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygetsource
-Version: 0.1.0
+Version: 0.1.1
 Summary: Decompiler written in Python for Python
 Author-email: Perceval Wajsburt <perceval.wajsburt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Perceval Wajsburt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,22 +28,24 @@
 Project-URL: homepage, https://github.com/perceval/pygetsource/
 Project-URL: repository, https://github.com/perceval/pygetsource/
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-<a href="https://github.com/psf/black/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
-<a href="https://pypi.org/project/pygetsource/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pygetsource"></a>
-<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+[![Codecov](https://img.shields.io/codecov/c/github/percevalw/pygetsource?logo=codecov&style=flat-square)](https://codecov.io/gh/percevalw/pygetsource)
+[![PyPI](https://img.shields.io/pypi/v/pygetsource?color=blue&style=flat-square)](https://pypi.org/project/pygetsource/)
+![Tests](https://img.shields.io/github/actions/workflow/status/percevalw/pygetsource/tests.yml?branch=main&label=tests&style=flat-square)
+[![Code style: black](https://img.shields.io/badge/code_style-black-black?style=flat-square)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 
 
 # pygetsource
 
-`pygetsource` is a Python decompiler, aiming to convert bytecode instructions back into Python code. This is useful when trying to recover the source code of a function from its bytecode instructions.
+`pygetsource` is a Python decompiler, aiming to convert compiled bytecode instructions back into Python code.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
 
 ```python
 a = 2
@@ -56,15 +58,17 @@
 STORE_FAST 0
 ```
 
 The latter form is typically stored in `.pyc` files and in the `__code__` attribute of function objects. The goal of `pygetsource` is to reverse this process.
 
 The project takes its name from the `inspect.getsource` function, which returns the source code of a function, but it is not always applicable, as explained above.
 
-`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+
+Finally, this software is distributed under the permissive MIT license.
 
 ## Installation
 
 Install the package using pip:
 
 ```bash
 pip install pygetsource
@@ -93,34 +97,34 @@
 
 
 print(pygetsource.getsource(func.__code__))
 ```
 
 produces the following output:
 
-```
+```python
 a = 5
 while i < 10:
     if a == 2:
         break
     elif a == 4:
         return 3
     else:
         a = i // 5
 d = 3
 e = 4
 return e + d
 ```
 
-Notice how the `else` statement is added to the `elif` statement, yet the two programs are functionally equivalent.
+Notice how the `else` statement was added to the `elif` statement, yet the two programs are functionally equivalent.
 
 
 ## When is this useful ?
 
-`pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when a function is created through an eval statement or lambda syntax, since for the latter, Python versions earlier than 3.11 do not store the exact character offset of the function in the source code, making it hard to retrieve the lambda source code.
+`pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when you want to get the source code of a function created through an eval statement or a lambda syntax. Indeed, running `inspect.getsource` fail in the latter case since the origin file of the function is either not available, or Python does not provide the exact boundaries, which are required in the case of lambda functions.
 
 ## Alternatives
 
 [uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above.
 It is also licensed under a copyleft GPL license, making it less suitable for larger projects with permissive licenses.
 
 [decompyle++ (pycdc)](https://github.com/zrax/pycdc) uses a state machine approach to build an AST iteratively by processing bytecode instructions. It's written in C++ and supports more Python versions than uncompyle6, but has more trouble decompiling  complex control structures like nested loops, break patterns, comprehensions, or the example given above. It also uses the copyleft GPL license.
@@ -132,16 +136,14 @@
 In constrast with [uncompyle6](https://github.com/rocky/python-uncompyle6) and [pycdc](https://github.com/zrax/pycdc), `pygetsource` uses the `ast` and `astunparse` libraries to generate the source code from the generated AST.
 
 Here is an example of a graph being reduced:
 
 ![Graph reduction](./docs/graph-example.svg)
 
 
-Finally, this software is distributed under the permissive MIT license, making it ideal for use as a dependency in larger projects.
-
 ## When is a decompilation successful ?
 
 Since the compilation process is injective, it's impossible to recover the exact original source code. Multiple Python programs can yield the same bytecode instructions. Also, the original source code is typically unavailable for comparison (why would you use this software otherwise ?).
 
 If we recompile the generated program, we can compare the two sets of bytecode instructions to ensure functional equivalence. However, Python may introduce no-op codes (like 'NOP') that might cause this verification to fail despite the two code objects being functionally equivalent.
 
 Instead, `pygetsource` compares the graph of the original code object with the graph of the recovered code object, after a pruning step. During this step, no-op codes are removed, jump instructions are pruned (while maintaining edges between source and target nodes), and dead-code is eliminated.
```

### Comparing `pygetsource-0.1.0/pyproject.toml` & `pygetsource-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -18,33 +18,43 @@
 where = ["."]
 include = ["pygetsource*"]
 namespaces = false
 
 # ----- Development configuration -----
 [project.optional-dependencies]
 dev = [
-    "pytest>=7.1.0,<8.0.0",
-    "pytest-cov>=3.0.0,<5.0.0",
-    "networkx>=3.1,<4.0",
-    "pygraphviz>=1.11,<2.0",
+    "pytest",
+    "pytest-cov",
+    "coverage[toml]>=7.2.0",
+    "networkx>=2.0.0,<4.0",
+    "pygraphviz>=1.7,<2.0",
+    "ipython>=6.0.0,<8.0.0",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "pygetsource.__version__" }
 
 # ----- Tests -----
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.coverage.report]
 exclude_also = [
-    "raise UnknownException"
-]
+    "def __repr__",
+    "raise NotImplementedError",
+    "raise .*Error",
+    "raise .*Exception",
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
+    "if DEBUG:",
+    "class .*\\bProtocol\\):",
+    "@(abc\\.)?abstractmethod",
+    ]
 
 # ----- Documentation -----
 [tool.interrogate]
 ignore-init-method = false
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = true
```

### Comparing `pygetsource-0.1.0/tests/test_py37.py` & `pygetsource-0.1.1/tests/test_py37.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-
 import pytest as pytest
 from utils import make_test_idem
 
 
 @make_test_idem
 def test_assign():
     a = 1
@@ -698,14 +696,15 @@
 def test_iter():
     for x in iter(a):
         pass
 
     [s2 for s1 in qs.split("&") for s2 in s1.split(";")]
 
 
+@pytest.mark.xfail(reason="try/except not implemented yet")
 @make_test_idem
 def test_empty_try():
     try:
         pass
     except:
         pass
 
@@ -748,17 +747,14 @@
                     break
                 return
             return
         else:
             x = 2
 
 
-@pytest.mark.xfail(
-    sys.version_info >= (3, 9), reason="behavior is the same but bytecode differs"
-)
 @make_test_idem
 def test_while_if_while_if_break_return():
     while True:
         if x:
             while True:
                 if x:
                     break
@@ -805,30 +801,25 @@
 def test_while_only_break():
     a = 1
     while x:
         break
     return None
 
 
-@pytest.mark.xfail(
-    sys.version_info >= (3, 9), reason="behavior is the same but bytecode differs"
-)
+@pytest.mark.xfail(reason="dead code changes the variable from local to free")
 @make_test_idem
 def test_while_true_if_if_continue_assign():
     while True:
         if x:
             if y:
                 continue
                 x = 1
     return z
 
 
-@pytest.mark.xfail(
-    sys.version_info >= (3, 9), reason="behavior is the same but bytecode differs"
-)
 @make_test_idem
 def test_while_true_if_if_continue():
     while True:
         if x:
             if y:
                 continue
         return line
```

### Comparing `pygetsource-0.1.0/tests/test_rebuild.py` & `pygetsource-0.1.1/tests/test_rebuild.py`

 * *Files identical despite different names*

