# Comparing `tmp/totolo-0.1.tar.gz` & `tmp/totolo-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totolo-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "totolo-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `totolo-0.1.tar` & `totolo-0.3.tar`

### file list

```diff
@@ -1,38 +1,46 @@
--rw-r--r--   0        0        0     3073 2023-07-20 23:48:34.395042 totolo-0.1/.gitignore
--rw-r--r--   0        0        0      892 2023-07-20 23:49:12.905042 totolo-0.1/.vscode/launch.json
--rw-r--r--   0        0        0      277 2023-07-21 08:49:08.178933 totolo-0.1/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2023-07-20 23:48:27.105042 totolo-0.1/LICENSE
--rw-r--r--   0        0        0      163 2023-07-20 23:51:46.605041 totolo-0.1/README.md
--rw-r--r--   0        0        0      500 2023-07-24 20:13:53.802434 totolo-0.1/pyproject.toml
--rw-r--r--   0        0        0       19 2023-07-24 20:08:48.822436 totolo-0.1/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-07-21 07:16:17.008968 totolo-0.1/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-07-21 07:17:42.658967 totolo-0.1/tests/data/cycles1.th.txt
--rw-r--r--   0        0        0       47 2023-07-21 07:17:42.658967 totolo-0.1/tests/data/cycles2.th.txt
--rw-r--r--   0        0        0       71 2023-07-21 07:17:42.658967 totolo-0.1/tests/data/cycles3.th.txt
--rw-r--r--   0        0        0   173716 2023-07-21 19:07:30.830223 totolo-0.1/tests/data/film-timeout-top100.st.txt
--rw-r--r--   0        0        0    34632 2023-07-23 17:10:34.367505 totolo-0.1/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
--rw-r--r--   0        0        0    28049 2023-07-23 17:10:34.367505 totolo-0.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
--rw-r--r--   0        0        0    48760 2023-07-23 17:10:34.367505 totolo-0.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
--rw-r--r--   0        0        0  1011578 2023-07-24 15:45:57.955943 totolo-0.1/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
--rw-r--r--   0        0        0    14882 2023-07-24 15:45:57.955943 totolo-0.1/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
--rw-r--r--   0        0        0      428 2023-07-21 19:17:22.740219 totolo-0.1/tests/data/storytree.st.txt
--rw-r--r--   0        0        0  1011579 2023-07-21 08:01:34.098951 totolo-0.1/tests/data/to-2023.07.09.th.txt
--rw-r--r--   0        0        0     2365 2023-07-22 14:49:15.654562 totolo-0.1/tests/data/to-sample-2023.07.09.st.txt
--rw-r--r--   0        0        0      762 2023-07-24 12:25:23.285030 totolo-0.1/tests/test_core.py
--rw-r--r--   0        0        0      110 2023-07-23 05:00:12.081255 totolo-0.1/tests/test_entry.py
--rw-r--r--   0        0        0     6654 2023-07-24 19:01:22.372462 totolo-0.1/tests/test_totolo.py
--rw-r--r--   0        0        0      189 2023-07-24 20:10:13.142435 totolo-0.1/totolo/__init__.py
--rw-r--r--   0        0        0     1247 2023-07-20 23:47:51.775042 totolo-0.1/totolo/api.py
--rw-r--r--   0        0        0        0 2023-07-20 23:47:51.775042 totolo-0.1/totolo/impl/__init__.py
--rw-r--r--   0        0        0     2731 2023-07-24 12:49:05.645021 totolo-0.1/totolo/impl/core.py
--rw-r--r--   0        0        0     3833 2023-07-24 15:22:49.825952 totolo-0.1/totolo/impl/entry.py
--rw-r--r--   0        0        0     3159 2023-07-24 12:22:44.955031 totolo-0.1/totolo/impl/field.py
--rw-r--r--   0        0        0      424 2023-07-23 05:18:38.591248 totolo-0.1/totolo/impl/keyword.py
--rw-r--r--   0        0        0     7980 2023-07-24 14:56:14.935962 totolo-0.1/totolo/impl/parser.py
--rw-r--r--   0        0        0        0 2023-07-20 23:47:51.775042 totolo-0.1/totolo/lib/__init__.py
--rw-r--r--   0        0        0     1192 2023-07-23 16:49:40.777513 totolo-0.1/totolo/lib/files.py
--rw-r--r--   0        0        0     1408 2023-07-20 23:47:51.775042 totolo-0.1/totolo/lib/textformat.py
--rw-r--r--   0        0        0     4242 2023-07-24 15:50:11.265941 totolo-0.1/totolo/story.py
--rw-r--r--   0        0        0     2665 2023-07-24 15:49:59.005942 totolo-0.1/totolo/theme.py
--rw-r--r--   0        0        0     6588 2023-07-24 17:38:55.372493 totolo-0.1/totolo/themeontology.py
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 totolo-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1112 2023-07-29 15:49:20.024088 totolo-0.3/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     1409 2023-07-29 16:47:10.254067 totolo-0.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      854 2023-07-29 15:47:06.414089 totolo-0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3081 2023-07-29 17:17:23.614057 totolo-0.3/.gitignore
+-rw-r--r--   0        0        0      892 2023-07-20 23:49:12.905042 totolo-0.3/.vscode/launch.json
+-rw-r--r--   0        0        0      277 2023-07-21 08:49:08.178933 totolo-0.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2023-07-20 23:48:27.105042 totolo-0.3/LICENSE
+-rw-r--r--   0        0        0      729 2023-07-27 20:44:23.163611 totolo-0.3/README.md
+-rw-r--r--   0        0        0     1259 2023-07-28 19:07:41.098512 totolo-0.3/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-07-26 12:59:05.647420 totolo-0.3/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-07-21 07:16:17.008968 totolo-0.3/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-21 07:17:42.658967 totolo-0.3/tests/data/cycles1.th.txt
+-rw-r--r--   0        0        0       47 2023-07-21 07:17:42.658967 totolo-0.3/tests/data/cycles2.th.txt
+-rw-r--r--   0        0        0       71 2023-07-21 07:17:42.658967 totolo-0.3/tests/data/cycles3.th.txt
+-rw-r--r--   0        0        0   173716 2023-07-21 19:07:30.830223 totolo-0.3/tests/data/film-timeout-top100.st.txt
+-rw-r--r--   0        0        0   332534 2023-07-28 18:29:09.328525 totolo-0.3/tests/data/flat.tar.gz
+-rw-r--r--   0        0        0      166 2023-07-28 14:22:48.076573 totolo-0.3/tests/data/messy.st.txt
+-rw-r--r--   0        0        0   332557 2023-07-27 20:34:04.643615 totolo-0.3/tests/data/sample-2023.07.23.tar.gz
+-rw-r--r--   0        0        0    34632 2023-07-23 17:10:34.367505 totolo-0.3/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
+-rw-r--r--   0        0        0    28050 2023-07-28 11:58:13.902891 totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
+-rw-r--r--   0        0        0    48760 2023-07-23 17:10:34.367505 totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
+-rw-r--r--   0        0        0  1011578 2023-07-24 15:45:57.955943 totolo-0.3/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
+-rw-r--r--   0        0        0    14882 2023-07-24 15:45:57.955943 totolo-0.3/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
+-rw-r--r--   0        0        0      428 2023-07-21 19:17:22.740219 totolo-0.3/tests/data/storytree.st.txt
+-rw-r--r--   0        0        0  1011579 2023-07-21 08:01:34.098951 totolo-0.3/tests/data/to-2023.07.09.th.txt
+-rw-r--r--   0        0        0     2365 2023-07-28 11:18:26.352906 totolo-0.3/tests/data/to-sample-2023.07.09-copy.st.txt
+-rw-r--r--   0        0        0     2365 2023-07-22 14:49:15.654562 totolo-0.3/tests/data/to-sample-2023.07.09.st.txt
+-rw-r--r--   0        0        0     6150 2023-07-28 07:54:27.717457 totolo-0.3/tests/test_entries.py
+-rw-r--r--   0        0        0     5692 2023-07-28 19:02:13.738514 totolo-0.3/tests/test_impl.py
+-rw-r--r--   0        0        0     2219 2023-07-28 18:43:03.928521 totolo-0.3/tests/test_lib.py
+-rw-r--r--   0        0        0    10843 2023-07-28 16:10:26.086532 totolo-0.3/tests/test_totolo.py
+-rw-r--r--   0        0        0      189 2023-07-29 15:22:50.924097 totolo-0.3/totolo/__init__.py
+-rw-r--r--   0        0        0     1201 2023-07-26 18:32:07.507797 totolo-0.3/totolo/api.py
+-rw-r--r--   0        0        0        0 2023-07-20 23:47:51.775042 totolo-0.3/totolo/impl/__init__.py
+-rw-r--r--   0        0        0     2953 2023-07-28 19:02:31.728514 totolo-0.3/totolo/impl/core.py
+-rw-r--r--   0        0        0     5245 2023-07-28 19:57:11.728495 totolo-0.3/totolo/impl/entry.py
+-rw-r--r--   0        0        0     3160 2023-07-28 18:52:24.978517 totolo-0.3/totolo/impl/field.py
+-rw-r--r--   0        0        0      424 2023-07-23 05:18:38.591248 totolo-0.3/totolo/impl/keyword.py
+-rw-r--r--   0        0        0     7567 2023-07-28 19:07:02.088512 totolo-0.3/totolo/impl/parser.py
+-rw-r--r--   0        0        0        0 2023-07-20 23:47:51.775042 totolo-0.3/totolo/lib/__init__.py
+-rw-r--r--   0        0        0     1134 2023-07-28 18:49:06.178518 totolo-0.3/totolo/lib/files.py
+-rw-r--r--   0        0        0     1283 2023-07-28 18:48:39.808519 totolo-0.3/totolo/lib/textformat.py
+-rw-r--r--   0        0        0     3456 2023-07-28 19:56:14.668495 totolo-0.3/totolo/story.py
+-rw-r--r--   0        0        0     2209 2023-07-28 19:56:03.888495 totolo-0.3/totolo/theme.py
+-rw-r--r--   0        0        0     6687 2023-07-28 18:47:09.658519 totolo-0.3/totolo/themeontology.py
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 totolo-0.3/PKG-INFO
```

### Comparing `totolo-0.1/.gitignore` & `totolo-0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -153,7 +153,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+.pypirc
```

### Comparing `totolo-0.1/.vscode/launch.json` & `totolo-0.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `totolo-0.1/LICENSE` & `totolo-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `totolo-0.1/tests/data/film-timeout-top100.st.txt` & `totolo-0.3/tests/data/film-timeout-top100.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.1/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt` & `totolo-0.3/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt` & `totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 :: Title
 Dr. Jekyll and Mr. Hyde
 
 :: Date
 1920-03-28
 
-:: Description
+::  Description
 A 1920 film based on the Robert Louis Stevenson's novel Strange Case of Dr
 Jekyll and Mr Hyde directed and written by J. Charles Haydon.
 
 :: References
 https://en.wikipedia.org/wiki/Dr._Jekyll_and_Mr._Hyde_(1920_Paramount_film)
 
 :: Ratings
```

### Comparing `totolo-0.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt` & `totolo-0.3/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.1/tests/data/sample-2023.07.23/notes/themes/primary.th.txt` & `totolo-0.3/tests/data/sample-2023.07.23/notes/themes/primary.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.1/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt` & `totolo-0.3/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.1/tests/data/to-2023.07.09.th.txt` & `totolo-0.3/tests/data/to-2023.07.09.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.1/tests/data/to-sample-2023.07.09.st.txt` & `totolo-0.3/tests/data/to-sample-2023.07.09-copy.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-0.1/totolo/api.py` & `totolo-0.3/totolo/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,23 +20,21 @@
 class TORemote:
     def __call__(self, url: str = "") -> ThemeOntology:
         if not url:
             url = DEFAULT_URL + "archive/refs/heads/master.tar.gz"
         return TOParser.add_url(empty(), url)
 
     def version(self, version: str = ""):
-        if not version:
-            return self()
         if re.match(r"v\d+\.\d+\.\d+$", version):
             url = DEFAULT_URL + f"archive/refs/tags/{version}.tar.gz"
         elif re.match(r"v20\d{2}\.\d{2}$", version):
             url = DEFAULT_URL + f"archive/refs/tags/{version}.tar.gz"
         else:
             raise ValueError(f"Unknown version format {version}.")
         return self(url)
 
     def versions(self):
         url = API_URL + "releases"
         with urllib.request.urlopen(url) as response:
-            response.read()
-        for item in json.loads(response.read()):
+            contents = response.read()
+        for item in json.loads(contents):
             yield item["tag_name"], item["name"]
```

### Comparing `totolo-0.1/totolo/impl/core.py` & `totolo-0.3/totolo/impl/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,51 +3,59 @@
 
 
 class TOAttr:
     def __init__(self, default="", private=False):
         self.default = default
         self.private = private
 
+    def __str__(self):
+        tname = self.__class__.__name__
+        return f"{tname}({self.default})"
+
 
 class TOStoredAttr(TOAttr):
     def __init__(self, datatype="blob", default=None, required=False):
         if default is None:
             default = [] if "list" in datatype else ""
         super().__init__(default, True)
         self.datatype = datatype
         self.required = required
 
+    def __str__(self):
+        tname = self.__class__.__name__
+        return f"{tname}<{self.datatype}>({self.default})"
+
 
 class TOObjectMeta(type):
-    def __new__(meta, name, bases, attr):
+    def __new__(mcs, name, bases, attr):
         to_attrs = OrderedDict()
         for base in bases:
             for key, value in getattr(base, "_to_attrs", {}).items():
                 if key not in attr:
                     to_attrs[key] = value
         for key, value in list(attr.items()):
             if isinstance(value, TOStoredAttr):
                 nkey = key.replace("_", " ")
                 to_attrs[nkey] = value
                 del attr[key]
             elif isinstance(value, TOAttr):
                 to_attrs[key] = value
                 del attr[key]
         attr["_to_attrs"] = to_attrs
-        return super().__new__(meta, name, bases, attr)
+        return super().__new__(mcs, name, bases, attr)
 
     def __call__(cls, *args, **kwargs):
         self = super().__call__(*args, **kwargs)
         for key, value in self._to_attrs.items():
             if not value.private and not hasattr(self, key):
                 setattr(self, key, deepcopy(value.default))
         return self
 
     @classmethod
-    def __prepare__(mcls, _cls, _bases):
+    def __prepare__(mcs, _cls, _bases):
         return OrderedDict()
 
 
 def a(*args, **kwargs):
     return TOAttr(*args, **kwargs)
 
 
@@ -77,16 +85,16 @@
         try:
             return self.get_attr(key).datatype
         except (KeyError, AttributeError) as _e:
             return "unknown"
 
     def field_required(self, key):
         try:
-            return self.get_attr(key).datatype
+            return self.get_attr(key).required
         except (KeyError, AttributeError) as _e:
-            return "unknown"
+            return False
 
     def __str__(self):
         return "[TOObject]"
 
     def __repr__(self):
         return f'{type(self).__name__}<{str(self)}>'
```

### Comparing `totolo-0.1/totolo/impl/entry.py` & `totolo-0.3/totolo/impl/entry.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,26 +7,46 @@
 class TOEntry(TOObject):
     name = a("")
     fields = a(OrderedDict())
     parents = a(set())
     children = a(set())
     source = a([])
     source_location = a("<api>)")
-    ontology = a()
+    ontology = a(lambda: None)
+
+    def __lt__(self, other):
+        return str(self) < str(other)
+
+    def __hash__(self):
+        return hash(self.name)
 
     def __str__(self):
-        return "{}[{}]".format(
-            self.name.encode("ascii", "ignore"),
-            len(self.fields)
-        )
+        name = self.name.encode("ascii", "ignore")
+        return f"{name}[{len(self.fields)}]"
 
     def __getitem__(self, key):
         return self.get(key)
 
     def __setitem__(self, key, value):
+        if isinstance(value, list):
+            value = TOField(
+                name=key,
+                fieldtype="list",
+                source=value,
+                data=value,
+                parts=value
+            )
+        elif not isinstance(value, TOField):
+            data = str(value)
+            value = TOField(
+                name=key,
+                fieldtype="blob",
+                source=[data],
+                data=[data],
+                parts=[data])
         self.fields[key] = value
 
     def __delitem__(self, key):
         del self.fields[key]
 
     def iter_fields(self, reorder=False, skipunknown=False):
         if reorder:
@@ -48,15 +68,15 @@
 
     def validate(self):
         junklines = []
         for idx, line in enumerate(self.source):
             if idx > 1:
                 if line.startswith("::"):
                     break
-                elif line.strip():
+                if line.strip():
                     junklines.append(line)
         if junklines:
             junkmsg = '/'.join(junklines)
             if len(junkmsg) > 13:
                 junkmsg = junkmsg[:10] + "..."
             yield f"{self.name}: junk in entry header: {junkmsg}"
         for field in self.fields.values():
@@ -70,16 +90,15 @@
                 lines.append(field.text_canonical())
                 lines.append("")
         return "\n".join(lines)
 
     def text_original(self):
         lines = [self.name, "=" * len(self.name), ""]
         for field in self.iter_fields(reorder=False, skipunknown=False):
-            lines.append(field.text_canonical())
-            lines.append("")
+            lines.append(field.text_original())
         return "\n".join(lines)
 
     def get(self, fieldname):
         """Get field, returning a frozen default field if it doesn't exist."""
         field = self.fields.get(fieldname, None)
         if field is not None:
             return field
@@ -109,12 +128,35 @@
     def _dfs(self, attr, lookup):
         visited = set()
         pending = [self.name]
         visited.update(pending)
         while pending:
             name = pending.pop()
             yield name
-            item = lookup[name]
-            for nitem in getattr(item, attr):
-                if nitem not in visited:
-                    pending.append(nitem)
-                    visited.add(nitem)
+            item = lookup.get(name, None)
+            if item is not None:
+                for nitem in getattr(item, attr):
+                    if nitem not in visited:
+                        pending.append(nitem)
+                        visited.add(nitem)
+
+    @staticmethod
+    def html_references_(references_text):
+        description = [
+            '<P class="obj-description"><b>References:</b><BR>'
+        ]
+        reflines = [line.strip() for line in references_text.split("\n")]
+        reflines = [x for x in reflines if x]
+        for line in reflines:
+            aline = f'<A href="{line}">{line}</A>'
+            description.append(aline)
+        description.append("</P>\n")
+        return "\n".join(description)
+
+    @staticmethod
+    def references_(references_text):
+        description = ["References:"]
+        reflines = [line.strip() for line in references_text.split("\n")]
+        reflines = [x for x in reflines if x]
+        for line in reflines:
+            description.append(line)
+        return "\n".join(description)
```

### Comparing `totolo-0.1/totolo/impl/field.py` & `totolo-0.3/totolo/impl/field.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 
     def __setattr__(self, name, value):
         if name != "frozen":
             self.assert_mutable()
         super().__setattr__(name, value)
 
     def __repr__(self):
-        return "{}<{}>[{}]".format(
-            type(self).__name__,
-            self.name.encode("ascii", "ignore"),
-            len(self.data)
-        )
+        tname = type(self).__name__
+        name = self.name.encode("ascii", "ignore")
+        ndata = len(self.data)
+        return f"{tname}<{name}>[{ndata}]"
 
     def __str__(self):
         return self.text_canonical_contents()
 
     def __iter__(self):
         for part in self.iter_parts():
             yield part
@@ -46,58 +45,59 @@
     def str(self):
         return str(self)
 
     def list(self):
         return list(self.parts)
 
     def empty(self):
-        return any(self.parts)
+        return not any(self.parts)
 
     def iter_parts(self):
         for part in self.parts:
             yield part
 
     def text_canonical_contents(self):
         parts = [str(x) for x in self.iter_parts()]
         return "\n".join(parts)
 
     def text_canonical(self):
         parts = [f":: {self.name}"]
         parts.extend(str(x) for x in self.iter_parts())
         return "\n".join(parts)
 
-    def delete_kw(self, kw):
-        """Delete a keyword."""
+    def text_original(self):
+        return "\n".join(self.source)
+
+    def delete_kw(self, keyword):
         self.assert_mutable()
         fieldtype = self.fieldtype
         todelete = set()
         if fieldtype == "kwlist":
             for idx, part in enumerate(self.parts):
-                if part.keyword == kw:
+                if part.keyword == keyword:
                     todelete.add(idx)
         self.parts = [p for idx, p in enumerate(self.parts) if idx not in todelete]
-        return min(todelete) if todelete else len(self.parts)
+        return len(todelete)
 
-    def update_kw(self, kw, keyword=None, motivation=None, capacity=None, notes=None):
-        """Edit a keyword."""
+    def update_kw(self, match_keyword, keyword=None,
+                  motivation=None, capacity=None, notes=None):
         self.assert_mutable()
         assert self.fieldtype == "kwlist"
         for part in self.parts:
-            if part.keyword == kw:
+            if part.keyword == match_keyword:
                 if keyword is not None:
                     part.keyword = keyword
                 if motivation is not None:
                     part.motivation = motivation
                 if capacity is not None:
                     part.capacity = capacity
                 if notes is not None:
                     part.notes = notes
 
     def insert_kw(self, idx=None, keyword="", motivation="", capacity="", notes=""):
-        """Insert a keyword."""
         self.assert_mutable()
         assert self.fieldtype == "kwlist"
         if idx is None:
             idx = len(self.parts)
         self.parts.insert(
             idx,
             TOKeyword(
```

### Comparing `totolo-0.1/totolo/impl/parser.py` & `totolo-0.3/totolo/impl/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,68 +85,56 @@
             if part in delcorr:
                 state = part
             elif part in delcorr.values():
                 if delcorr.get(state, None) == part:
                     state = ""
                 else:
                     raise AssertionError(
-                        "Malformed field (bracket mismatch):\n  %s" % field
+                        f"Malformed field (bracket mismatch):\n {field}"
                     )
             elif part in splitters and not state:
                 tokrow = dict2row(token)
                 if not tokrow[0].strip():
                     pass  # we allow splitting by both newline and comma
                 else:
                     yield tokrow
                 token = {}
             else:
                 token[state] = token.get(state, "") + part
 
-        tokrow = dict2row(token)
-        if tokrow[0].strip():
-            yield dict2row(token)
-
     @classmethod
     def make_field(cls, lines, fieldtype):
         field = TOField(
             fieldtype=fieldtype,
             name=lines[0].strip(": "),
-            data=lines[1:],
+            data=[line.strip() for line in lines[1:] if line.strip()],
             source=list(lines),
         )
         if fieldtype == "kwlist":
             for kwtuple in TOParser.iter_kwitems(field.data):
                 field.parts.append(TOKeyword(*kwtuple))
         elif fieldtype == "list":
             for item in TOParser.iter_listitems(field.data):
                 field.parts.append(item)
         elif fieldtype == "text":
             field.parts.append(
                 totolo.lib.textformat.add_wordwrap(
-                    "\n".join(
-                        field.data)).strip())
-        else:
+                    "\n".join(field.data)).strip()
+            )
+        else:  # date/ blob
             field.parts.append('\n'.join(field.data))
         return field
 
     @classmethod
     def populate_entry(cls, entry, lines):
         entry.source.extend(lines)
-        cleaned = []
-        for line in lines:
-            cline = line.strip()
-            if cline or (cleaned and cleaned[-1]):
-                cleaned.append(cline)  # no more than one blank line in a row
+        cleaned = [line.strip() for line in lines]
         assert len(cleaned) > 1 and cleaned[1].startswith("==="), "missing name"
-        while cleaned and not cleaned[-1]:
-            cleaned.pop()
         entry.name = cleaned[0]
         for fieldlines in cls.iter_fields(cleaned):
-            while fieldlines and not fieldlines[-1]:
-                fieldlines.pop()
             name = fieldlines[0].strip(": ")
             fieldtype = entry.field_type(name)
             field = cls.make_field(fieldlines, fieldtype)
             entry[field.name] = field
         return entry
 
     @classmethod
@@ -159,16 +147,14 @@
         theme = cls.populate_entry(TOTheme(), lines)
         return theme
 
     @classmethod
     def parse_stories(cls, lines):
         collection_entry = None
         entries = []
-        if isinstance(lines, str):
-            lines = lines.splitlines()
         for idx, entrylines in enumerate(TOParser.iter_entries(lines)):
             entry = cls.make_story(entrylines)
             if idx == 0:
                 mycols = entry.get("Collections").parts
                 if mycols and mycols[0] == entry.sid:
                     collection_entry = entry
             if idx > 0 and collection_entry:
@@ -176,55 +162,53 @@
                 field.parts.append(entry.sid)
             entries.append(entry)
         return entries
 
     @classmethod
     def parse_themes(cls, lines):
         entries = []
-        if isinstance(lines, str):
-            lines = lines.splitlines()
         for _idx, entrylines in enumerate(TOParser.iter_entries(lines)):
             entry = cls.make_theme(entrylines)
             entries.append(entry)
         return entries
 
     @classmethod
-    def add_url(cls, to, url):
+    def add_url(cls, ontology, url):
         suffixes = [".tar", ".tar.gz"]
         if any(url.endswith(x) for x in suffixes):
             with totolo.lib.files.remote_tar(url) as dirname:
-                cls.add_files(to, dirname)
+                cls.add_files(ontology, dirname)
         else:
             raise ValueError(f"Expected url ending in one of {suffixes}")
-        return to
+        return ontology
 
     @classmethod
-    def add_files(cls, to, paths):
+    def add_files(cls, ontology, paths):
         if isinstance(paths, str):
             paths = [paths]
         for path in paths:
-            to.basepaths.add(path)
+            ontology.basepaths.add(path)
             if os.path.isdir(path):
                 for filepath in totolo.lib.files.walk(path, r".*\.(st|th)\.txt$"):
-                    cls._add_file(to, filepath)
+                    cls._add_file(ontology, filepath)
             else:
-                cls._add_file(to, path)
-        return to.refresh_relations()
+                cls._add_file(ontology, path)
+        return ontology.refresh_relations()
 
     @classmethod
-    def _add_file(cls, to, path):
+    def _add_file(cls, ontology, path):
         target = {}
-        with open(path, "r", encoding='utf-8') as fh:
+        with open(path, "r", encoding='utf-8') as fhandle:
             entry_iterable = []
             if path.endswith(".th.txt"):
-                entry_iterable = cls.parse_themes(fh)
-                target = to.theme
+                entry_iterable = cls.parse_themes(fhandle)
+                target = ontology.theme
             elif path.endswith(".st.txt"):
-                entry_iterable = cls.parse_stories(fh)
-                target = to.story
+                entry_iterable = cls.parse_stories(fhandle)
+                target = ontology.story
             for entry in entry_iterable:
                 entry.source_location = path
-                entry.ontology = weakref.ref(to)
-                to.entries.setdefault(path, [])
-                to.entries[path].append(entry)
+                entry.ontology = weakref.ref(ontology)
+                ontology.entries.setdefault(path, [])
+                ontology.entries[path].append(entry)
                 target[entry.name] = entry
-        return to
+        return ontology
```

### Comparing `totolo-0.1/totolo/lib/files.py` & `totolo-0.3/totolo/lib/files.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,20 +19,19 @@
         if len(paths) == 1 and os.path.isdir(paths[0]):
             yield paths[0]
         else:
             yield dirname
 
 
 def walk(path: str, pattern: str = ".*", levels: int = -1):
-    r = re.compile(pattern)
-    # yield matching files
+    regex = re.compile(pattern)
+
     for item in os.listdir(path):
         spath = os.path.join(path, item)
-        if r.match(item):
+        if regex.match(item):
             if os.path.isfile(spath):
                 yield spath
-    # recurse
+
     for item in os.listdir(path):
         spath = os.path.join(path, item)
         if os.path.isdir(spath) and levels != 0:
-            for res in walk(spath, pattern, levels - 1):
-                yield res
+            yield from walk(spath, pattern, levels - 1)
```

### Comparing `totolo-0.1/totolo/lib/textformat.py` & `totolo-0.3/totolo/lib/textformat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import textwrap
 
 
 def remove_wordwrap(text):
     """
-    Remove single newline characters (i.e. '\n') from string, but leave double newlines (i.e. '\n\n').
-    Args:
-        text: string
-    Returns: string
+    Remove single newline characters (i.e. '\n') from string, but leave double
+    newlines (i.e. '\n\n').
     """
     text_blocks = text.split("\n")
     dewordwraped_text_block = []
     dewordwraped_text_blocks = []
 
     for text_block in text_blocks:
         text_block = text_block.strip()
@@ -23,22 +21,19 @@
             dewordwraped_text_block.append(text_block)
 
     if dewordwraped_text_block:
         dewordwraped_text_blocks.append(" ".join(dewordwraped_text_block))
 
     return "\n\n".join(dewordwraped_text_blocks)
 
+
 def add_wordwrap(text, wrap_length=78):
     """
-    Add line breaks to string (i.e. '\n' character) so that each line is at most 'wrap_length'
-    characters in length.
-    Args:
-        text: string
-        wrap_length: integer
-    Returns: string
+    Add line breaks to string (i.e. '\\n' character) so that each line is at
+    most 'wrap_length' characters in length.
     """
     paragraphs = remove_wordwrap(text)
     wordwrapped_lines = []
 
     for paragraph in paragraphs.split("\n\n"):
         for wordwrapped_line in textwrap.fill(paragraph, wrap_length).split("\n"):
             wordwrapped_lines.append(wordwrapped_line.strip())
```

### Comparing `totolo-0.1/totolo/story.py` & `totolo-0.3/totolo/story.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import html
 import re
 
 from .impl.core import sa
 from .impl.entry import TOEntry
 
 
 class TOStory(TOEntry):
@@ -32,20 +33,20 @@
                 for part in field.iter_parts():
                     yield weight, part
 
     def iter_themes(self):
         """
         Iterate over the theme objects associated with this story object.
         """
-        if not getattr(self, "ontology", None):
+        ontology = self.ontology()
+        if ontology is None:
             raise RuntimeError(
                 "Story must be associated with an ontology to look up themes.")
-        to = self.ontology()
         for weight, part in self.iter_theme_entries():
-            theme = to.theme[part.keyword]
+            theme = ontology.theme[part.keyword]
             yield weight, theme
 
     @property
     def date(self):
         """
         Return the date entry as verbatim it is recorded in the text file.
         """
@@ -76,52 +77,30 @@
         return self.name
 
     @property
     def title(self):
         return self.get("Title").text_canonical_contents().strip()
 
     def verbose_description(self):
-        """
-        A description that combines various other fields, including Notes, Examples,
-        Aliases, and References.
-        """
         description = str(self.get("Description"))
         references = str(self.get("References")).strip()
         if references:
-            description += "\n\nReferences:\n"
-            for line in references.split("\n"):
-                line = line.strip()
-                if line:
-                    description += line + "\n"
+            description += self.references_(references)
         return description
 
     def html_description(self):
-        """
-        Turn the verbose description into html.
-        """
-        import html
         description = html.escape(str(self.get("Description")))
         references = html.escape(str(self.get("References")).strip())
         description = '<P class="obj-description"><BR>\n' + description
         description += "</P>\n"
         if references:
-            description += '<P class="obj-description"><b>References:</b><BR>\n'
-            for line in references.split("\n"):
-                line = line.strip()
-                if line:
-                    aline = '<A href="{}">{}</A>'.format(line, line)
-                    description += aline + "\n"
-            description += "</P>\n"
+            description += self.html_references_(references)
         return description
 
     def html_short_description(self):
-        """
-        A limited length short description without embelishments like "references".
-        """
-        import html
         description = str(self.get("Description"))[:256]
         return html.escape(description)
 
     def _lookup(self):
         try:
             return self.ontology().story
         except AttributeError:
```

### Comparing `totolo-0.1/totolo/theme.py` & `totolo-0.3/totolo/theme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import html
+
 from .impl.core import sa
 from .impl.entry import TOEntry
 
 
 class TOTheme(TOEntry):
     Description = sa("text", required=True)
     Parents = sa("list")
@@ -19,23 +21,22 @@
         if notes:
             description += "\n\nNotes:\n" + notes
         if examples:
             description += "\n\nExamples:\n" + examples
         if aliases:
             description += "\n\nAliases:\n" + aliases
         if references:
-            description += "\n\nReferences:\n"
-            for line in references.split("\n"):
-                line = line.strip()
-                if line:
-                    description += line + "\n"
+            description += self.references_(references)
         return description
 
+    def html_short_description(self):
+        description = str(self.get("Description"))[:256]
+        return html.escape(description)
+
     def html_description(self):
-        import html
         description = html.escape(str(self.get("Description")))
         examples = html.escape(str(self.get("Examples")).strip())
         aliases = html.escape(str(self.get("Aliases")).strip())
         notes = html.escape(str(self.get("Notes")).strip())
         references = html.escape(str(self.get("References")).strip())
         description = '<P class="obj-description"><BR>\n' + description
         description += "</P>\n"
@@ -46,26 +47,15 @@
             description += '<P class="obj-description"><b>Examples:</b><BR>\n' + examples
             description += "</P>\n"
         if aliases:
             aliases = ', '.join(aliases.split("\n"))
             description += '<P class="obj-description"><b>Aliases:</b><BR>\n' + aliases
             description += "</P>\n"
         if references:
-            description += '<P class="obj-description"><b>References:</b><BR>\n'
-            for line in references.split("\n"):
-                line = line.strip()
-                if line:
-                    aline = '<A href="{}">{}</A>'.format(line, line)
-                    description += aline + "\n"
-            description += "</P>\n"
+            description += self.html_references_(references)
         return description
 
-    def html_short_description(self):
-        import html
-        description = str(self.get("Description"))[:256]
-        return html.escape(description)
-
     def _lookup(self):
         try:
             return self.ontology().theme
         except AttributeError:
             return {}
```

### Comparing `totolo-0.1/totolo/themeontology.py` & `totolo-0.3/totolo/themeontology.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,21 @@
             yield story
 
     def themes(self):
         for theme in self.theme.values():
             yield theme
 
     def astory(self):
-        return random.sample(self.story.values(), 1)[0]
+        return random.sample(list(self.story.values()), 1)[0]
 
     def atheme(self):
-        return random.sample(self.theme.values(), 1)[0]
+        return random.sample(list(self.theme.values()), 1)[0]
 
     def dataframe(self, implied_themes=True):
-        import pandas as pd
+        import pandas as pd  # pylint: disable=C0415
         data = []
         for story in self.stories():
             for weight, part in story.iter_theme_entries():
                 themes = [part.keyword]
                 if implied_themes and part.keyword in self.theme:
                     theme = self.theme[part.keyword]
                     themes.extend(theme.ancestors())
@@ -59,58 +59,59 @@
         """Validate basic format of theme and story entries."""
         lookup = defaultdict(dict)
         for path, entries in self.entries.items():
             for entry in entries:
                 for warning in entry.validate():
                     yield f"{path}: {warning}"
                 if entry.name in lookup[type(entry)]:
-                    yield f"{path}: Multiple {type(entry)} with name '{entry.name}'"
+                    tname = type(entry).__name__
+                    yield f"{path}: Multiple {tname} with name '{entry.name}'"
+                lookup[type(entry)][entry.name] = path
 
     def validate_storythemes(self):
         """Detect undefined themes used in stories."""
         for story in self.stories():
             for weight in ["choice", "major", "minor", "not"]:
                 field = f"{weight.capitalize()} Themes"
-                for kwf in story.get(field):
-                    if kwf.keyword not in self.theme:
-                        name, kw = story.name, kwf.keyword
-                        yield f"{name}: Undefined '{weight} theme' with name '{kw}'"
+                for kwfield in story.get(field):
+                    if kwfield.keyword not in self.theme:
+                        yield (f"{story.name}: Undefined '{weight} theme' with "
+                               f"name '{kwfield.keyword}'")
 
     def validate_cycles(self):
         """Detect cycles (stops after first cycle encountered)."""
         parents = {}
         for theme in self.themes():
-            parents[theme.name] = [parent for parent in theme.get("Parents")]
+            parents[theme.name] = list(theme.get("Parents"))
 
         def dfs(current, tpath=None):
             tpath = tpath or []
             if current in tpath:
                 cycle = tpath[tpath.index(current):]
                 return f"Cycle: {cycle}"
-            else:
-                tpath.append(current)
-                for parent in parents[current]:
-                    msg = dfs(parent, tpath)
-                    if msg:
-                        return msg
-                tpath.pop()
+            tpath.append(current)
+            for parent in parents[current]:
+                msg = dfs(parent, tpath)
+                if msg:
+                    return msg
+            tpath.pop()
             return None
 
         for theme in self.themes():
             msg = dfs(theme.name)
             if msg:
                 yield msg
                 break
 
-    def write_clean(self, verbose=False):
+    def write_clean(self):
         """
         Write the ontology back to its source file while cleaning up syntax and
         omitting unknown field names.
         """
-        self.write(verbose=verbose)
+        self.write(cleaned=True)
 
     def write(self, prefix=None, cleaned=False, verbose=False):
         old_prefix = "" if prefix is None else os.path.commonpath(self.basepaths)
         for path, entries in self.entries.items():
             if prefix is not None:
                 rel_path = os.path.relpath(path, old_prefix)
                 path = os.path.join(prefix, rel_path)
@@ -157,23 +158,23 @@
         return self
 
     def _writefile(self, path, entries, cleaned):
         cskey = "Component Stories"
         dirname = os.path.dirname(path)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
-        with open(path, "w", encoding='utf-8') as fh:
+        with open(path, "w", encoding='utf-8') as fhandle:
             sids = set(e.name for e in entries)
             for idx, entry in enumerate(entries):
                 if idx == 0 and entry.name in entry["Collections"]:
                     field = entry.get(cskey)
                     parts = [x for x in field.parts if x not in sids]
                     if parts != field.parts:
                         entry = copy.deepcopy(entry)
                         if parts:
                             field = entry.setdefault(cskey)
                             field.parts = parts
                         else:
                             entry.delete(cskey)
                 lines = entry.text_canonical() if cleaned else entry.text_original()
-                fh.write(lines)
-                fh.write("\n\n")
+                fhandle.write(lines)
+                fhandle.write("\n\n" if cleaned else "\n")
```

