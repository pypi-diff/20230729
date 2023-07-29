# Comparing `tmp/tcod_ecs-4.2.0.tar.gz` & `tmp/tcod_ecs-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-4.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-4.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-4.2.0.tar` & `tcod_ecs-4.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/LICENSE
--rw-r--r--   0        0        0    10905 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/README.md
--rw-r--r--   0        0        0     3527 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1394 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     1512 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/_converter.py
--rw-r--r--   0        0        0      160 2023-07-29 00:37:52.716245 tcod_ecs-4.2.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0    30100 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/entity.py
--rw-r--r--   0        0        0        0 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0    14844 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/query.py
--rw-r--r--   0        0        0     1113 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/typing.py
--rw-r--r--   0        0        0    11647 2023-07-29 00:37:43.503470 tcod_ecs-4.2.0/tcod/ecs/world.py
--rw-r--r--   0        0        0    12159 1970-01-01 00:00:00.000000 tcod_ecs-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/LICENSE
+-rw-r--r--   0        0        0    10905 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/README.md
+-rw-r--r--   0        0        0     3527 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1394 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0     1512 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/_converter.py
+-rw-r--r--   0        0        0      160 2023-07-29 01:38:41.763200 tcod_ecs-4.2.1/tcod/ecs/_version.py
+-rw-r--r--   0        0        0    30100 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/entity.py
+-rw-r--r--   0        0        0        0 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/py.typed
+-rw-r--r--   0        0        0    14844 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/query.py
+-rw-r--r--   0        0        0     1113 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/typing.py
+-rw-r--r--   0        0        0    11647 2023-07-29 01:38:34.211134 tcod_ecs-4.2.1/tcod/ecs/world.py
+-rw-r--r--   0        0        0    12159 1970-01-01 00:00:00.000000 tcod_ecs-4.2.1/PKG-INFO
```

### Comparing `tcod_ecs-4.2.0/LICENSE` & `tcod_ecs-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/README.md` & `tcod_ecs-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/pyproject.toml` & `tcod_ecs-4.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/tcod/ecs/__init__.py` & `tcod_ecs-4.2.1/tcod/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/tcod/ecs/_converter.py` & `tcod_ecs-4.2.1/tcod/ecs/_converter.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/tcod/ecs/entity.py` & `tcod_ecs-4.2.1/tcod/ecs/entity.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/tcod/ecs/query.py` & `tcod_ecs-4.2.1/tcod/ecs/query.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/tcod/ecs/typing.py` & `tcod_ecs-4.2.1/tcod/ecs/typing.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-4.2.0/tcod/ecs/world.py` & `tcod_ecs-4.2.1/tcod/ecs/world.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,28 +51,28 @@
     tags_by_entity: defaultdict[Entity, defaultdict[object, set[Entity]]],
     components_by_entity: defaultdict[Entity, defaultdict[_ComponentKey[object], dict[Entity, Any]]],
 ) -> defaultdict[tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]]:
     """Return the relation lookup table from the relations sparse-sets."""
     relations_lookup: defaultdict[
         tuple[Any, _RelationTargetLookup] | tuple[_RelationTargetLookup, Any, None], set[Entity]
     ] = defaultdict(set)
-    for entity, tags in tags_by_entity.items():
+    for origin, tags in tags_by_entity.items():
         for tag, targets in tags.items():
             for target in targets:
-                relations_lookup[(tag, ...)].add(target)
-                relations_lookup[(tag, entity)].add(target)
-                relations_lookup[(target, tag, None)].add(entity)
-                relations_lookup[(..., tag, None)].add(entity)
-    for entity, components in components_by_entity.items():
+                relations_lookup[(tag, ...)].add(origin)
+                relations_lookup[(tag, target)].add(origin)
+                relations_lookup[(origin, tag, None)].add(target)
+                relations_lookup[(..., tag, None)].add(target)
+    for origin, components in components_by_entity.items():
         for component_key, target_components in components.items():
             for target in target_components:
-                relations_lookup[(component_key, ...)].add(target)
-                relations_lookup[(component_key, entity)].add(target)
-                relations_lookup[(target, component_key, None)].add(entity)
-                relations_lookup[(..., component_key, None)].add(entity)
+                relations_lookup[(component_key, ...)].add(origin)
+                relations_lookup[(component_key, origin)].add(origin)
+                relations_lookup[(origin, component_key, None)].add(target)
+                relations_lookup[(..., component_key, None)].add(target)
 
     return relations_lookup
 
 
 @attrs.define(eq=False)
 class World:
     """A container for entities and components."""
```

### Comparing `tcod_ecs-4.2.0/PKG-INFO` & `tcod_ecs-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 4.2.0
+Version: 4.2.1
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

