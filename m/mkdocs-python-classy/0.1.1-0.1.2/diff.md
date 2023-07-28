# Comparing `tmp/mkdocs_python_classy-0.1.1.tar.gz` & `tmp/mkdocs_python_classy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_python_classy-0.1.1.tar", max compression
+gzip compressed data, was "mkdocs_python_classy-0.1.2.tar", max compression
```

## Comparing `mkdocs_python_classy-0.1.1.tar` & `mkdocs_python_classy-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      581 2023-07-28 16:42:49.216893 mkdocs_python_classy-0.1.1/LICENSE
--rw-r--r--   0        0        0      302 2023-07-28 16:42:49.216893 mkdocs_python_classy-0.1.1/NOTICE
--rw-r--r--   0        0        0     3997 2023-07-28 16:42:49.216893 mkdocs_python_classy-0.1.1/README.md
--rw-r--r--   0        0        0     7950 2023-07-28 16:42:49.220893 mkdocs_python_classy-0.1.1/mkdocs_python_classy/__init__.py
--rw-r--r--   0        0        0      288 2023-07-28 16:42:49.220893 mkdocs_python_classy-0.1.1/mkdocs_python_classy/constants.py
--rw-r--r--   0        0        0       32 2023-07-28 16:42:49.220893 mkdocs_python_classy-0.1.1/mkdocs_python_classy/css/classy.css
--rw-r--r--   0        0        0    13413 2023-07-28 16:42:49.220893 mkdocs_python_classy-0.1.1/mkdocs_python_classy/inspector.py
--rw-r--r--   0        0        0     3743 2023-07-28 16:42:49.224893 mkdocs_python_classy-0.1.1/mkdocs_python_classy/utils.py
--rw-r--r--   0        0        0     3254 2023-07-28 16:43:03.684957 mkdocs_python_classy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 mkdocs_python_classy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      581 2023-07-28 22:49:04.649912 mkdocs_python_classy-0.1.2/LICENSE
+-rw-r--r--   0        0        0      302 2023-07-28 22:49:04.649912 mkdocs_python_classy-0.1.2/NOTICE
+-rw-r--r--   0        0        0     3997 2023-07-28 22:49:04.649912 mkdocs_python_classy-0.1.2/README.md
+-rw-r--r--   0        0        0     7950 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/constants.py
+-rw-r--r--   0        0        0       32 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/css/classy.css
+-rw-r--r--   0        0        0    13361 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/inspector.py
+-rw-r--r--   0        0        0     6730 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/utils.py
+-rw-r--r--   0        0        0     3254 2023-07-28 22:49:14.693887 mkdocs_python_classy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 mkdocs_python_classy-0.1.2/PKG-INFO
```

### Comparing `mkdocs_python_classy-0.1.1/LICENSE` & `mkdocs_python_classy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_python_classy-0.1.1/README.md` & `mkdocs_python_classy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_python_classy-0.1.1/mkdocs_python_classy/__init__.py` & `mkdocs_python_classy-0.1.2/mkdocs_python_classy/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_python_classy-0.1.1/mkdocs_python_classy/inspector.py` & `mkdocs_python_classy-0.1.2/mkdocs_python_classy/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         self.klass_name = dotted_path.rsplit(".")[0]
         self.module_name = dotted_path.rsplit(".")[1]
         self.dotted_path = dotted_path
 
         self.module_path = self.klasses[self.dotted_path]["module_path"]
         self.subclass_path = self.klasses[self.dotted_path]["subclass_path"]
         self.url = self.klasses[self.dotted_path]["url"]
-        self.other_klasses = {}
+        self.klass_code = {}
 
     def get_klass(self):
         """Load the class."""
         return import_string(self.dotted_path)
 
     def get_page_url(self):
         """Get the url of the class."""
@@ -151,16 +151,16 @@
     def get_klass_mro(self):
         """Get the class inheritance order or MRO."""
         ancestors = []
         for ancestor in self.get_klass().mro():
             if ancestor is object:
                 break
             ancestors.append(ancestor)
-            if not self.other_klasses.get(get_dotted_path(ancestor)):
-                self.other_klasses[get_dotted_path(ancestor)] = get_attribute_code(
+            if not self.klass_code.get(get_dotted_path(ancestor)):
+                self.klass_code[get_dotted_path(ancestor)] = get_attribute_code(
                     import_string(get_dotted_path(ancestor))
                 )
         return ancestors
 
     def get_children(self):
         """Get children."""
         children = []
@@ -176,19 +176,15 @@
     def get_attributes(self):
         """Get the attributes of the class."""
         attrs = Attributes()
         attr_dict = {}
         sorted_dict = {}
 
         for klass in self.get_klass_mro():
-            dotted_path = get_dotted_path(klass)
-            if dotted_path in self.klasses:
-                attr_info = self.klasses[dotted_path]["attr_code"]
-            elif dotted_path in self.other_klasses:
-                attr_info = self.other_klasses[dotted_path]
+            attr_info = self.klass_code[get_dotted_path(klass)]
 
             for attr_str, code in attr_info.items():
                 val = Attribute(
                     name=attr_str, value=attr_str, classobject=klass, instance_class=self.get_klass(), attr_code=code
                 )
                 if not val.attr_code:
                     continue
@@ -301,32 +297,33 @@
         self.klass_short = {}
         for klass in self.klasses:
             self.klass_details[klass] = KlassInspector(self.klasses, klass)
             self.klass_short[klass] = self.klass_details[klass].dotted_path
 
     def get_all_klasses(self):
         """Dynamically find all classes in scope."""
-        for module_str in self.modules_str:
+        for module_str in self.modules_str:  # pylint: disable=too-many-nested-blocks
             module = importlib.import_module(module_str)
             for attr_str in dir(module):
                 attr = getattr(module, attr_str)
                 try:
                     issubclass(attr, (self.base_classes_tuple))
                 except TypeError:
                     continue
                 for base_class in self.base_classes:
                     if issubclass(attr, (base_class[1])) and not attr_str.startswith("_"):
                         if any(attr.__module__.startswith(i) for i in self.libraries):
                             url = self.get_url(module_str, base_class[0], attr.__name__)
-                            self.klasses[get_dotted_path(attr)] = {
-                                "module_path": module_str,
-                                "subclass_path": base_class[0],
-                                "url": url,
-                                "attr_code": get_attribute_code(import_string(get_dotted_path(attr))),
-                            }
+                            if not self.klasses.get(get_dotted_path(attr)):
+                                self.klasses[get_dotted_path(attr)] = {
+                                    "module_path": module_str,
+                                    "subclass_path": base_class[0],
+                                    "url": url,
+                                }
+                            # self.klasses_code[get_dotted_path(attr)] = get_attribute_code(import_string(get_dotted_path(attr)))
                         break
 
     def get_url(self, module_str, base_class_str, name):
         """Toggle the url based on the strategy."""
         if self.strategy == "subclass":
             return self.urls[base_class_str] + f"#{name.lower()}"
         if self.strategy == "module":
```

### Comparing `mkdocs_python_classy-0.1.1/pyproject.toml` & `mkdocs_python_classy-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-python-classy"
-version = "v0.1.1"
+version = "v0.1.2"
 description = "Mkdocs plugin to view Python Classes."
 authors = ["Ken Celenza <ken@celenza.org>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["mkdocs"]
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `mkdocs_python_classy-0.1.1/PKG-INFO` & `mkdocs_python_classy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-python-classy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mkdocs plugin to view Python Classes.
 License: Apache
 Keywords: mkdocs
 Author: Ken Celenza
 Author-email: ken@celenza.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-python-classy Version: 0.1.1 Summary: Mkdocs
+Metadata-Version: 2.1 Name: mkdocs-python-classy Version: 0.1.2 Summary: Mkdocs
 plugin to view Python Classes. License: Apache Keywords: mkdocs Author: Ken
 Celenza Author-email: ken@celenza.org Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

