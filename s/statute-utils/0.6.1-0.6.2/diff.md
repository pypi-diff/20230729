# Comparing `tmp/statute_utils-0.6.1.tar.gz` & `tmp/statute_utils-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.6.1.tar", max compression
+gzip compressed data, was "statute_utils-0.6.2.tar", max compression
```

## Comparing `statute_utils-0.6.1.tar` & `statute_utils-0.6.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.1/LICENSE
--rw-r--r--   0        0        0     2640 2023-07-16 05:44:56.640061 statute_utils-0.6.1/README.md
--rw-r--r--   0        0        0     1357 2023-07-17 01:45:55.216080 statute_utils-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      858 2023-07-17 01:59:03.643591 statute_utils-0.6.1/statute_utils/__init__.py
--rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.1/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     5976 2023-07-16 05:09:00.421516 statute_utils-0.6.1/statute_utils/components/branch.py
--rw-r--r--   0        0        0     8323 2023-07-16 08:01:53.752165 statute_utils-0.6.1/statute_utils/components/builder.py
--rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.6.1/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.1/statute_utils/components/short.py
--rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.1/statute_utils/components/utils.py
--rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.1/statute_utils/config.py
--rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.1/statute_utils/main.py
--rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.1/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.1/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.1/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.1/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.1/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.1/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.1/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.1/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6640 2023-07-17 01:48:41.595692 statute_utils-0.6.1/statute_utils/statute.py
--rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.1/statute_utils/templater.py
--rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.1/statute_utils/templates/crumbs.html
--rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.1/statute_utils/templates/paragraph.html
--rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.1/statute_utils/templates/subtree.html
--rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.1/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     2416 2023-07-16 08:50:40.061466 statute_utils-0.6.1/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 statute_utils-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2640 2023-07-16 05:44:56.640061 statute_utils-0.6.2/README.md
+-rw-r--r--   0        0        0     1357 2023-07-29 18:31:00.746124 statute_utils-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.2/statute_utils/__init__.py
+-rw-r--r--   0        0        0     3035 2023-07-29 18:21:42.065621 statute_utils-0.6.2/statute_utils/codification.py
+-rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.2/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.2/statute_utils/components/branch.py
+-rw-r--r--   0        0        0     8323 2023-07-16 08:01:53.752165 statute_utils-0.6.2/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    11357 2023-07-28 03:46:47.927866 statute_utils-0.6.2/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.2/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.2/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.2/statute_utils/config.py
+-rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.2/statute_utils/main.py
+-rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.2/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.2/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.2/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.2/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.2/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.2/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.2/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.2/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6640 2023-07-29 17:46:52.576680 statute_utils-0.6.2/statute_utils/statute.py
+-rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.2/statute_utils/templater.py
+-rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.2/statute_utils/templates/crumbs.html
+-rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.2/statute_utils/templates/paragraph.html
+-rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.2/statute_utils/templates/subtree.html
+-rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.2/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     2416 2023-07-16 08:50:40.061466 statute_utils-0.6.2/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 statute_utils-0.6.2/PKG-INFO
```

### Comparing `statute_utils-0.6.1/LICENSE` & `statute_utils-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/README.md` & `statute_utils-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/pyproject.toml` & `statute_utils-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.6.1"
+version = "0.6.2"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.6.1/statute_utils/__init__.py` & `statute_utils-0.6.2/statute_utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .codification import Codification
 from .components import (
     TREE_FILTERS,
     StatuteSerialCategory,
     StatuteTitle,
     StatuteTitleCategory,
     add_blg,
     add_num,
```

### Comparing `statute_utils-0.6.1/statute_utils/components/__init__.py` & `statute_utils-0.6.2/statute_utils/components/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/components/branch.py` & `statute_utils-0.6.2/statute_utils/components/branch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-import yaml
+import yaml  # type: ignore
 
 from .builder import from_json
 
 
 def make_branch(node: dict, nodes: list[dict]) -> dict:
     """`Recursive function that adds `nodes` to a position in the subtree
     represented by `node`.
@@ -117,15 +117,15 @@
         child_key (str, optional): The node which represents a list of children nodes.
             Defaults to "units".
     """
     if isinstance(nodes, list):
         for counter, node in enumerate(nodes, start=1):
             node["id"] = f"{parent_id}{str(counter)}."
             if node.get(child_key, None):
-                set_node_ids(node[child_key], node["id"], child_key)
+                set_node_ids(node[child_key], node["id"], child_key)  # type: ignore
 
 
 class literal(str):
     pass
 
 
 def literal_presenter(dumper, data):
@@ -161,17 +161,20 @@
             data = []
             if node.get("item"):
                 candidate = node["item"]
                 if candidate := str(node["item"]).strip():
                     if candidate.isdigit():
                         candidate = int(candidate)
                 data.append(("item", candidate))
+
             if node.get("caption"):
                 data.append(("caption", node["caption"].strip()))
+
             if node.get("content"):
                 formatted_content = literal(node["content"].strip())
                 data.append(("content", formatted_content))
+
             if node.get("units", None):
                 walked_units = walk(node["units"])
                 data.append(("units", walked_units))
             revised_nodes.append(dict(data))
     return revised_nodes
```

### Comparing `statute_utils-0.6.1/statute_utils/components/builder.py` & `statute_utils-0.6.2/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/components/category.py` & `statute_utils-0.6.2/statute_utils/components/category.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         """Given the value `<v>` of a category (lowercased, as saved in the database),
         use `StatuteSerialCategory(<v>)`. This will get the proper category. Use the
         category alongside the passed `num`.
 
         Examples:
             >>> civ = StatuteSerialCategory('ra')
             >>> civ.cite('386')
-            'R.A No. 386'
+            'R.A. No. 386'
             >>> spain = StatuteSerialCategory('spain')
             >>> spain.cite('penal')
             'Spanish Penal Code'
             >>> roc = StatuteSerialCategory('roc')
             >>> roc.cite('1964')
             '1964 Rules of Court'
 
@@ -261,15 +261,15 @@
             case StatuteSerialCategory.CircularOCA:
                 return f"OCA Circular No. {num.upper()}"
             case StatuteSerialCategory.CircularSC:
                 return f"SC Circular No. {num.upper()}"
             case _:
                 ...
                 base = ".".join([i for i in self.value]).upper()
-                return f"{base} No. {num.upper()}"
+                return f"{base}. No. {num.upper()}"
 
 
 class StatuteTitle(NamedTuple):
     """Will be used to populate the database; assumes a fixed `statute_id`."""
 
     category: StatuteTitleCategory
     text: str
```

### Comparing `statute_utils-0.6.1/statute_utils/components/short.py` & `statute_utils-0.6.2/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/components/utils.py` & `statute_utils-0.6.2/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/config.py` & `statute_utils-0.6.2/statute_utils/config.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/main.py` & `statute_utils-0.6.2/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/models.py` & `statute_utils-0.6.2/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/models_names.py` & `statute_utils-0.6.2/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/models_serials.py` & `statute_utils-0.6.2/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/recipes/digits.py` & `statute_utils-0.6.2/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/recipes/spain.py` & `statute_utils-0.6.2/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/statute.py` & `statute_utils-0.6.2/statute_utils/statute.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
     walk,
 )
 from .models import Rule
 from .templater import html_tree_from_hierarchy
 
 
 class Statute(NamedTuple):
-    """A instance is dependent on a statute path from a fixed
-    directory. The shape of the Python object will be different
+    """A instance is dependent on a specifically
+    formatted statute Path.
+
+    The shape of the contents will be different
     from the shape of the dumpable `.yml` export."""
 
     titles: list[StatuteTitle]
     rule: Rule
     variant: int
     date: datetime.date
     units: list[dict]
```

### Comparing `statute_utils-0.6.1/statute_utils/templater.py` & `statute_utils-0.6.2/statute_utils/templater.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/templates/tree.css` & `statute_utils-0.6.2/statute_utils/templates/tree.css`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/statute_utils/templates/tree.html` & `statute_utils-0.6.2/statute_utils/templates/tree.html`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.1/PKG-INFO` & `statute_utils-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.6.1
+Version: 0.6.2
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

