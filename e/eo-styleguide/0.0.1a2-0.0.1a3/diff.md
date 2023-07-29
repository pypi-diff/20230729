# Comparing `tmp/eo_styleguide-0.0.1a2.tar.gz` & `tmp/eo_styleguide-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo_styleguide-0.0.1a2.tar", max compression
+gzip compressed data, was "eo_styleguide-0.0.1a3.tar", max compression
```

## Comparing `eo_styleguide-0.0.1a2.tar` & `eo_styleguide-0.0.1a3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0     3096 2023-07-23 14:12:32.395350 eo_styleguide-0.0.1a2/README.md
--rw-r--r--   0        0        0     1237 2023-07-23 13:29:32.045996 eo_styleguide-0.0.1a2/pyeo/__init__.py
--rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a2/pyeo/features/__init__.py
--rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a2/pyeo/features/feature.py
--rw-r--r--   0        0        0     1553 2023-07-23 14:12:32.395680 eo_styleguide-0.0.1a2/pyeo/features/final_object.py
--rw-r--r--   0        0        0     2389 2023-07-23 13:29:32.046454 eo_styleguide-0.0.1a2/pyeo/features/method_has_protocol.py
--rw-r--r--   0        0        0     1768 2023-07-23 13:29:32.046560 eo_styleguide-0.0.1a2/pyeo/features/object_has_protocol.py
--rw-r--r--   0        0        0     2010 2023-07-23 13:29:32.046685 eo_styleguide-0.0.1a2/pyeo/features/protocol_method_code_free.py
--rw-r--r--   0        0        0     2350 2023-07-23 14:12:32.396200 eo_styleguide-0.0.1a2/pyeo/main.py
--rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a2/pyeo/py.typed
--rw-r--r--   0        0        0      797 2023-07-23 14:12:39.888892 eo_styleguide-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     3421 2023-07-29 13:16:52.754001 eo_styleguide-0.0.1a3/README.md
+-rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a3/pyeo/__init__.py
+-rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a3/pyeo/features/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a3/pyeo/features/feature.py
+-rw-r--r--   0        0        0     1553 2023-07-23 14:12:32.395680 eo_styleguide-0.0.1a3/pyeo/features/final_object.py
+-rw-r--r--   0        0        0     2724 2023-07-29 05:28:56.222285 eo_styleguide-0.0.1a3/pyeo/features/method_has_protocol.py
+-rw-r--r--   0        0        0     2639 2023-07-29 05:28:56.222616 eo_styleguide-0.0.1a3/pyeo/features/no_code_in_ctors.py
+-rw-r--r--   0        0        0     1739 2023-07-25 19:51:55.626481 eo_styleguide-0.0.1a3/pyeo/features/no_er_names.py
+-rw-r--r--   0        0        0     1711 2023-07-26 11:22:26.628858 eo_styleguide-0.0.1a3/pyeo/features/no_property_methods.py
+-rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a3/pyeo/features/no_reflection.py
+-rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a3/pyeo/features/no_setters.py
+-rw-r--r--   0        0        0     1729 2023-07-29 11:19:51.010786 eo_styleguide-0.0.1a3/pyeo/features/no_staticmethods.py
+-rw-r--r--   0        0        0     1768 2023-07-23 13:29:32.046560 eo_styleguide-0.0.1a3/pyeo/features/object_has_protocol.py
+-rw-r--r--   0        0        0     2092 2023-07-26 10:49:44.099286 eo_styleguide-0.0.1a3/pyeo/features/protocol_method_code_free.py
+-rw-r--r--   0        0        0     3089 2023-07-29 13:16:52.754447 eo_styleguide-0.0.1a3/pyeo/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a3/pyeo/py.typed
+-rw-r--r--   0        0        0      813 2023-07-29 13:17:17.336205 eo_styleguide-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a3/PKG-INFO
```

### Comparing `eo_styleguide-0.0.1a2/README.md` & `eo_styleguide-0.0.1a3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,33 +2,59 @@
 
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 
 Pyeo  is an advanced static analysis tool tailored specifically to enforce the principles advocated by
 Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure
 that your Python code adheres to the core tenets of elegance, simplicity, and maintainability.
 
+```bash
+pip install eo-styleguide
+```
+
+Simple example of usage:
+
+```python
+from typing import Protocol, final
+
+import attrs
+from pyeo import elegant
+
+
+class House(Protocol):
+    def area(self) -> int: ...
+
+
+@elegant
+@final
+@attrs.define(frozen=True)
+class HttpHouse(House):
+
+    def area(self) -> int:
+        return 10
+```
+
 - [x] ~~No null~~ ([why?](http://www.yegor256.com/2014/05/13/why-null-is-bad.html))
 
 Mypy helps prevent AttributeError and other type-related errors by providing static type checking for Python code. It allows specifying variable types, function arguments, and return types to catch potential type issues before the program runs. By using Mypy, developers can identify and fix problems related to attribute access and other type mismatches, leading to improved code quality and easier maintenance.
 
-- [ ] No code in constructors ([why?](http://www.yegor256.com/2015/05/07/ctors-must-be-code-free.html))
+- [x] No code in constructors ([why?](http://www.yegor256.com/2015/05/07/ctors-must-be-code-free.html))
 
-- [ ] No getters and setters ([why?](http://www.yegor256.com/2014/09/16/getters-and-setters-are-evil.html))
+- [x] No getters and setters ([why?](http://www.yegor256.com/2014/09/16/getters-and-setters-are-evil.html))
 
 - [x] No mutable objects ([why?](http://www.yegor256.com/2014/06/09/objects-should-be-immutable.html))
 
 `attrs.define(frozen=True)` is a parameter used in the attrs library to create classes with attributes that cannot be modified after the instance is created (i.e., immutable or "frozen" classes).
 The [attrs](https://www.attrs.org/en/stable/) library allows defining classes using the `@attr.s` decorator or by explicitly calling the `attr.define` function, and `frozen=True` is one of the parameters for specifying attribute behavior in the class. 
 When you use `attrs.define(frozen=True)` for a class, all its attributes become read-only after the instance is created, making the class "frozen" or "immutable," preventing any changes to its attribute values.
 
-- [ ] No readers, parsers, controllers, sorters, and so on ([why?](https://www.yegor256.com/2015/03/09/objects-end-with-er.html))
+- [x] No readers, parsers, controllers, sorters, and so on ([why?](https://www.yegor256.com/2015/03/09/objects-end-with-er.html))
 
-- [ ] No static methods, not even private ones ([why?](http://www.yegor256.com/2017/02/07/private-method-is-new-class.html))
+- [x] No static methods, not even private ones ([why?](http://www.yegor256.com/2017/02/07/private-method-is-new-class.html))
 
-- [ ] No instanceof, type casting, or reflection ([why?](http://www.yegor256.com/2015/04/02/class-casting-is-anti-pattern.html))
+- [x] No instanceof, type casting, or reflection ([why?](http://www.yegor256.com/2015/04/02/class-casting-is-anti-pattern.html))
 
 - [x] No public methods without a contract (interface) ([why?](https://www.yegor256.com/2014/11/20/seven-virtues-of-good-object.html#2-he-works-by-contracts))
 
 - [ ] No statements in test methods except assert ([why?](http://www.yegor256.com/2017/05/17/single-statement-unit-tests.html))
 
 - [ ] No ORM or ActiveRecord ([why?](https://www.yegor256.com/2014/12/01/orm-offensive-anti-pattern.html) and [why?](https://www.yegor256.com/2016/07/26/active-record.html))
```

### Comparing `eo_styleguide-0.0.1a2/pyeo/__init__.py` & `eo_styleguide-0.0.1a3/pyeo/features/feature.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
+from typing import Protocol
 
 
-def elegant(class_):
-    """Decorator for elegant objects and protocols.
+class Feature(Protocol):
+    """Feature interface."""
 
-    :param class_: decorated class
-    """
+    def analyze(self, ctx) -> bool:
+        """Analyzing.
+
+        :param ctx: mypy context
+        """
```

### Comparing `eo_styleguide-0.0.1a2/pyeo/features/__init__.py` & `eo_styleguide-0.0.1a3/pyeo/features/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a2/pyeo/features/feature.py` & `eo_styleguide-0.0.1a3/pyeo/features/object_has_protocol.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,18 +16,27 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from typing import Protocol
 
 
-class Feature(Protocol):
-    """Feature interface."""
+class ObjectHasProtocolFeature(object):
+    """Check object has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
+        :return: bool
         """
+        if not ctx.cls.base_type_exprs:
+            ctx.api.fail("Class '{0}' does not implement a Protocol.".format(ctx.cls.name), ctx.cls)
+            return False
+        base_type_exprs = ctx.cls.base_type_exprs[0]
+        for node in base_type_exprs.node.mro:
+            if node.is_protocol:
+                return True
+        ctx.api.fail("Class '{0}' does not implement a Protocol.".format(ctx.cls.name), ctx.cls)
+        return False
```

### Comparing `eo_styleguide-0.0.1a2/pyeo/features/final_object.py` & `eo_styleguide-0.0.1a3/pyeo/features/final_object.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a2/pyeo/features/method_has_protocol.py` & `eo_styleguide-0.0.1a3/pyeo/features/method_has_protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
+from mypy.nodes import Decorator
 
 
 class EachMethodHasProtocolFeature(object):
     """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         object_methods = {
             def_body.name: def_body
             for def_body in ctx.cls.defs.body
-            if not def_body.name.startswith('_')
+            if not def_body.name.startswith('_') and not self._method_is_ctor(def_body)
         }
         if not ctx.cls.base_type_exprs:
             return False
         extra_method_names = set(object_methods.keys()) - {  # noqa: WPS224 need a refactor
             method.name
             for base_type in ctx.cls.base_type_exprs
             for node in base_type.node.mro
@@ -55,7 +56,15 @@
                     "Class '{0}' have public extra method '{1}' without protocol.".format(
                         ctx.cls.name,
                         method.name,
                     ),
                     method,
                 )
         return True
+
+    def _method_is_ctor(self, def_body) -> bool:
+        if not isinstance(def_body, Decorator):
+            return False
+        for dec in def_body.original_decorators:
+            if dec.name == 'classmethod':
+                return True
+        return False
```

### Comparing `eo_styleguide-0.0.1a2/pyeo/features/object_has_protocol.py` & `eo_styleguide-0.0.1a3/pyeo/features/no_code_in_ctors.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,27 +16,49 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
+from mypy.nodes import AssignmentStmt, Decorator, ReturnStmt
 
 
-class ObjectHasProtocolFeature(object):
-    """Check object has protocol."""
+class NoCodeInCtorFeature(object):
+    """Checking each object method has protocol."""
 
     def analyze(self, ctx) -> bool:
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
-        if not ctx.cls.base_type_exprs:
-            ctx.api.fail("Class '{0}' does not implement a Protocol.".format(ctx.cls.name), ctx.cls)
-            return False
-        base_type_exprs = ctx.cls.base_type_exprs[0]
-        for node in base_type_exprs.node.mro:
-            if node.is_protocol:
-                return True
-        ctx.api.fail("Class '{0}' does not implement a Protocol.".format(ctx.cls.name), ctx.cls)
-        return False
+        for func in ctx.cls.defs.body:
+            if isinstance(func, Decorator) and 'classmethod' in {dec.name for dec in func.original_decorators}:
+                self._secondary_ctor_check(ctx, func)
+            elif func.name == '__init__':
+                self._primary_ctor_check(ctx, func)
+        return True
+
+    def _secondary_ctor_check(self, ctx, func):
+        for elem in func.func.body.body:
+            # TODO: ReturnStmt can contain logic like list comprehension
+            # we must iter by nodes of expr and check all elements
+            #
+            # @classmethod
+            # def secondary_ctor(cls, ages: list[str]):
+            #     return cls(
+            #         [int(x) for x in ages]
+            #     )
+            if not isinstance(elem, ReturnStmt):
+                ctx.api.fail(
+                    'Find code in ctor {0}.{1}.'.format(ctx.cls.name, func.name),
+                    ctx.cls,
+                )
+
+    def _primary_ctor_check(self, ctx, func):
+        for elem in func.body.body:
+            if not isinstance(elem, AssignmentStmt):
+                ctx.api.fail(
+                    'Find code in ctor {0}.{1}.'.format(ctx.cls.name, func.name),
+                    ctx.cls,
+                )
```

### Comparing `eo_styleguide-0.0.1a2/pyeo/features/protocol_method_code_free.py` & `eo_styleguide-0.0.1a3/pyeo/features/protocol_method_code_free.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
-from mypy.nodes import EllipsisExpr, PassStmt, StrExpr
+from mypy.nodes import EllipsisExpr, FuncDef, PassStmt, StrExpr
 
 
 class ProtocolMethodCodeFreeFeature(object):
     """Check protocol methods code free."""
 
     def analyze(self, ctx) -> bool:  # noqa: WPS231 need in refactor
         """Analyzing.
 
         :param ctx: mypy context
         :return: bool
         """
         for method in ctx.cls.defs.body:
             fail_args = ("Protocol '{0}' method '{1}' has implementation".format(ctx.cls.name, method.name), ctx.cls)
+            if not isinstance(method, FuncDef):
+                continue
             for body_item in method.body.body:
                 if isinstance(body_item, PassStmt):
                     continue
                 if not hasattr(body_item, 'expr'):  # noqa: WPS421 need in refactor
                     ctx.api.fail(*fail_args)
                     continue
                 if not isinstance(body_item.expr, (EllipsisExpr, StrExpr)):
```

### Comparing `eo_styleguide-0.0.1a2/pyeo/main.py` & `eo_styleguide-0.0.1a3/pyeo/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,31 +20,46 @@
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
 """
 from mypy.plugin import Plugin
 
 from pyeo.features.final_object import FinalClassFeature
 from pyeo.features.method_has_protocol import EachMethodHasProtocolFeature
+from pyeo.features.no_code_in_ctors import NoCodeInCtorFeature
+from pyeo.features.no_er_names import NoErNamesFeature
+from pyeo.features.no_property_methods import NoPropertyMethodsFeature
+from pyeo.features.no_reflection import NoReflectionFeature
+from pyeo.features.no_setters import NoSettersFeature
+from pyeo.features.no_staticmethods import NoStaticmethodsFeature
 from pyeo.features.object_has_protocol import ObjectHasProtocolFeature
 from pyeo.features.protocol_method_code_free import ProtocolMethodCodeFreeFeature
 
 
 def analyze(ctx):
     """Features controller.
 
     :param ctx: mypy context
     :return: bool
     """
     if ctx.cls.removed_base_type_exprs and ctx.cls.removed_base_type_exprs[0].fullname == 'typing.Protocol':
+        NoPropertyMethodsFeature().analyze(ctx)
         ProtocolMethodCodeFreeFeature().analyze(ctx)
+        NoSettersFeature().analyze(ctx)
+        NoStaticmethodsFeature().analyze(ctx)
         return True
     if not ObjectHasProtocolFeature().analyze(ctx):
         return True
     EachMethodHasProtocolFeature().analyze(ctx)
     FinalClassFeature().analyze(ctx)
+    NoErNamesFeature().analyze(ctx)
+    NoPropertyMethodsFeature().analyze(ctx)
+    NoSettersFeature().analyze(ctx)
+    NoCodeInCtorFeature().analyze(ctx)
+    NoStaticmethodsFeature().analyze(ctx)
+    NoReflectionFeature().analyze(ctx)
     return True
 
 
 class CustomPlugin(Plugin):
     """Our plugin for mypy."""
 
     def get_class_decorator_hook_2(self, fullname: str):  # noqa: WPS114 mypy api
```

### Comparing `eo_styleguide-0.0.1a2/pyproject.toml` & `eo_styleguide-0.0.1a3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "eo-styleguide"
 packages = [
     {include = "pyeo"}
 ]
-version = "0.0.1-alpha2"
+version = "0.0.1-alpha3"
 description = "Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability."
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 mypy = "^1.0"
+attrs = "^23.0"
 
 [tool.poetry.group.dev.dependencies]
 wemake-python-styleguide = "0.17.0"
 pytest-mypy-plugins = "2.0.0"
 flake8-copyright = "0.2.4"
 
 [build-system]
```

### Comparing `eo_styleguide-0.0.1a2/PKG-INFO` & `eo_styleguide-0.0.1a3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,78 @@
 Metadata-Version: 2.1
 Name: eo-styleguide
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability.
 License: MIT
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=23.0,<24.0)
 Requires-Dist: mypy (>=1.0,<2.0)
 Description-Content-Type: text/markdown
 
 # pyeo
 
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 
 Pyeo  is an advanced static analysis tool tailored specifically to enforce the principles advocated by
 Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure
 that your Python code adheres to the core tenets of elegance, simplicity, and maintainability.
 
+```bash
+pip install eo-styleguide
+```
+
+Simple example of usage:
+
+```python
+from typing import Protocol, final
+
+import attrs
+from pyeo import elegant
+
+
+class House(Protocol):
+    def area(self) -> int: ...
+
+
+@elegant
+@final
+@attrs.define(frozen=True)
+class HttpHouse(House):
+
+    def area(self) -> int:
+        return 10
+```
+
 - [x] ~~No null~~ ([why?](http://www.yegor256.com/2014/05/13/why-null-is-bad.html))
 
 Mypy helps prevent AttributeError and other type-related errors by providing static type checking for Python code. It allows specifying variable types, function arguments, and return types to catch potential type issues before the program runs. By using Mypy, developers can identify and fix problems related to attribute access and other type mismatches, leading to improved code quality and easier maintenance.
 
-- [ ] No code in constructors ([why?](http://www.yegor256.com/2015/05/07/ctors-must-be-code-free.html))
+- [x] No code in constructors ([why?](http://www.yegor256.com/2015/05/07/ctors-must-be-code-free.html))
 
-- [ ] No getters and setters ([why?](http://www.yegor256.com/2014/09/16/getters-and-setters-are-evil.html))
+- [x] No getters and setters ([why?](http://www.yegor256.com/2014/09/16/getters-and-setters-are-evil.html))
 
 - [x] No mutable objects ([why?](http://www.yegor256.com/2014/06/09/objects-should-be-immutable.html))
 
 `attrs.define(frozen=True)` is a parameter used in the attrs library to create classes with attributes that cannot be modified after the instance is created (i.e., immutable or "frozen" classes).
 The [attrs](https://www.attrs.org/en/stable/) library allows defining classes using the `@attr.s` decorator or by explicitly calling the `attr.define` function, and `frozen=True` is one of the parameters for specifying attribute behavior in the class. 
 When you use `attrs.define(frozen=True)` for a class, all its attributes become read-only after the instance is created, making the class "frozen" or "immutable," preventing any changes to its attribute values.
 
-- [ ] No readers, parsers, controllers, sorters, and so on ([why?](https://www.yegor256.com/2015/03/09/objects-end-with-er.html))
+- [x] No readers, parsers, controllers, sorters, and so on ([why?](https://www.yegor256.com/2015/03/09/objects-end-with-er.html))
 
-- [ ] No static methods, not even private ones ([why?](http://www.yegor256.com/2017/02/07/private-method-is-new-class.html))
+- [x] No static methods, not even private ones ([why?](http://www.yegor256.com/2017/02/07/private-method-is-new-class.html))
 
-- [ ] No instanceof, type casting, or reflection ([why?](http://www.yegor256.com/2015/04/02/class-casting-is-anti-pattern.html))
+- [x] No instanceof, type casting, or reflection ([why?](http://www.yegor256.com/2015/04/02/class-casting-is-anti-pattern.html))
 
 - [x] No public methods without a contract (interface) ([why?](https://www.yegor256.com/2014/11/20/seven-virtues-of-good-object.html#2-he-works-by-contracts))
 
 - [ ] No statements in test methods except assert ([why?](http://www.yegor256.com/2017/05/17/single-statement-unit-tests.html))
 
 - [ ] No ORM or ActiveRecord ([why?](https://www.yegor256.com/2014/12/01/orm-offensive-anti-pattern.html) and [why?](https://www.yegor256.com/2016/07/26/active-record.html))
```

