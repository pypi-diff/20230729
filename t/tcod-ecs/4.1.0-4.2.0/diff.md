# Comparing `tmp/tcod_ecs-4.1.0.tar.gz` & `tmp/tcod_ecs-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-4.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-4.1.0.tar` & `tcod_ecs-4.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-07-28 13:55:08.163962 tcod_ecs-4.1.0/LICENSE
--rw-r--r--   0        0        0    10905 2023-07-28 13:55:08.163962 tcod_ecs-4.1.0/README.md
--rw-r--r--   0        0        0     3527 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     1394 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     1512 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/_converter.py
--rw-r--r--   0        0        0      160 2023-07-28 13:55:18.652201 tcod_ecs-4.1.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0    28196 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/entity.py
--rw-r--r--   0        0        0        0 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0    14844 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/query.py
--rw-r--r--   0        0        0     1113 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/typing.py
--rw-r--r--   0        0        0    11647 2023-07-28 13:55:08.167962 tcod_ecs-4.1.0/tcod/ecs/world.py
--rw-r--r--   0        0        0    12159 1970-01-01 00:00:00.000000 tcod_ecs-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/LICENSE
+-rw-r--r--   0        0        0    10905 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/README.md
+-rw-r--r--   0        0        0     3527 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1394 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0     1512 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/_converter.py
+-rw-r--r--   0        0        0      160 2023-07-29 00:37:52.716245 tcod_ecs-4.2.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0    30100 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/entity.py
+-rw-r--r--   0        0        0        0 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0    14844 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/query.py
+-rw-r--r--   0        0        0     1113 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/typing.py
+-rw-r--r--   0        0        0    11647 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/world.py
+-rw-r--r--   0        0        0    12159 1970-01-01 00:00:00.000000 tcod_ecs-4.2.0/PKG-INFO
```

### Comparing `tcod_ecs-4.1.0/LICENSE` & `tcod_ecs-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/README.md` & `tcod_ecs-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/pyproject.toml` & `tcod_ecs-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/tcod/ecs/__init__.py` & `tcod_ecs-4.2.0/tcod/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/tcod/ecs/_converter.py` & `tcod_ecs-4.2.0/tcod/ecs/_converter.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/tcod/ecs/entity.py` & `tcod_ecs-4.2.0/tcod/ecs/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Final,
     Generic,
     Iterable,
     Iterator,
+    KeysView,
+    Mapping,
     MutableMapping,
     MutableSet,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
@@ -94,14 +96,26 @@
             pass
         self = super().__new__(cls)
         self.world = world  # type:ignore[misc]  # https://github.com/python/mypy/issues/5774
         self.uid = uid  # type:ignore[misc]
         _entity_table[world][uid] = self
         return self
 
+    def clear(self) -> None:
+        """Deletes all of this entities components, tags, and relations.
+
+        Relations targeting this component are still kept.
+
+        .. versionadded:: 4.2.0
+        """
+        self.components.clear()
+        self.tags.clear()
+        self.relation_tags_many.clear()
+        self.relation_components.clear()
+
     @property
     def components(self) -> EntityComponents:
         """Access an entities components.
 
         Example::
 
             >>> entity.components[str] = "foo"  # Assign component
@@ -701,31 +715,66 @@
 
     def __len__(self) -> int:
         """Return the count of targets for this component relation."""
         by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
         return 0 if by_entity is None else len(by_entity.get(self.key, ()))
 
 
-class EntityComponentRelations:
+class EntityComponentRelations(MutableMapping[_ComponentKey[Any], EntityComponentRelationMapping[Any]]):
     """Proxy to access the component relations of an entity.
 
     See :any:`Entity.relation_components`.
+
+    ..versionchanged:: 4.2.0
+        Is now a :any:`MutableMapping` subtype.
     """
 
     __slots__ = ("entity",)
 
     def __init__(self, entity: Entity) -> None:
         """Initialize this attribute for the given entity."""
         assert isinstance(entity, Entity), entity
         self.entity: Final = entity
 
     def __getitem__(self, key: _ComponentKey[T]) -> EntityComponentRelationMapping[T]:
         """Access relations for this component key as a `{target: component}` dict-like object."""
         return EntityComponentRelationMapping(self.entity, key)
 
+    def __setitem__(self, __key: _ComponentKey[T], __values: Mapping[Entity, object]) -> None:
+        """Redefine the component relations for this entity.
+
+        ..versionadded:: 4.2.0
+        """
+        if isinstance(__values, EntityComponentRelationMapping) and __values.entity is self.entity:
+            return
+        mapping: EntityComponentRelationMapping[object] = self[__key]
+        mapping.clear()
+        for target, component in __values.items():
+            mapping[target] = component
+
     def __delitem__(self, key: _ComponentKey[object]) -> None:
         """Remove all relations associated with this component key."""
         EntityComponentRelationMapping(self.entity, key).clear()
 
-    def __contains__(self, key: _ComponentKey[object]) -> bool:
+    def __contains__(self, key: object) -> bool:
         """Return True if this entity contains a relation component for this component key."""
-        return bool(EntityComponentRelationMapping(self.entity, key))
+        return key in self.keys()  # noqa: SIM118 # https://github.com/astral-sh/ruff/issues/6163
+
+    def clear(self) -> None:
+        """Clears the relation components this entity has with other entities.
+
+        Does not clear relations targeting this entity.
+        """
+        for component_key in list(self):
+            self[component_key].clear()
+
+    def keys(self) -> KeysView[_ComponentKey[object]]:
+        """Returns the components keys this entity has relations for."""
+        return self.entity.world._relation_components_by_entity.get(self.entity, {}).keys()
+
+    def __iter__(self) -> Iterator[_ComponentKey[object]]:
+        """Iterates over the component keys this entity has relations for."""
+        return iter(self.keys())
+
+    def __len__(self) -> int:
+        """Returns the number of unique component keys this entity has relations for."""
+        return len(self.entity.world._relation_components_by_entity.get(self.entity, ()))
```

### Comparing `tcod_ecs-4.1.0/tcod/ecs/query.py` & `tcod_ecs-4.2.0/tcod/ecs/query.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/tcod/ecs/typing.py` & `tcod_ecs-4.2.0/tcod/ecs/typing.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/tcod/ecs/world.py` & `tcod_ecs-4.2.0/tcod/ecs/world.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.1.0/PKG-INFO` & `tcod_ecs-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 4.1.0
+Version: 4.2.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

