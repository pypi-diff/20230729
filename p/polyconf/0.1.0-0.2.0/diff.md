# Comparing `tmp/polyconf-0.1.0.tar.gz` & `tmp/polyconf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyconf-0.1.0.tar", max compression
+gzip compressed data, was "polyconf-0.2.0.tar", max compression
```

## Comparing `polyconf-0.1.0.tar` & `polyconf-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1070 2023-06-10 01:30:40.153095 polyconf-0.1.0/LICENSE
--rw-r--r--   0        0        0     1257 2023-06-11 21:28:24.320179 polyconf-0.1.0/README.md
--rw-r--r--   0        0        0     3161 2023-06-11 22:09:06.020813 polyconf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 01:30:40.154095 polyconf-0.1.0/src/polyconf/core/__init__.py
--rw-r--r--   0        0        0     1097 2023-06-11 21:21:06.076522 polyconf-0.1.0/src/polyconf/core/deepmerge.py
--rw-r--r--   0        0        0     7629 2023-06-10 01:30:40.154095 polyconf-0.1.0/src/polyconf/core/model/__init__.py
--rw-r--r--   0        0        0      788 2023-06-10 01:30:40.154095 polyconf-0.1.0/src/polyconf/core/model/context.py
--rw-r--r--   0        0        0    11219 2023-06-11 21:08:49.606031 polyconf-0.1.0/src/polyconf/core/model/datum.py
--rw-r--r--   0        0        0     4295 2023-06-10 01:30:40.155095 polyconf-0.1.0/src/polyconf/core/model/plugin.py
--rw-r--r--   0        0        0      686 2023-06-10 14:58:11.548868 polyconf-0.1.0/src/polyconf/core/model/status.py
--rw-r--r--   0        0        0     3941 2023-06-10 01:30:40.155095 polyconf-0.1.0/src/polyconf/core/registry.py
--rw-r--r--   0        0        0     3238 2023-06-10 01:30:40.155095 polyconf-0.1.0/src/polyconf/core/typing_.py
--rw-r--r--   0        0        0     1422 2023-06-10 01:30:40.155095 polyconf-0.1.0/src/polyconf/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-10 01:30:40.155095 polyconf-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      196 2023-06-10 02:02:13.577270 polyconf-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0    26272 2023-06-10 01:30:40.155095 polyconf-0.1.0/tests/test_plugin.py
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 polyconf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-10 01:30:40.153095 polyconf-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1279 2023-06-15 15:29:21.055694 polyconf-0.2.0/README.md
+-rw-r--r--   0        0        0     2749 2023-07-29 16:27:06.768723 polyconf-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 01:30:40.154095 polyconf-0.2.0/src/polyconf/core/__init__.py
+-rw-r--r--   0        0        0     1890 2023-07-20 00:52:39.389043 polyconf-0.2.0/src/polyconf/core/deepmerge.py
+-rw-r--r--   0        0        0     7583 2023-07-23 00:00:07.199244 polyconf-0.2.0/src/polyconf/core/model/__init__.py
+-rw-r--r--   0        0        0      795 2023-07-20 00:58:56.617155 polyconf-0.2.0/src/polyconf/core/model/context.py
+-rw-r--r--   0        0        0    13147 2023-07-20 00:18:12.694346 polyconf-0.2.0/src/polyconf/core/model/datum.py
+-rw-r--r--   0        0        0     4309 2023-07-19 23:01:37.615542 polyconf-0.2.0/src/polyconf/core/model/plugin.py
+-rw-r--r--   0        0        0      707 2023-07-20 01:00:22.201583 polyconf-0.2.0/src/polyconf/core/model/status.py
+-rw-r--r--   0        0        0     5426 2023-07-23 15:31:28.778428 polyconf-0.2.0/src/polyconf/core/registry.py
+-rw-r--r--   0        0        0     3238 2023-06-10 01:30:40.155095 polyconf-0.2.0/src/polyconf/core/typing_.py
+-rw-r--r--   0        0        0     1422 2023-06-10 01:30:40.155095 polyconf-0.2.0/src/polyconf/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-23 13:44:26.524557 polyconf-0.2.0/src/polyconf/mock_plugins/ipsum/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-23 15:20:24.180805 polyconf-0.2.0/src/polyconf/mock_plugins/ipsum/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-23 13:44:26.524557 polyconf-0.2.0/src/polyconf/mock_plugins/lorem/__init__.py
+-rw-r--r--   0        0        0      702 2023-07-23 15:19:39.920605 polyconf-0.2.0/src/polyconf/mock_plugins/lorem/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-10 01:30:40.155095 polyconf-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-10 02:02:13.577270 polyconf-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0    26272 2023-06-10 01:30:40.155095 polyconf-0.2.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 polyconf-0.2.0/PKG-INFO
```

### Comparing `polyconf-0.1.0/LICENSE` & `polyconf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyconf-0.1.0/README.md` & `polyconf-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,9 @@
 ```
 
 The refactor is _heavy_, indeed.  At the time of this writing, `cloc` calculates it at only `22` lines of code.
 However, I still want to give credit where it's due because there are a couple lessons in recursion
 and fallback behavior that would have been painful to work out myself.
 It also serves as a reminder for future reference because if I ever reverse the moratorium on 3rd party libs,
 I'll happily depend on `deepmerge` directly.
+
+<!-- github-only -->
```

### Comparing `polyconf-0.1.0/src/polyconf/core/model/__init__.py` & `polyconf-0.2.0/src/polyconf/core/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,31 +20,27 @@
         - Put another way, it's generic for "str | int | bool | None"
         - A motivation is ease of serialization (including JSON).
     - datum -- Is the blessed "augmented scalar".
         - Although it has an attribute that is a collection, a datum itself (class level) is not a collection.
         - Note the use of "scalar" is more restrictive and does not imply "datum".
     - collection -- Is specifically constrained to native collection types "set | list | dict".
         - In general, the members/values are "scalars" (as defined above) and/or "datums".
-        - Specific to representing collections as datums,
-          in the case of dict, the keys are explicit and the type implies the collection type.
+        - Specific to representing collections as datums, in the case of dict, the keys are explicit and the type implies the collection type.
             - int key implies a list
             - str key implies a dict
         - Note there currently isn't a case for collections of collections (perhaps called "2nd order collection"?).
             - This is because when composing data with "datums",
               collection are always represented with a datum and its "children" attribute.
     - serialization -- In general (outside of PolyConf), usually implies targeting outside the application,
       whether to disk or over the network, but PolyConf's usage is closer to "marshalling" (should I refactor?).
       The target is portability within the application, thus the "de/serialize()" methods produce native Python
       objects and not a (usually JSON) string.
-        - A motivation (perhaps primary) is to ease deep merging between "datums",
-          which is a complex topic/task.
-        - I vendored a library ("deepmerge") that has exhaustive support for deep merging dictionaries.
-          Therefore, the "merge" process serials each side to dictionaries, the deserializes the result.
-        - Currently, the use cases are constrained within PolyConf, but it's easily conceivable that the
-          application using PolyConf could use it, too (thus it's publicly exposed).
+      - A motivation (perhaps primary) is to ease deep merging between "datums", which is a complex topic/task.
+      - I vendored a library ("deepmerge") that has exhaustive support for deep merging dictionaries. Therefore, the "merge" process serials each side to dictionaries, the deserializes the result.
+      - Currently, the use cases are constrained within PolyConf, but it's easily conceivable that the application using PolyConf could use it, too (thus it's publicly exposed).
 
 Maxims:
     - "value" and "children" are mutually exclusive.
     - "value" indicates a leaf node
     - "value" is always a scalar object
     - "children" is a collection
     - "children" members are always Datums
```

### Comparing `polyconf-0.1.0/src/polyconf/core/model/context.py` & `polyconf-0.2.0/src/polyconf/core/model/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+"""Context"""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any
 
 from .datum import Datum
 from .status import Status, status_new
 
 
 def root_datum() -> Datum:
+    """Factory function to create a root datum."""
     return Datum(name="root")
 
 
 @dataclass
 class Context:
+    """PolyConf runtime context"""
+
     app_name: str
     app_prefix: str = ""
     trim_prefix: bool = True
     given: dict[str, Any] = field(default_factory=dict)
     status: Status = field(default_factory=status_new)
     result: Datum = field(default_factory=root_datum)
 
     def __post_init__(self) -> None:
         self.app_prefix = self.app_prefix or self.app_name.upper()
 
         if self.given:
-            # self.result = {k: Datum(k, v, sources={"given"}) for k, v in self.given.items()}
             self.result = Datum.from_dict(data=self.given, source="given")
```

### Comparing `polyconf-0.1.0/src/polyconf/core/model/datum.py` & `polyconf-0.2.0/src/polyconf/core/model/datum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Datum module."""
+"""Datum"""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, Self, Type, TypeVar
 
 from polyconf.core import typing_ as t
@@ -35,29 +35,39 @@
     name: t.PrimitiveIndex
     value: t.PrimitiveScalar = None
     children: set[Datum] = field(default_factory=set)
     sources: set[str] = field(default_factory=set)
 
     @property
     def children_names(self) -> set[t.PrimitiveIndex]:
+        """Name attributes of all children as a set."""
         return {c.name for c in self.children}
 
     @property
     def as_native_value(self) -> t.PrimitiveType:
+        """Native representation of the data value."""
         # NOTE: currently not actively in use, but it seems useful and works well.
         if self.value is not None:
             return self.value
-        elif self.children:
+
+        if self.children:
             if self.looks_like() == list:
                 return [child.as_native_value for child in self.children]
             return {c.name: c.as_native_value for c in self.children}
-        else:
-            return None
+
+        return None
 
     def add_child(self, datum: Datum, merge: bool = False) -> None:
+        """Add a child to the collection.
+
+        Args:
+            datum: The child to add.
+            merge: Whether to merge the existing child with the new one.
+        """
+
         if existing_child := self.get(name=datum.name):
             # When exists, always drop first because "merge" intends to "replace".
             self.remove_child(datum)
 
             if merge:
                 merged_child = existing_child | datum
                 self.children.add(merged_child)
@@ -65,41 +75,57 @@
                 self.children.add(datum)
 
         # New child
         else:
             self.children.add(datum)
 
     def remove_child(self, datum: Datum) -> None:
+        """Remove a child from the collection.
+
+        Args:
+            datum: The child to remove.
+
+        Note:
+            This is more well behaved than:
+                `self.children.discard(datum)`
+                (or `self.children.remove(datum)`)
+            because the native lookup is based on hash, but the desired basis is on name.
+        """
         if found_child := self.get(datum.name):
             self.children.remove(found_child)
 
-        # Note: This is more well behaved than:
-        # self.children.discard(datum)
-        #   (or self.children.remove(datum))
-        # because the native lookup is based on hash, while the desired basis is on name.
-
     def put(
         self,
         name: t.PrimitiveIndex,
         value: t.PrimitiveScalar = None,
         source: str | None = None,
         merge: bool = False,
     ) -> None:
+        """Put a raw value into the collection.
+
+        Args:
+            name: The name of the value.
+            value: The value to store.
+            source: The source of the value.
+            merge: Whether to merge the existing child with the new one.
+        """
         if name not in self.children_names:
-            sources = set() if source is None else {source}
+            sources: set[str] = set() if source is None else {source}
             self.add_child(Datum(name=name, value=value, sources=sources), merge=merge)
             return
 
         # TODO: Confirm these changes persist.
         if child_node := self.get(name=name):
             child_node.value = value
             if source:
                 child_node.sources.add(source)
 
     def traverse(self) -> None:
+        """Traverse the collection."""
+
         nodes_to_visit = [self]
         while nodes_to_visit:
             current_node = nodes_to_visit.pop()
             bad_state = all(
                 [
                     current_node.value is not None,
                     current_node.children is not None,
@@ -116,49 +142,64 @@
         """Get child datum by name.
 
         Queries self.children for a matching "name" attribute.
         If not found, it returns a default, which may be specified by the caller.
 
         Args:
             name: The child datum name to retrieve.
-            default: The default value to return if the child is not found.
-                Defaults to None.
+            default: The default value to return if the child is not found. Defaults to None.
         """
         return next((child for child in self.children if child.name == name), default)
 
     def eq_helper(self) -> str:
+        """Helper for equality comparison."""
+
         fields = [
             self.name,
             self.value,
             sorted(self.children),
             sorted(self.sources),
         ]
         return "|".join(repr(x) for x in fields)
 
     def looks_like(self) -> Type[str | int | bool | list[Any] | dict[Any, Any]]:
+        """Check if the datum looks like a primitive value."""
+
         if self.value is not None:
             return self.value.__class__
 
-        first_index = list(self.children)[0].name
+        first_index: str | int = list(self.children)[0].name
+
         if isinstance(first_index, int):
-            return list
-        elif isinstance(first_index, str):
-            return dict
-        else:
-            raise TypeError(first_index)
+            return list  # pyright: ignore [reportUnknownVariableType]
+
+        if isinstance(first_index, str):
+            return dict  # pyright: ignore [reportUnknownVariableType]
+
+        raise TypeError(first_index)
 
     @classmethod
     def assimilate(
         cls,
         name: t.PrimitiveIndex,
         data: t.PrimitiveType,
         source: str,
         parent: Self,
         merge: bool = False,
     ) -> None:
+        """Assimilate! Naming is hard.
+
+        Args:
+            name: The name of the value.
+            data: The value to store.
+            source: The source of the value.
+            parent: The parent node.
+            merge: Whether to merge the existing child with the new one.
+        """
+
         # Plain scalar value -- no recursion.
         if t.is_primitive_scalar(data) and data is not None:
             parent.put(name=name, value=data, source=source, merge=merge)
 
         # Container value -- perform recursion.
         elif t.is_primitive_dict(data):
             dict_node = cls(name=name, sources={source})
@@ -173,14 +214,23 @@
             parent.add_child(list_node, merge=merge)
 
         else:
             raise TypeError(data)
 
     @classmethod
     def from_dict(cls, data: dict[str, Any], source: str = "cls-factory") -> Self:
+        """Create a datum from a dictionary.
+
+        Args:
+            data: The dictionary to convert to a datum. Keys must be strings.
+            source: The source of the datum.
+
+        Returns:
+            The datum created from the dictionary.
+        """
         root = cls(name="root", sources={source})
         for key, value in data.items():
             root.assimilate(name=key, data=value, source=source, parent=root)
         return root
 
     # def _is_valid_datum_serial(self, data: t.PrimitiveDict) -> bool:
 
@@ -244,32 +294,50 @@
 
         # root = cls(name="root", sources={source})
         # for key, value in data.items():
         #     root.assimilate(name=key, data=value, source=source, parent=root)
         # return root
 
     def serialize(self) -> t.PrimitiveDict:
+        """Serialize the datum to a dictionary.
+
+        Returns:
+            The serialized datum.
+        """
         data: t.PrimitiveDict = {
             "name": self.name,
         }
         if self.value is not None:
             data["value"] = self.value
         if self.children:
             data["children"] = [child.serialize() for child in sorted(self.children)]
         if self.sources:
             data["sources"] = list(self.sources)
         return data
 
-    def __or__(self, other: Datum) -> Datum:
+    def __or__(self, other: Any) -> Datum:
+        """Merge this datum with another datum.
+
+        This is achieved by serializing the datums to dictionaries, using deep.merge() to merge those dictionaries,
+        then deserializing the merged dictionary back to a datum.
+
+        Args:
+            other: The datum to merge with.
+
+        Returns:
+            The merged datum.
+
+        Raises:
+            NotImplemented: If the other datum is not a datum.
+        """
         if not isinstance(other, Datum):
             return NotImplemented
 
         self_dict = self.serialize()
         other_dict = other.serialize()
-        # other_dict: dict = other.serialize() if isinstance(other, Datum) else other
 
         deep.merge(self_dict, other_dict)  # type:ignore
 
         return self.deserialize(self_dict)
 
     def __ror__(self, other: Datum) -> Datum:
         if not isinstance(other, Datum):
```

### Comparing `polyconf-0.1.0/src/polyconf/core/model/plugin.py` & `polyconf-0.2.0/src/polyconf/core/model/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Plugin"""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 from polyconf.core import typing_ as t
```

### Comparing `polyconf-0.1.0/src/polyconf/core/registry.py` & `polyconf-0.2.0/src/polyconf/core/registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,69 @@
+"""Registry"""
+
 import importlib
 import logging
 import pkgutil
 import types
 from collections.abc import Iterator
+from dataclasses import asdict
 from typing import Any, Callable
 
 from polyconf.core.model import Context, Plugin
 from polyconf.core.utils import pipe
 
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger(__name__)
 
 
 def iter_namespace(ns_pkg: types.ModuleType) -> Iterator[pkgutil.ModuleInfo]:
-    # Specifying the second argument (prefix) to iter_modules makes the
-    # returned name an absolute name instead of a relative one. This allows
-    # import_module to work without having to do additional modification to
-    # the name.
+    """Iterate over all modules in a namespace package.
+
+    Specifying the second argument (prefix) to iter_modules makes the
+    returned name an absolute name instead of a relative one. This allows
+    import_module to work without having to do additional modification to
+    the name.
+    """
 
     return pkgutil.iter_modules(ns_pkg.__path__, f"{ns_pkg.__name__}.")
 
     # ns_pkg_path = ns_pkg.__path__
     # result = pkgutil.walk_packages(ns_pkg_path, f"{ns_pkg.__name__}.")
     # return result
 
 
 class Registry:
+    """Registry of plugins."""
+
     def __init__(self, selected_plugins: list[str], **kwargs: Plugin) -> None:
         self.selected_plugins: list[str] = selected_plugins
         self._discovered_plugin_modules: dict[str, types.ModuleType] = {}
-        self._active_plugin_modules: dict[str, Any] = {}
+        self._active_plugin_modules: dict[str, types.ModuleType] = {}
         self._active_plugins: dict[str, Plugin] = kwargs
 
     def discover_plugins(self, package: types.ModuleType) -> None:
+        """Discover plugins in a package."""
+
         # fmt: off
         self._discovered_plugin_modules = {
             name.removeprefix(f"{package.__name__}."): importlib.import_module(f"{name}.plugin")
             for _finder, name, _is_pkg
             in iter_namespace(package)
         }
         # fmt: on
 
     @property
     def discovered_plugins(self) -> dict[str, types.ModuleType]:
+        """Return a dictionary of discovered plugins."""
         return self._discovered_plugin_modules
 
     def init_plugins(self, package: types.ModuleType | None = None, **kwargs: Any) -> None:
+        """Initialize the plugins."""
+
         if package is None:
             log.warning("No package specified. Doing nothing.")
             return
 
         if not self._discovered_plugin_modules:
             self.discover_plugins(package)
 
@@ -70,54 +83,90 @@
             name: module.factory(**kwargs)
             for name, module in self._active_plugin_modules.items()
         }
         # fmt: on
 
     @property
     def available_plugins(self) -> list[Callable[[Context], Context]]:
+        """Return a list of available plugins."""
         return [plugin.hydrate for plugin in self._active_plugins.values()]
 
     @property
     def plugins(self) -> list[Callable[[Context], Context]]:
-        if not self.selected_plugins:
+        """Return a list of active plugins."""
+        if not self.selected_plugins or self.selected_plugins == ["ALL"]:
             return self.available_plugins
         # fmt: off
         return [
             plugin.hydrate
             for plugin in self._active_plugins.values()
             if plugin.name in self.selected_plugins
         ]
         # fmt: on
 
     @property
     def plugin_map(self) -> dict[str, Plugin]:
+        """Return a dictionary of active plugins."""
         return self._active_plugins
 
     def register_plugin(self, name: str, plugin: Plugin) -> None:
+        """Register a plugin."""
         self._active_plugins[name] = plugin
 
+    def resolve(self, context: Context) -> Context:
+        """Resolve a context."""
+        return pipe(context, *self.plugins)
+
 
 class FooPlugin(Plugin):
+    """A (temporary) dummy plugin for testing."""
+
     name = "foo"
 
     def hydrate(self, context: Context) -> Context:
         self.logger.info(f'{self.name} says, "hello"')
+        self.add_result("zz", "ZZZ", context, "fake")
+        self.add_result("foo", True, context, "fake")
         return context
 
 
 class BarPlugin(Plugin):
+    """Another (temporary) dummy plugin for testing."""
+
     name = "bar"
 
     def hydrate(self, context: Context) -> Context:
         self.logger.info(f'{self.name} says, "hello"')
-        self.add_result("zz", "ZZ", context, "fake")
+        self.add_result("zz", "zz", context, "fake")
+        self.add_result("bar", True, context, "fake")
         return context
 
 
 if __name__ == "__main__":
-    registry = Registry(selected_plugins=["bar"], foo=FooPlugin(log))
-    registry.register_plugin("bar", BarPlugin(log))
+    # registry = Registry(
+    #     selected_plugins=[
+    #         "foo",
+    #         "bar",
+    #     ],
+    #     foo=FooPlugin(log),  # register via kwargs
+    # )
+    # registry.register_plugin("bar", BarPlugin(log))  # register via method
+
+    import polyconf.mock_plugins
+    registry = Registry(selected_plugins=["ALL"])
+    registry.init_plugins(polyconf.mock_plugins, logger=log)
+    log.info(f"{registry.plugins=}")
 
     ctx = Context(app_name="widget", given={"a": "b", "c": "d"})
-    result: Context = pipe(ctx, *registry.plugins)
-    log.info(f"{result=}")
-    # log.info(f"{result.as_obj=}")
+    result: Context = registry.resolve(ctx)
+
+    # The context object is never replaced, just modified as it is passed down the pipeline.
+    assert result is ctx
+
+    log.info(f"{result.result.as_native_value=}")
+
+    d = asdict(result)
+    # log.info(f"{d['result']=}")
+
+    log.info("Result children:")
+    for child in d["result"]["children"]:
+        log.info(f"\t{child=}")
```

### Comparing `polyconf-0.1.0/src/polyconf/core/typing_.py` & `polyconf-0.2.0/src/polyconf/core/typing_.py`

 * *Files identical despite different names*

### Comparing `polyconf-0.1.0/src/polyconf/core/utils.py` & `polyconf-0.2.0/src/polyconf/core/utils.py`

 * *Files identical despite different names*

### Comparing `polyconf-0.1.0/tests/test_plugin.py` & `polyconf-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `polyconf-0.1.0/PKG-INFO` & `polyconf-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: polyconf
-Version: 0.1.0
+Version: 0.2.0
 Summary: Gather and merge configuration from many sources.
-Home-page: https://github.com/boweeb/polyconf
+Home-page: https://polyconf.readthedocs.io
 License: MIT
 Keywords: polyconf,configuration
 Author: Jesse Butcher
 Author-email: boweeb@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Documentation, https://github.com/boweeb/polyconf
+Project-URL: Documentation, https://polyconf.readthedocs.io
 Project-URL: Repository, https://github.com/boweeb/polyconf
 Description-Content-Type: text/markdown
 
 # PolyConf
 
 ## Credit
 
@@ -42,7 +42,9 @@
 
 The refactor is _heavy_, indeed.  At the time of this writing, `cloc` calculates it at only `22` lines of code.
 However, I still want to give credit where it's due because there are a couple lessons in recursion
 and fallback behavior that would have been painful to work out myself.
 It also serves as a reminder for future reference because if I ever reverse the moratorium on 3rd party libs,
 I'll happily depend on `deepmerge` directly.
 
+<!-- github-only -->
+
```

