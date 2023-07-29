# Comparing `tmp/soagen-0.0.1.tar.gz` & `tmp/soagen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soagen-0.0.1.tar", last modified: Thu Jul 20 13:57:32 2023, max compression
+gzip compressed data, was "soagen-0.1.0.tar", last modified: Sat Jul 29 16:41:39 2023, max compression
```

## Comparing `soagen-0.0.1.tar` & `soagen-0.1.0.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 13:57:32.240716 soagen-0.0.1/
--rw-rw-rw-   0        0        0       54 2023-07-15 09:44:20.000000 soagen-0.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2023-07-15 09:44:20.000000 soagen-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3252 2023-07-20 13:57:32.239716 soagen-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2377 2023-07-20 10:44:09.000000 soagen-0.0.1/README.md
--rw-rw-rw-   0        0        0     1644 2023-07-20 13:47:36.000000 soagen-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 13:57:32.240716 soagen-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-20 13:57:32.198717 soagen-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 13:57:32.220716 soagen-0.0.1/src/soagen/
--rw-rw-rw-   0        0        0      438 2023-07-20 13:06:50.000000 soagen-0.0.1/src/soagen/__init__.py
--rw-rw-rw-   0        0        0      851 2023-07-20 10:58:18.000000 soagen-0.0.1/src/soagen/column.py
--rw-rw-rw-   0        0        0     6073 2023-07-20 10:58:42.000000 soagen-0.0.1/src/soagen/config.py
--rw-rw-rw-   0        0        0     2762 2023-07-20 11:07:15.000000 soagen-0.0.1/src/soagen/configurable.py
--rw-rw-rw-   0        0        0      596 2023-07-16 22:02:35.000000 soagen-0.0.1/src/soagen/errors.py
--rw-rw-rw-   0        0        0     5669 2023-07-20 10:57:55.000000 soagen-0.0.1/src/soagen/header_file.py
-drwxrwxrwx   0        0        0        0 2023-07-20 13:57:32.239716 soagen-0.0.1/src/soagen/hpp/
--rw-rw-rw-   0        0        0     5571 2023-07-20 13:33:03.000000 soagen-0.0.1/src/soagen/hpp/.clang-format
--rw-rw-rw-   0        0        0     8122 2023-07-19 07:09:11.000000 soagen-0.0.1/src/soagen/hpp/allocator.hpp
--rw-rw-rw-   0        0        0    24020 2023-07-19 07:09:11.000000 soagen-0.0.1/src/soagen/hpp/column_traits.hpp
--rw-rw-rw-   0        0        0     9823 2023-07-20 13:32:48.000000 soagen-0.0.1/src/soagen/hpp/compressed_pair.hpp
--rw-rw-rw-   0        0        0     2495 2023-07-20 13:32:48.000000 soagen-0.0.1/src/soagen/hpp/core.hpp
--rw-rw-rw-   0        0        0     5487 2023-07-20 13:32:49.000000 soagen-0.0.1/src/soagen/hpp/functions.hpp
--rw-rw-rw-   0        0        0      806 2023-07-15 09:44:20.000000 soagen-0.0.1/src/soagen/hpp/header_end.hpp
--rw-rw-rw-   0        0        0      919 2023-07-15 09:44:20.000000 soagen-0.0.1/src/soagen/hpp/header_start.hpp
--rw-rw-rw-   0        0        0      308 2023-07-15 09:44:20.000000 soagen-0.0.1/src/soagen/hpp/meson.build
--rw-rw-rw-   0        0        0     8032 2023-07-19 05:35:16.000000 soagen-0.0.1/src/soagen/hpp/meta.hpp
--rw-rw-rw-   0        0        0    42894 2023-07-20 13:32:51.000000 soagen-0.0.1/src/soagen/hpp/preprocessor.hpp
--rw-rw-rw-   0        0        0   171169 2023-07-20 13:33:03.000000 soagen-0.0.1/src/soagen/hpp/soagen.hpp
--rw-rw-rw-   0        0        0    37916 2023-07-20 13:54:56.000000 soagen-0.0.1/src/soagen/hpp/table.hpp
--rw-rw-rw-   0        0        0    26762 2023-07-19 07:09:11.000000 soagen-0.0.1/src/soagen/hpp/table_traits.hpp
--rw-rw-rw-   0        0        0      421 2023-07-20 13:32:48.000000 soagen-0.0.1/src/soagen/hpp/version.hpp
--rw-rw-rw-   0        0        0    13223 2023-07-20 10:49:11.000000 soagen-0.0.1/src/soagen/includes.py
--rw-rw-rw-   0        0        0     1005 2023-07-15 09:44:20.000000 soagen-0.0.1/src/soagen/injectors.py
--rw-rw-rw-   0        0        0     3391 2023-07-20 10:49:11.000000 soagen-0.0.1/src/soagen/log.py
--rw-rw-rw-   0        0        0    13285 2023-07-20 13:50:10.000000 soagen-0.0.1/src/soagen/main.py
--rw-rw-rw-   0        0        0      282 2023-07-20 12:43:15.000000 soagen-0.0.1/src/soagen/meson.build
--rw-rw-rw-   0        0        0     2596 2023-07-15 09:44:20.000000 soagen-0.0.1/src/soagen/metavars.py
--rw-rw-rw-   0        0        0     3094 2023-07-20 11:00:38.000000 soagen-0.0.1/src/soagen/natvis_file.py
--rw-rw-rw-   0        0        0     1478 2023-07-20 13:32:46.000000 soagen-0.0.1/src/soagen/paths.py
--rw-rw-rw-   0        0        0     4711 2023-07-15 09:44:20.000000 soagen-0.0.1/src/soagen/preprocessor.py
--rw-rw-rw-   0        0        0     2225 2023-07-16 22:02:37.000000 soagen-0.0.1/src/soagen/schemas.py
--rw-rw-rw-   0        0        0    23985 2023-07-20 10:58:23.000000 soagen-0.0.1/src/soagen/struct.py
--rw-rw-rw-   0        0        0     1837 2023-07-15 09:44:20.000000 soagen-0.0.1/src/soagen/type_list.py
--rw-rw-rw-   0        0        0     2095 2023-07-20 13:32:17.000000 soagen-0.0.1/src/soagen/utils.py
--rw-rw-rw-   0        0        0     5198 2023-07-20 10:49:14.000000 soagen-0.0.1/src/soagen/variable.py
--rw-rw-rw-   0        0        0      569 2023-07-20 13:06:07.000000 soagen-0.0.1/src/soagen/version.py
--rw-rw-rw-   0        0        0        6 2023-07-20 13:27:06.000000 soagen-0.0.1/src/soagen/version.txt
--rw-rw-rw-   0        0        0     8766 2023-07-20 10:49:15.000000 soagen-0.0.1/src/soagen/writer.py
-drwxrwxrwx   0        0        0        0 2023-07-20 13:57:32.227718 soagen-0.0.1/src/soagen.egg-info/
--rw-rw-rw-   0        0        0     3252 2023-07-20 13:57:32.000000 soagen-0.0.1/src/soagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2023-07-20 13:57:32.000000 soagen-0.0.1/src/soagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 13:57:32.000000 soagen-0.0.1/src/soagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-20 13:57:32.000000 soagen-0.0.1/src/soagen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-20 13:57:32.000000 soagen-0.0.1/src/soagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 13:57:32.000000 soagen-0.0.1/src/soagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 13:16:09.000000 soagen-0.0.1/src/soagen.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.449712 soagen-0.1.0/
+-rw-rw-rw-   0        0        0       62 2023-07-29 16:31:26.000000 soagen-0.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1372 2023-07-29 16:41:39.448713 soagen-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-07-29 16:32:13.000000 soagen-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:41:39.449712 soagen-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.404713 soagen-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.426712 soagen-0.1.0/src/soagen/
+-rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/__init__.py
+-rw-rw-rw-   0        0        0      918 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/column.py
+-rw-rw-rw-   0        0        0     5040 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/config.py
+-rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/configurable.py
+-rw-rw-rw-   0        0        0    19105 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/cpp.py
+-rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/errors.py
+-rw-rw-rw-   0        0        0    10934 2023-07-29 16:23:15.000000 soagen-0.1.0/src/soagen/header_file.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.442713 soagen-0.1.0/src/soagen/hpp/
+-rw-rw-rw-   0        0        0     5621 2023-07-29 16:38:51.000000 soagen-0.1.0/src/soagen/hpp/.clang-format
+-rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/allocator.hpp
+-rw-rw-rw-   0        0        0    31723 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/column_traits.hpp
+drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.446713 soagen-0.1.0/src/soagen/hpp/generated/
+-rw-rw-rw-   0        0        0     9857 2023-07-29 16:38:30.000000 soagen-0.1.0/src/soagen/hpp/generated/compressed_pair.hpp
+-rw-rw-rw-   0        0        0     2935 2023-07-29 16:38:30.000000 soagen-0.1.0/src/soagen/hpp/generated/core.hpp
+-rw-rw-rw-   0        0        0     7897 2023-07-29 16:38:31.000000 soagen-0.1.0/src/soagen/hpp/generated/functions.hpp
+-rw-rw-rw-   0        0        0    43678 2023-07-29 16:38:32.000000 soagen-0.1.0/src/soagen/hpp/generated/preprocessor.hpp
+-rw-rw-rw-   0        0        0      421 2023-07-29 16:38:30.000000 soagen-0.1.0/src/soagen/hpp/generated/version.hpp
+-rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/header_end.hpp
+-rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/header_start.hpp
+-rw-rw-rw-   0        0        0    15165 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/iterator.hpp
+-rw-rw-rw-   0        0        0    24779 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/meta.hpp
+-rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/mixins.hpp
+-rw-rw-rw-   0        0        0     7272 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/row.hpp
+drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.447713 soagen-0.1.0/src/soagen/hpp/single/
+-rw-rw-rw-   0        0        0   234341 2023-07-29 16:38:50.000000 soagen-0.1.0/src/soagen/hpp/single/soagen.hpp
+-rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/soagen.hpp
+-rw-rw-rw-   0        0        0    53309 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/table.hpp
+-rw-rw-rw-   0        0        0    41432 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/table_traits.hpp
+-rw-rw-rw-   0        0        0     1103 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/injectors.py
+-rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/log.py
+-rw-rw-rw-   0        0        0    21973 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/main.py
+-rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/metavars.py
+-rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/natvis_file.py
+-rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/paths.py
+-rw-rw-rw-   0        0        0     5464 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/preprocessor.py
+-rw-rw-rw-   0        0        0     2494 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/schemas.py
+-rw-rw-rw-   0        0        0    66861 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/struct.py
+-rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/type_list.py
+-rw-rw-rw-   0        0        0     2697 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/utils.py
+-rw-rw-rw-   0        0        0     3782 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/variable.py
+-rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/version.py
+-rw-rw-rw-   0        0        0        6 2023-07-29 16:20:11.000000 soagen-0.1.0/src/soagen/version.txt
+-rw-rw-rw-   0        0        0    12323 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/writer.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.433713 soagen-0.1.0/src/soagen.egg-info/
+-rw-rw-rw-   0        0        0     1372 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1364 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.1.0/src/soagen.egg-info/zip-safe
```

### Comparing `soagen-0.0.1/LICENSE.txt` & `soagen-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soagen-0.0.1/pyproject.toml` & `soagen-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,25 @@
 
 [project]
 name = 'soagen'
 requires-python = '>=3.9'
 description = 'Struct-of-Arrays generator for C++ projects.'
 authors = [{ name = "Mark Gillard", email = "mark.gillard@outlook.com.au" }]
 license = { text = 'MIT' }
-keywords = ['c++', 'soa', 'struct-of-arrays', 'std::vector']
+keywords = [
+	'c++',
+	'soa',
+	'struct-of-arrays',
+	'structure-of-arrays',
+	'struct of arrays',
+	'structure of arrays',
+	'parallel-arrays',
+	'parallel arrays',
+	'std::vector',
+]
 classifiers = [
 	'Development Status :: 3 - Alpha',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: C++',
 	'Topic :: Software Development :: Code Generators',
 	'Topic :: Utilities',
 ]
@@ -30,15 +40,15 @@
 	'schema != 0.7.5',
 	'colorama',
 	'trieregex',
 ]
 dynamic = ['version', 'readme']
 
 [project.scripts]
-soagen = "soagen:main"
+soagen = 'soagen:main'
 
 [project.urls]
 Source = 'https://github.com/marzer/soagen'
 Tracker = 'https://github.com/marzer/soagen/issues'
 Funding = 'https://github.com/sponsors/marzer'
 
 [tool.setuptools]
@@ -55,8 +65,14 @@
 where = ["src"]
 namespaces = true
 
 [tool.setuptools.package-data]
 "*" = ['*.txt', '*.hpp', '.clang-format']
 
 [tool.setuptools.exclude-package-data]
-"*" = ['meson.build']
+"*" = ['meson.build', '.git*']
+
+[tool.black]
+line-length = 120
+target-version = ['py39']
+skip-string-normalization = true
+skip-magic-trailing-comma = true
```

### Comparing `soagen-0.0.1/src/soagen/column.py` & `soagen-0.1.0/src/soagen/column.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,24 +6,22 @@
 
 from .configurable import Configurable
 from .metavars import *
 from .writer import *
 
 
 class Column(Configurable):
-
-	def __init__(self, var, prev=False):
-		super().__init__(var)
-		self.variable = var
-		self.struct = var.struct
-		self.index = -1  # set by the struct
-		self.name = 'previous_' + var.name if prev else var.name
-		self.alignment = var.alignment
-		self.type = var.type
-		self.param_type = var.param_type
-		self.pointer_type = var.pointer_type
-		self.const_pointer_type = var.const_pointer_type
-		self.default = var.default
-
+    def __init__(self, var, prev=False):
+        super().__init__(var)
+        self.variable = var
+        self.struct = var.struct
+        self.index = -1  # set by the struct
+        self.name = 'previous_' + var.name if prev else var.name
+        self.alignment = var.alignment
+        self.type = var.type
+        self.param_type = var.param_type
+        self.pointer_type = var.pointer_type
+        self.const_pointer_type = var.const_pointer_type
+        self.default = var.default
 
 
 __all__ = [r'Column']
```

### Comparing `soagen-0.0.1/src/soagen/errors.py` & `soagen-0.1.0/src/soagen/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 #!/usr/bin/env python3
 # This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 # Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 # See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 # SPDX-License-Identifier: MIT
 
-from schema import SchemaError
-
-
 
 class Error(Exception):
 
-	"""Base class for other exceptions."""
-
-	def __init__(self, *message):
-		self.__message = r' '.join([str(m) for m in message])
-		super().__init__(self.__message)
+    """Base class for other exceptions."""
 
-	def __str__(self):
-		return self.__message
+    def __init__(self, *message):
+        self.__message = r' '.join([str(m) for m in message])
+        super().__init__(self.__message)
 
+    def __str__(self):
+        return self.__message
 
 
-__all__ = ['Error', 'SchemaError']
+__all__ = ['Error']
```

### Comparing `soagen-0.0.1/src/soagen/hpp/.clang-format` & `soagen-0.1.0/src/soagen/hpp/.clang-format`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 AllowShortIfStatementsOnASingleLine: Never
 AllowShortLoopsOnASingleLine: false
 AlwaysBreakAfterDefinitionReturnType: None
 AlwaysBreakAfterReturnType: None
 AlwaysBreakBeforeMultilineStrings: false
 AlwaysBreakTemplateDeclarations: Yes
 AttributeMacros:
+    - SOAGEN_ABSTRACT_INTERFACE
+    - SOAGEN_CALLCONV
     - SOAGEN_EMPTY_BASES
     - SOAGEN_NODISCARD_CLASS
-    - SOAGEN_ABSTRACT_INTERFACE
     - SOAGEN_TRIVIAL_ABI
     - SOAGEN_VECTORCALL
-    - SOAGEN_CALLCONV
 BinPackArguments: false
 BinPackParameters: false
 BraceWrapping:
     AfterCaseLabel: true
     AfterClass: true
     AfterControlStatement: Always
     AfterEnum: true
@@ -167,27 +167,29 @@
     - SOAGEN_CONST_GETTER
     - SOAGEN_CONST_INLINE_GETTER
     - SOAGEN_CONST_INLINE_GETTER
     - SOAGEN_CONSTEVAL
     - SOAGEN_CONSTRAINED_TEMPLATE
     - SOAGEN_CPP20_CONSTEXPR
     - SOAGEN_DECLSPEC
+    - SOAGEN_HIDDEN_BASE
     - SOAGEN_HIDDEN_CONSTRAINT
     - SOAGEN_INLINE_GETTER
     - SOAGEN_MALLOC
     - SOAGEN_NEVER_INLINE
     - SOAGEN_NODISCARD
     - SOAGEN_NODISCARD_CTOR
     - SOAGEN_PURE
     - SOAGEN_PURE_GETTER
     - SOAGEN_PURE_INLINE_GETTER
     - _Pragma
     - __pragma
 TabWidth: 4
 TypenameMacros:
+    - SOAGEN_ENABLE_IF_T
 UseCRLF: false
 UseTab: Always
 WhitespaceSensitiveMacros:
     - STRINGIZE
     - PP_STRINGIZE
     - BOOST_PP_STRINGIZE
     - SOAGEN_ATTR
```

### Comparing `soagen-0.0.1/src/soagen/hpp/allocator.hpp` & `soagen-0.1.0/src/soagen/hpp/allocator.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,148 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
-#include "functions.hpp"
-
+#include "generated/functions.hpp"
 #include "header_start.hpp"
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 namespace soagen
 {
+	/// @brief The default allocator used by soagen tables.
+	///
+	/// @note Use of this allocator is not required; you can use any allocator compatible with the
+	/// 		 std::allocator protocol, so long as its `value_type` is `char`, `unsigned char` or `std::byte`.
+	///
+	/// @section customizing_allocators Customizing allocators for soagen
+	/// 	Custom allocators may implement two soagen-specific extensions
+	/// 	relating to memory alignment to assist the compiler with generating performant code.
+	/// 	These are detailed below.
+	///
+	/// @subsection customizing_allocators_min_alignment Specifying a min_alignment
+	/// 	If you know that your allocator will never align allocations on a boundary smaller than a
+	/// 	particular value (say, 64 bytes), you can make soagen aware of this by adding a constexpr
+	/// 	constant called `min_alignment`. Example:
+	///
+	/// 	@cpp
+	/// 	struct my_allocator
+	/// 	{
+	/// 		inline constexpr std::size_t min_alignment = 64;
+	/// 	}
+	/// 	@ecpp
+	///
+	/// 	Soagen will then propagate this information to the tables where it may be of use to the compiler.
+	///
+	/// @subsection customizing_allocators_aligned_allocate Providing an alignment-aware allocate()
+	/// 	If your environment has some aligned-allocation facility you wish to make soagen aware of, you
+	/// 	can do so by providing an alignment-aware overload of `allocate()` taking a `std::align_val_t`
+	/// 	for alignment:
+	///
+	/// 	@cpp
+	/// 	struct my_allocator
+	/// 	{
+	/// 		value_type* allocate(std::size_t size, std::align_val_t alignment)
+	/// 		{
+	/// 			return my_aligned_alloc_function(size, static_cast<std::size_t>(alignment));
+	/// 		}
+	/// 	}
+	/// 	@ecpp
+	///
+	/// 	Soagen will choose this overload over any others if it is present.
 	struct allocator
 	{
-		using value_type							 = std::byte;
-		using pointer								 = value_type*;
-		using const_pointer							 = const value_type*;
-		using void_pointer							 = std::byte*;
-		using const_void_pointer					 = const std::byte*;
-		using size_type								 = size_t;
-		using difference_type						 = ptrdiff_t;
-		using is_always_equal						 = std::true_type;
+		/// @brief The value type allocated by this allocator.
+		using value_type		 = std::byte;
+		using pointer			 = value_type*;
+		using const_pointer		 = const value_type*;
+		using void_pointer		 = std::byte*;
+		using const_void_pointer = const std::byte*;
+		using size_type			 = size_t;
+		using difference_type	 = ptrdiff_t;
+
+		/// @brief Instances of this allocator are always equal.
+		using is_always_equal = std::true_type;
+
+		/// @brief Instances of this allocator don't propagate on copy-assignment.
 		using propagate_on_container_copy_assignment = std::false_type;
+
+		/// @brief Instances of this allocator don't propagate on move-assignment.
 		using propagate_on_container_move_assignment = std::false_type;
-		using propagate_on_container_swap			 = std::false_type;
 
+		/// @brief Instances of this allocator don't propagate on swap.
+		using propagate_on_container_swap = std::false_type;
+
+		/// @brief The minimum alignment of any allocations created by this allocator.
 		static constexpr size_t min_alignment =
 			max(size_t{ __STDCPP_DEFAULT_NEW_ALIGNMENT__ }, alignof(std::max_align_t), alignof(value_type));
+		static_assert(has_single_bit(min_alignment));
 
+		/// @brief Alignment-aware allocation.
+		/// @param size The size of the desired allocation, in bytes.
+		/// @param alignment The minimum desired alignment, in bytes. Must be a power-of-two.
+		/// @return A new allocation.
+		/// @throws std::bad_alloc If the system aligned-allocation function failed.
 		SOAGEN_NODISCARD
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_DECLSPEC(noalias)
 		SOAGEN_DECLSPEC(restrict)
 		SOAGEN_ATTR(assume_aligned(min_alignment))
 		SOAGEN_ATTR(returns_nonnull)
 		SOAGEN_ATTR(malloc)
 		value_type* allocate(size_t size, std::align_val_t alignment = std::align_val_t{ min_alignment })
 		{
+			SOAGEN_ASSUME(size);
+			SOAGEN_ASSUME(static_cast<size_t>(alignment));
+
+			size	  = (size + static_cast<size_t>(alignment) - 1u) & ~(static_cast<size_t>(alignment) - 1u);
+			alignment = std::align_val_t{ max(static_cast<size_t>(alignment), min_alignment) };
+
+			SOAGEN_ASSUME((static_cast<size_t>(alignment) & (static_cast<size_t>(alignment) - 1u)) == 0u);
+
 #if SOAGEN_WINDOWS
-			auto ptr = _aligned_malloc(size, max(static_cast<size_t>(alignment), min_alignment));
+			auto ptr = _aligned_malloc(size, static_cast<size_t>(alignment));
 #else
-			auto ptr = std::aligned_alloc(max(static_cast<size_t>(alignment), min_alignment), size);
+			auto ptr = std::aligned_alloc(static_cast<size_t>(alignment), size);
 #endif
-			if (!ptr)
+			if SOAGEN_UNLIKELY(!ptr)
 				throw std::bad_alloc{};
 
 			return soagen::assume_aligned<min_alignment>(static_cast<pointer>(ptr));
 		}
 
+		/// @brief Deallocation.
+		/// @param ptr The pointer to the memory being deallocated.
+		/// @param size The size requested during the initial call to #allocate().
+		/// @attention `ptr` must be a value acquired as the return value of #allocate()!
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_ATTR(nonnull)
-		void deallocate(value_type* ptr, size_t /* size */) noexcept
+		void deallocate(value_type* ptr, [[maybe_unused]] size_t size) noexcept
 		{
 			SOAGEN_ASSUME(ptr != nullptr);
+			SOAGEN_ASSUME(size);
 
 #if SOAGEN_WINDOWS
 			_aligned_free(ptr);
 #else
 			std::free(ptr);
 #endif
 		}
 
-	  private:
+		/// @brief Equality operator.
 		SOAGEN_CONST_INLINE_GETTER
 		friend bool operator==(const allocator&, const allocator&) noexcept
 		{
 			return true;
 		}
 
+		/// @brief Inequality operator.
 		SOAGEN_CONST_INLINE_GETTER
 		friend bool operator!=(const allocator&, const allocator&) noexcept
 		{
 			return false;
 		}
 	};
 	static_assert(std::is_trivially_default_constructible_v<allocator>);
@@ -140,19 +209,19 @@
 			// 2. propagating,     non-equal   yes
 			// 3. non-propagating, equal       yes
 			// 4. non-propagating, non-equal   no (need to re-use existing capacity + move elementwise)
 			static constexpr bool container_move_assign_always_takes_ownership =
 				base_traits::propagate_on_container_move_assignment::value || base_traits::is_always_equal::value;
 		};
 	}
-	/// @endcond
 
 	// primary template - allocator has an aligned-allocation overload
 	template <typename Allocator, bool = detail::has_aligned_allocate<Allocator>>
-	struct allocator_traits : public detail::allocator_traits_base<Allocator>
+	struct allocator_traits //
+		: public detail::allocator_traits_base<Allocator>
 	{
 		using base_traits = detail::allocator_traits_base<Allocator>;
 		using typename base_traits::value_type;
 		using typename base_traits::size_type;
 
 		SOAGEN_NODISCARD
 		SOAGEN_DECLSPEC(noalias)
@@ -167,15 +236,16 @@
 				alloc.allocate(num,
 							   std::align_val_t{ max(static_cast<size_t>(alignment), base_traits::min_alignment) }));
 		}
 	};
 
 	// secondary template - we have to implement the alignment management manually :(:(
 	template <typename Allocator>
-	struct allocator_traits<Allocator, false> : public detail::allocator_traits_base<Allocator>
+	struct allocator_traits<Allocator, false> //
+		: public detail::allocator_traits_base<Allocator>
 	{
 		using base_traits = detail::allocator_traits_base<Allocator>;
 		using typename base_traits::value_type;
 		using typename base_traits::size_type;
 		using typename base_traits::pointer;
 
 	  private:
@@ -218,10 +288,12 @@
 
 			const auto info = reinterpret_cast<alloc_info*>(ptr)[-1];
 			SOAGEN_ASSERT(n == info.requested_size);
 
 			alloc.deallocate(info.ptr, info.actual_size);
 		}
 	};
+
+	/// @endcond
 }
 
 #include "header_end.hpp"
```

### Comparing `soagen-0.0.1/src/soagen/hpp/column_traits.hpp` & `soagen-0.1.0/src/soagen/hpp/column_traits.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 #pragma once
 
-#include "functions.hpp"
+#include "generated/functions.hpp"
 #include "header_start.hpp"
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 /// @cond
 namespace soagen::detail
@@ -68,26 +68,26 @@
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			}
 #endif
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& default_construct_at(std::byte* buffer, size_t element_index) //
+		static constexpr storage_type& default_construct(std::byte* buffer, size_t element_index) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			return default_construct(buffer + element_index * sizeof(storage_type));
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
-		static void default_construct_at(std::byte* buffer, size_t start_index, size_t count) //
+		static void default_construct(std::byte* buffer, size_t start_index, size_t count) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 			SOAGEN_ASSUME(count);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 2022071
 			if constexpr (is_implicit_lifetime_type<storage_type>)
@@ -97,121 +97,172 @@
 			}
 			else
 #endif
 				if constexpr (std::is_nothrow_default_constructible_v<storage_type>
 							  || std::is_trivially_destructible_v<storage_type>)
 			{
 				for (const size_t e = start_index + count; start_index < e; start_index++)
-					default_construct_at(buffer, start_index);
+					default_construct(buffer, start_index);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = start_index;
 
 				try
 				{
 					for (const size_t e = start_index + count; i < e; i++)
-						default_construct_at(buffer, i);
+						default_construct(buffer, i);
 				}
 				catch (...)
 				{
 					for (; i-- > start_index;)
-						destruct_at(buffer, i);
+						destruct(buffer, i);
 					throw;
 				}
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_copyable = std::is_trivially_copyable_v<storage_type>;
+
+	  private:
+		// note: these *should* just be regular variable templates but evidently GCC
+		// chokes on partial variable template specialization at class scope:
+		// https://gcc.gnu.org/bugzilla/show_bug.cgi?id=71954
+
+		template <typename... Args>
+		struct is_constructible_with_memcpy_ : std::false_type
+		{};
+		template <typename Arg>
+		struct is_constructible_with_memcpy_<Arg>
+			: std::bool_constant<sizeof(storage_type) == sizeof(remove_cvref<Arg>)	//
+								 && is_trivially_copyable							//
+								 && is_implicit_lifetime_type<storage_type>			//
+								 && std::is_trivially_copyable_v<remove_cvref<Arg>> //
+								 && (std::is_same_v<storage_type, remove_cvref<Arg>>
+									 || (any_same<storage_type, char, unsigned char, std::byte>
+										 && any_same<remove_cvref<Arg>, char, unsigned char, std::byte>)
+									 || (std::is_same_v<storage_type, void*> && std::is_pointer_v<remove_cvref<Arg>>))>
+		{};
+
+	  public:
+		template <typename... Args>
+		static constexpr bool is_constructible_with_memcpy = is_constructible_with_memcpy_<Args...>::value;
+
 		template <typename... Args>
-		static constexpr bool is_constructible = std::is_constructible_v<storage_type, Args&&...>;
+		static constexpr bool is_trivially_constructible =
+			is_constructible_with_memcpy<Args...>
+			|| std::is_trivially_constructible_v<storage_type, remove_cvref<Args>...>;
+
+	  private:
+		template <typename... Args>
+		struct is_constructible_
+			: std::bool_constant<is_trivially_constructible<Args...> || std::is_constructible_v<storage_type, Args...>>
+		{};
+		template <typename T>
+		struct is_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
+														  || is_trivially_constructible<T*>	  //
+														  || std::is_constructible_v<storage_type, T*>>
+		{};
 		template <typename T>
-		static constexpr bool is_constructible<T*&> = std::is_same_v<storage_type, void*>;
+		struct is_constructible_<T*&> : std::bool_constant<std::is_same_v<storage_type, void*> //
+														   || is_trivially_constructible<T*&>  //
+														   || std::is_constructible_v<storage_type, T*&>>
+		{};
 		template <typename T>
-		static constexpr bool is_constructible<T*&&> = std::is_same_v<storage_type, void*>;
+		struct is_constructible_<T*&&> : std::bool_constant<std::is_same_v<storage_type, void*> //
+															|| is_trivially_constructible<T*&&> //
+															|| std::is_constructible_v<storage_type, T*&&>>
+		{};
+		template <typename... Args>
+		struct is_constructible_<emplacer<Args...>&&> : is_constructible_<Args...>
+		{};
+
+	  public:
 		template <typename... Args>
-		static constexpr bool is_constructible<emplacer<Args...>&&> = is_constructible<Args...>;
+		static constexpr bool is_constructible = is_constructible_<Args...>::value;
 
+	  private:
 		template <typename... Args>
-		static constexpr bool is_nothrow_constructible = std::is_nothrow_constructible_v<storage_type, Args&&...>;
+		struct is_nothrow_constructible_ : std::bool_constant<is_trivially_constructible<Args...>
+															  || std::is_nothrow_constructible_v<storage_type, Args...>>
+		{};
+		template <typename T>
+		struct is_nothrow_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
+																  || is_trivially_constructible<T*>	  //
+																  || std::is_nothrow_constructible_v<storage_type, T*>>
+		{};
 		template <typename T>
-		static constexpr bool is_nothrow_constructible<T*&> = std::is_same_v<storage_type, void*>;
+		struct is_nothrow_constructible_<T*&>
+			: std::bool_constant<std::is_same_v<storage_type, void*> //
+								 || is_trivially_constructible<T*&>	 //
+								 || std::is_nothrow_constructible_v<storage_type, T*&>>
+		{};
 		template <typename T>
-		static constexpr bool is_nothrow_constructible<T*&&> = std::is_same_v<storage_type, void*>;
+		struct is_nothrow_constructible_<T*&&>
+			: std::bool_constant<std::is_same_v<storage_type, void*> //
+								 || is_trivially_constructible<T*&&> //
+								 || std::is_nothrow_constructible_v<storage_type, T*&&>>
+		{};
+		template <typename... Args>
+		struct is_nothrow_constructible_<emplacer<Args...>&&> : is_nothrow_constructible_<Args...>
+		{};
+
+	  public:
 		template <typename... Args>
-		static constexpr bool is_nothrow_constructible<emplacer<Args...>&&> = is_constructible<Args...>;
+		static constexpr bool is_nothrow_constructible = is_nothrow_constructible_<Args...>::value;
 
 	  private:
 		template <typename... Args, size_t... Indices>
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct_from_emplacer(std::byte* destination,
 															   emplacer<Args...>&& args,
 															   std::index_sequence<Indices...>) //
 			noexcept(is_nothrow_constructible<Args...>)
 		{
-			static_assert(sizeof...(Args) == sizeof...(Indices));
 			static_assert((std::is_reference_v<Args> && ...));
+			static_assert(sizeof...(Args) == sizeof...(Indices));
+			SOAGEN_ASSUME(destination != nullptr);
 
-			if constexpr (std::is_aggregate_v<storage_type>)
-			{
-				return *(
-					::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-						storage_type{ static_cast<Args>(
-							*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(args.ptrs[Indices]))... });
-			}
-			else
-			{
-				return *(
-					::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-						storage_type(static_cast<Args>(
-							*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(args.ptrs[Indices]))...));
-			}
+			return construct(destination,
+							 static_cast<Args>(*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(
+								 args.ptrs[Indices]))...);
 		}
 
 	  public:
-		template <typename... Args>
-		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& construct_from_emplacer(std::byte* destination,
-															   emplacer<Args...>&& args) //
-			noexcept(is_nothrow_constructible<Args...>)
-		{
-			static_assert((std::is_reference_v<Args> && ...));
-
-			return construct_from_emplacer(destination,
-										   static_cast<emplacer<Args...>&&>(args),
-										   std::make_index_sequence<sizeof...(Args)>{});
-		}
-
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct(std::byte* destination, Args&&... args) //
 			noexcept(is_nothrow_constructible<Args&&...>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 
 			if constexpr (sizeof...(Args) == 0)
 			{
 				return default_construct(destination);
 			}
 			else
 			{
-				if constexpr (sizeof...(Args) == 1										   //
-							  && (std::is_pointer_v<std::remove_reference_t<Args>> && ...) //
-							  && std::is_same_v<storage_type, void*>)
+				if constexpr (sizeof...(Args) == 1 && (is_emplacer<std::remove_reference_t<Args>> && ...))
 				{
-					return *(
-						::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-							storage_type{ const_cast<storage_type>(reinterpret_cast<const volatile void*>(args))... });
+					return construct_from_emplacer(
+						destination,
+						static_cast<Args&&>(args)...,
+						std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
-				else if constexpr (sizeof...(Args) == 1 && (is_emplacer<std::remove_reference_t<Args>> && ...))
+				else if constexpr (is_constructible_with_memcpy<Args&&...>)
 				{
-					return construct_from_emplacer(destination, static_cast<Args&&>(args)...);
+					std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
+								soagen::assume_aligned<alignof(storage_type)>(&args)...,
+								sizeof(storage_type));
+
+					return get(destination);
 				}
 				else if constexpr (std::is_aggregate_v<storage_type>)
 				{
 					return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
 								 storage_type{ static_cast<Args&&>(args)... });
 				}
 				else
@@ -237,39 +288,39 @@
 			{
 				return construct(buffer + element_index * sizeof(storage_type), static_cast<Args&&>(args)...);
 			}
 		}
 
 		//--- move-construction ----------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_move_constructible = is_trivially_constructible<storage_type&&>;
+
 		static constexpr bool is_move_constructible =
-			std::is_move_constructible_v<storage_type>
+			is_trivially_move_constructible				  //
+			|| std::is_move_constructible_v<storage_type> //
 			|| (std::is_default_constructible_v<storage_type> && std::is_move_assignable_v<storage_type>);
 
-		static constexpr bool is_nothrow_move_constructible = std::is_move_constructible_v<storage_type>
-																? std::is_nothrow_move_constructible_v<storage_type>
-																: (std::is_nothrow_default_constructible_v<storage_type>
-																   && std::is_nothrow_move_assignable_v<storage_type>);
-
-		static constexpr bool is_trivially_move_constructible =
-			std::is_move_constructible_v<storage_type> ? std::is_trivially_move_constructible_v<storage_type>
-													   : (std::is_trivially_default_constructible_v<storage_type>
-														  && std::is_trivially_move_assignable_v<storage_type>);
+		static constexpr bool is_nothrow_move_constructible =
+			is_trivially_move_constructible
+				? true
+				: (std::is_move_constructible_v<storage_type> ? std::is_nothrow_move_constructible_v<storage_type>
+															  : std::is_nothrow_default_constructible_v<storage_type>
+																	&& std::is_nothrow_move_assignable_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_constructible)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
 		static storage_type& move_construct(std::byte* destination, std::byte* source) //
 			noexcept(is_nothrow_move_constructible)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_move_constructible_v<storage_type>)
+			if constexpr (is_trivially_move_constructible || std::is_move_constructible_v<storage_type>)
 			{
 				return construct(destination, static_cast<storage_type&&>(get(source)));
 			}
 			else
 			{
 				static_assert(std::is_default_constructible_v<storage_type>);
 				static_assert(std::is_move_assignable_v<storage_type>);
@@ -293,54 +344,54 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_move_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_construct_at(std::byte* dest_buffer,
-														 size_t dest_element_index,
-														 std::byte* source_buffer,
-														 size_t source_element_index) //
+		static constexpr storage_type& move_construct(std::byte* dest_buffer,
+													  size_t dest_element_index,
+													  std::byte* source_buffer,
+													  size_t source_element_index) //
 			noexcept(std::is_nothrow_move_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return move_construct(dest_buffer + dest_element_index * sizeof(storage_type),
 								  source_buffer + source_element_index * sizeof(storage_type));
 		}
 
 		//--- copy-construction ----------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_copy_constructible = is_trivially_constructible<const storage_type&>;
+
 		static constexpr bool is_copy_constructible =
-			std::is_copy_constructible_v<storage_type>
+			is_trivially_copy_constructible				  //
+			|| std::is_copy_constructible_v<storage_type> //
 			|| (std::is_default_constructible_v<storage_type> && std::is_copy_assignable_v<storage_type>);
 
-		static constexpr bool is_nothrow_copy_constructible = std::is_copy_constructible_v<storage_type>
-																? std::is_nothrow_copy_constructible_v<storage_type>
-																: (std::is_nothrow_default_constructible_v<storage_type>
-																   && std::is_nothrow_copy_assignable_v<storage_type>);
-
-		static constexpr bool is_trivially_copy_constructible =
-			std::is_copy_constructible_v<storage_type> ? std::is_trivially_copy_constructible_v<storage_type>
-													   : (std::is_trivially_default_constructible_v<storage_type>
-														  && std::is_trivially_copy_assignable_v<storage_type>);
+		static constexpr bool is_nothrow_copy_constructible =
+			is_trivially_copy_constructible
+				? true
+				: (std::is_copy_constructible_v<storage_type> ? std::is_nothrow_copy_constructible_v<storage_type>
+															  : std::is_nothrow_default_constructible_v<storage_type>
+																	&& std::is_nothrow_copy_assignable_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_constructible)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
 		static storage_type& copy_construct(std::byte* destination, const std::byte* source) //
 			noexcept(is_nothrow_copy_constructible)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_copy_constructible_v<storage_type>)
+			if constexpr (is_trivially_copy_constructible || std::is_copy_constructible_v<storage_type>)
 			{
 				return construct(destination, static_cast<const storage_type&>(get(source)));
 			}
 			else
 			{
 				static_assert(std::is_default_constructible_v<storage_type>);
 				static_assert(std::is_copy_assignable_v<storage_type>);
@@ -364,18 +415,18 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_constructible)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_construct_at(std::byte* dest_buffer,
-														 size_t dest_element_index,
-														 const std::byte* source_buffer,
-														 size_t source_element_index) //
+		static constexpr storage_type& copy_construct(std::byte* dest_buffer,
+													  size_t dest_element_index,
+													  const std::byte* source_buffer,
+													  size_t source_element_index) //
 			noexcept(is_nothrow_copy_constructible)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return copy_construct(dest_buffer + dest_element_index * sizeof(storage_type),
 								  source_buffer + source_element_index * sizeof(storage_type));
@@ -392,108 +443,126 @@
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
 				get(target).~storage_type();
 			}
 		}
 
 		SOAGEN_ATTR(nonnull)
-		static constexpr void destruct_at([[maybe_unused]] std::byte* buffer,	 //
-										  [[maybe_unused]] size_t element_index) //
+		static constexpr void destruct([[maybe_unused]] std::byte* buffer,	  //
+									   [[maybe_unused]] size_t element_index) //
 			noexcept(std::is_nothrow_destructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
 				destruct(buffer + element_index * sizeof(storage_type));
 			}
 		}
 
 		//--- move-assignment ------------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_move_assignable =
+			is_constructible_with_memcpy<storage_type&&> || std::is_trivially_move_assignable_v<storage_type>;
+
 		static constexpr bool is_move_assignable =
-			std::is_move_assignable_v<storage_type>
+			is_trivially_move_assignable			   //
+			|| std::is_move_assignable_v<storage_type> //
 			|| (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_move_constructible_v<storage_type>);
 
 		static constexpr bool is_nothrow_move_assignable =
-			std::is_move_assignable_v<storage_type>
-				? std::is_nothrow_move_assignable_v<storage_type>
-				: (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_move_constructible_v<storage_type>);
-
-		static constexpr bool is_trivially_move_assignable =
-			std::is_move_assignable_v<storage_type> ? std::is_trivially_move_assignable_v<storage_type>
-													: (std::is_trivially_destructible_v<storage_type>
-													   && std::is_trivially_move_constructible_v<storage_type>);
+			is_trivially_move_assignable
+				? true
+				: (std::is_move_assignable_v<storage_type> ? std::is_nothrow_move_assignable_v<storage_type>
+														   : std::is_nothrow_destructible_v<storage_type>
+																 && std::is_nothrow_move_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& move_assign(std::byte* destination, void* source) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_move_assignable_v<storage_type>)
+			if constexpr (is_constructible_with_memcpy<storage_type&&>)
+			{
+				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
+							soagen::assume_aligned<alignof(storage_type)>(static_cast<std::byte*>(source)),
+							sizeof(storage_type));
+
+				return get(destination);
+			}
+			else if constexpr (is_trivially_move_assignable || std::is_move_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<storage_type&&>(get(static_cast<std::byte*>(source)));
 			}
 			else
 			{
-				// note we only fallback to this if they're nothrow because we don't want to leave the destination
+				// note we only fall back to this if they're nothrow because we don't want to leave the destination
 				// in a half-constructed state (it existed before the assignment, it should still exist after)
 				static_assert(std::is_nothrow_destructible_v<storage_type>);
 				static_assert(std::is_nothrow_move_constructible_v<storage_type>);
 
 				destruct(destination);
 				return move_construct(destination, static_cast<std::byte*>(source));
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_assign_at(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  std::byte* source_buffer,
-													  size_t source_element_index) //
+		static constexpr storage_type& move_assign(std::byte* dest_buffer,
+												   size_t dest_element_index,
+												   std::byte* source_buffer,
+												   size_t source_element_index) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return move_assign(dest_buffer + dest_element_index * sizeof(storage_type),
 							   source_buffer + source_element_index * sizeof(storage_type));
 		}
 
 		//--- copy-assignment ------------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_copy_assignable =
+			is_constructible_with_memcpy<const storage_type&> || std::is_trivially_copy_assignable_v<storage_type>;
+
 		static constexpr bool is_copy_assignable =
-			std::is_copy_assignable_v<storage_type>
+			is_trivially_copy_assignable			   //
+			|| std::is_copy_assignable_v<storage_type> //
 			|| (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_copy_constructible_v<storage_type>);
 
 		static constexpr bool is_nothrow_copy_assignable =
-			std::is_copy_assignable_v<storage_type>
-				? std::is_nothrow_copy_assignable_v<storage_type>
-				: (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_copy_constructible_v<storage_type>);
-
-		static constexpr bool is_trivially_copy_assignable =
-			std::is_copy_assignable_v<storage_type> ? std::is_trivially_copy_assignable_v<storage_type>
-													: (std::is_trivially_destructible_v<storage_type>
-													   && std::is_trivially_copy_constructible_v<storage_type>);
+			is_trivially_copy_assignable
+				? true
+				: (std::is_copy_assignable_v<storage_type> ? std::is_nothrow_copy_assignable_v<storage_type>
+														   : std::is_nothrow_destructible_v<storage_type>
+																 && std::is_nothrow_copy_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& copy_assign(std::byte* destination, const std::byte* source) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_copy_assignable_v<storage_type>)
+			if constexpr (is_constructible_with_memcpy<storage_type&&>)
+			{
+				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
+							soagen::assume_aligned<alignof(storage_type)>(static_cast<const std::byte*>(source)),
+							sizeof(storage_type));
+
+				return get(destination);
+			}
+			else if constexpr (is_trivially_copy_assignable || std::is_copy_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<const storage_type&>(get(source));
 			}
 			else
 			{
 				// note we only fallback to this if they're nothrow because we don't want to leave the destination
 				// in a half-constructed state (it existed before the assignment, it should still exist after)
@@ -503,18 +572,18 @@
 				destruct(destination);
 				return copy_construct(destination, source);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_assign_at(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  const std::byte* source_buffer,
-													  size_t source_element_index) //
+		static constexpr storage_type& copy_assign(std::byte* dest_buffer,
+												   size_t dest_element_index,
+												   const std::byte* source_buffer,
+												   size_t source_element_index) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return copy_assign(dest_buffer + dest_element_index * sizeof(storage_type),
 							   source_buffer + source_element_index * sizeof(storage_type));
@@ -549,85 +618,201 @@
 				move_assign(lhs, rhs);
 				move_assign(rhs, &temp);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_swappable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr void swap_at(std::byte* lhs_buffer,
-									  size_t lhs_element_index,
-									  std::byte* rhs_buffer,
-									  size_t rhs_element_index) //
+		static constexpr void swap(std::byte* lhs_buffer,
+								   size_t lhs_element_index,
+								   std::byte* rhs_buffer,
+								   size_t rhs_element_index) //
 			noexcept(is_nothrow_swappable)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
 			return swap(lhs_buffer + lhs_element_index * sizeof(storage_type),
 						rhs_buffer + rhs_element_index * sizeof(storage_type));
 		}
 
-		//--- trivially-copy (memmove) ---------------------------------------------------------------------------------
+		//--- memmove ---------------------------------------------------------------------------------
 
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_trivially_copyable_v<storage_type>)
-		static constexpr void trivially_copy(std::byte* dest_buffer,
-											 size_t dest_element_index,
-											 const std::byte* source_buffer,
-											 size_t source_element_index,
-											 size_t count) noexcept
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_trivially_copyable)
+		static constexpr void memmove(std::byte* dest_buffer,
+									  size_t dest_element_index,
+									  const std::byte* source_buffer,
+									  size_t source_element_index,
+									  size_t count) noexcept
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			std::memmove(dest_buffer + dest_element_index * sizeof(storage_type),
 						 source_buffer + source_element_index * sizeof(storage_type),
 						 count * sizeof(storage_type));
 		}
-	};
 
+		//--- equality -------------------------------------------------------------------------------------------------
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool equal(const std::byte* lhs, const std::byte* rhs) //
+			noexcept(is_nothrow_equality_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs != nullptr);
+			SOAGEN_ASSUME(rhs != nullptr);
+
+			return get(lhs) == get(rhs);
+		}
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool equal(const std::byte* lhs_buffer,
+									size_t lhs_start_index,
+									const std::byte* rhs_buffer,
+									size_t rhs_start_index,
+									size_t count = 1) //
+			noexcept(is_nothrow_equality_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs_buffer != nullptr);
+			SOAGEN_ASSUME(rhs_buffer != nullptr);
+
+			lhs_buffer += lhs_start_index * sizeof(storage_type);
+			rhs_buffer += rhs_start_index * sizeof(storage_type);
+			const auto end = lhs_buffer + count * sizeof(storage_type);
+
+			for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
+			{
+				if (!equal(lhs_buffer, rhs_buffer))
+					return false;
+			}
+
+			return true;
+		}
+
+		//--- less-than ------------------------------------------------------------------------------------------------
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_less_than_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool less_than(const std::byte* lhs, const std::byte* rhs) //
+			noexcept(is_nothrow_less_than_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs != nullptr);
+			SOAGEN_ASSUME(rhs != nullptr);
+
+			return get(lhs) < get(rhs);
+		}
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_less_than_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool less_than(const std::byte* lhs_buffer,
+										size_t lhs_element_index,
+										const std::byte* rhs_buffer,
+										size_t rhs_element_index) //
+			noexcept(is_nothrow_less_than_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs_buffer != nullptr);
+			SOAGEN_ASSUME(rhs_buffer != nullptr);
+
+			return less_than(lhs_buffer + lhs_element_index * sizeof(storage_type),
+							 rhs_buffer + rhs_element_index * sizeof(storage_type));
+		}
+	};
 }
 /// @endcond
 
 namespace soagen
 {
+	/// @brief	Traits for a single column of a table.
+	/// @tparam	ValueType	The column's value type.
+	/// @tparam	ParamType	The type used for the column in function parameter contexts (e.g. push_back()).
+	/// @tparam	Align		The minimum memory alignment of the first element in the column.
+	///
+	///	@attention	This class is an implementation detail for the soagen-generated Structure-of-arrays classes.
+	///				You don't need to know anything about it unless you are implementing your own SoA machinery
+	///				without using the soagen generator.
 	template <typename ValueType,
-			  typename ParamType = param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType),
-			  typename Base		 = detail::column_traits_base<storage_type<ValueType>>>
-	struct column_traits : public Base
+			  typename ParamType = soagen::param_type<ValueType>,
+			  size_t Align		 = alignof(ValueType)
+				  SOAGEN_HIDDEN_PARAM(typename Base = detail::column_traits_base<storage_type<ValueType>>)>
+	struct SOAGEN_EMPTY_BASES column_traits //
+		SOAGEN_HIDDEN_BASE(public Base)
 	{
+#if SOAGEN_DOXYGEN
+
+		/// @copydoc soagen::storage_type
+		using storage_type = POXY_IMPLEMENTATION_DETAIL(dummy);
+
+#endif
+
+		/// @brief	The column's value type.
 		using value_type = ValueType;
 		static_assert(!std::is_reference_v<value_type>, "column value_type may not be a reference");
 		static_assert(!std::is_void_v<value_type>, "column value_type may not be void");
 		static_assert(alignof(value_type) == alignof(typename Base::storage_type));
 		static_assert(sizeof(value_type) == sizeof(typename Base::storage_type));
 
+		/// @brief	The type used for the column in lvalue function parameter contexts (e.g. `push_back(const &)`).
 		using param_type = ParamType;
 		static_assert(!std::is_void_v<param_type>, "column param_type may not be void");
-		static_assert(std::is_convertible_v<param_type, value_type> || std::is_constructible_v<value_type, param_type>
-						  || (std::is_pointer_v<param_type> && std::is_same_v<typename Base::storage_type, void*>),
-					  "column value_type must be constructible or convertible from param_type");
-
+		static_assert(std::is_reference_v<param_type> || !is_cv<param_type>,
+					  "value parameters may not be cv-qualified");
+		static_assert(Base::template is_constructible<param_type>);
+
+		/// @brief	The type used when forwarding #param_type to the backing container (e.g. `table.emplace_back()`)
+		using param_forward_type = forward_type<param_type>;
+
+		/// @brief	The type used for the column in rvalue function parameter contexts (e.g. `push_back(&&)`).
+		using rvalue_type = soagen::rvalue_type<param_type>;
+		static_assert(Base::template is_constructible<rvalue_type>);
+
+		/// @brief	The type used when forwarding #rvalue_type to the backing container (e.g. `table.emplace_back()`)
+		using rvalue_forward_type = forward_type<rvalue_type>;
+
+		/// @brief	The default type for `emplace()` and `emplace_back()` for columns that have a `default` value.
+		using default_emplace_type = make_cref<rvalue_type>;
+
+		/// @brief	The minimum memory alignment of the first element in the column.
+		///
+		/// @note	This is *not* the alignment of each individual element! That is always `alignof(value_type)`.
+		///			This value is referring to the alignment of the allocation for the entire column's buffer region.
 		static constexpr size_t alignment = max(Align, alignof(value_type));
 		static_assert(has_single_bit(alignment), "column alignment must be a power of two");
 
-		static constexpr size_t max_capacity = static_cast<size_t>(-1) / sizeof(value_type);
-
+		/// @brief	The amount of elements to advance to maintain the requested #alignment for this column.
+		///
+		/// @details	The stride size you need to use when iterating through elements of this column such that
+		///				the starting element for each batch would have the same memory alignment as the value specified
+		/// 			for #alignment.
+		///
+		/// @note		Typically you can ignore this; column elements are always aligned correctly according to their
+		///				type. This is for over-alignment scenarios where you need to do things in batches (e.g. SIMD).
 		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
 	};
 
-	template <typename>
-	inline constexpr bool is_column_traits = false;
-
+	/// @brief True if `T` is an instance of #soagen::column_traits.
+	template <typename T>
+	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
+	/// @cond
 	template <typename StorageType>
 	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
-
 	template <typename ValueType, typename ParamType, size_t Align, typename Base>
 	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align, Base>> = is_column_traits<Base>;
-
+	template <typename T>
+	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
+	template <typename T>
+	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
+	template <typename T>
+	inline constexpr bool is_column_traits<const volatile T> = is_column_traits<T>;
+	/// @endcond
 }
 
 /// @cond
 namespace soagen::detail
 {
 	template <typename T>
 	struct to_base_traits_;
@@ -638,11 +823,18 @@
 		using type = column_traits_base<storage_type<ValueType>>;
 
 		static_assert(std::is_base_of_v<type, column_traits<ValueType, ParamType, Align>>);
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
+
+	template <typename ValueType, //
+			  typename ParamType = param_type<ValueType>,
+			  size_t Align		 = alignof(ValueType)>
+	using make_column = soagen::column_traits<ValueType, //
+											  ParamType,
+											  soagen::max(Align, alignof(ValueType))>;
 }
 /// @endcond
 
 #include "header_end.hpp"
```

### Comparing `soagen-0.0.1/src/soagen/hpp/compressed_pair.hpp` & `soagen-0.1.0/src/soagen/hpp/generated/compressed_pair.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 //#---------------------------------------------------------------------------------------------------------------------
 //#     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //#---------------------------------------------------------------------------------------------------------------------
 
 #pragma once
 
-#include "meta.hpp"
-#include "header_start.hpp"
+#include "../meta.hpp"
+#include "../header_start.hpp"
+
+/// @cond
 
 namespace soagen
 {
 	namespace detail
 	{
 #define SOAGEN_COMPRESSED_PAIR_BASE_GETTERS(T, name, expression)                                                       \
 	SOAGEN_PURE_INLINE_GETTER                                                                                          \
@@ -251,8 +253,10 @@
 	{
 		static_assert(I < 2);
 		using type = std::conditional_t<I == 1, Second, First>;
 	};
 
 }
 
-#include "header_end.hpp"
+/// @endcond
+
+#include "../header_end.hpp"
```

### Comparing `soagen-0.0.1/src/soagen/hpp/core.hpp` & `soagen-0.1.0/src/soagen/hpp/generated/core.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 //#---------------------------------------------------------------------------------------------------------------------
 //#     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //#---------------------------------------------------------------------------------------------------------------------
 
 #pragma once
 
 #include "preprocessor.hpp"
-
 SOAGEN_DISABLE_WARNINGS;
 #include <cstdint>
 #include <cstddef>
 #include <cstdlib>
+#include <cstring>
 #include <numeric>
 #include <type_traits>
 #include <new>
 #include <utility>
 #include <memory>
 #include <optional>
 SOAGEN_ENABLE_WARNINGS;
-
-#include "header_start.hpp"
+#include "../header_start.hpp"
 
 #if defined(__cpp_lib_launder) && __cpp_lib_launder >= 201606
 	#define SOAGEN_LAUNDER(...) std::launder(__VA_ARGS__)
 #elif SOAGEN_CLANG >= 8 || SOAGEN_GCC >= 7 || SOAGEN_ICC >= 1910 || SOAGEN_MSVC >= 1914                                \
 	|| SOAGEN_HAS_BUILTIN(__builtin_launder)
 	#define SOAGEN_LAUNDER(...) __builtin_launder(__VA_ARGS__)
 #else
 	#define SOAGEN_LAUNDER(...) __VA_ARGS__
 #endif
 
 //--- typedefs and type traits -----------------------------------------------------------------------------------------
 
+/// @brief The root namespace for the library.
 namespace soagen
 {
 	using std::size_t;
 	using std::ptrdiff_t;
 	using std::intptr_t;
 	using std::uintptr_t;
 	using std::nullptr_t;
@@ -42,43 +42,54 @@
 #if SOAGEN_HAS_BUILTIN(__type_pack_element)
 
 	template <size_t I, typename... T>
 	using type_at_index = __type_pack_element<I, T...>;
 
 #else
 
+	/// \cond
 	namespace detail
 	{
 		template <size_t I, typename T, typename... U>
 		struct type_at_index_impl
 		{
 			using type = typename type_at_index_impl<I - 1, U...>::type;
 		};
 
 		template <typename T, typename... U>
 		struct type_at_index_impl<0, T, U...>
 		{
 			using type = T;
 		};
 	}
+	/// \endcond
+
+	/// \brief	The type at the given index in the list.
 	template <size_t I, typename... T>
-	using type_at_index = typename detail::type_at_index_impl<I, T...>::type;
+	using type_at_index = POXY_IMPLEMENTATION_DETAIL(typename detail::type_at_index_impl<I, T...>::type);
 
 #endif
 
+	/// \cond
 	namespace detail
 	{
 		template <template <typename...> typename Trait, typename Enabler, typename... Args>
 		struct is_detected_impl : std::false_type
 		{};
 		template <template <typename...> typename Trait, typename... Args>
 		struct is_detected_impl<Trait, std::void_t<Trait<Args...>>, Args...> : std::true_type
 		{};
 		template <template <typename...> typename Trait, typename... Args>
 		inline constexpr auto is_detected_ = is_detected_impl<Trait, void, Args...>::value;
 	}
+	/// \endcond
+
+	/// \brief Detects if a type supports an interface.
+	/// \see
+	///		- [Detection Idiom](https://blog.tartanllama.xyz/detection-idiom/)
+	///		- [std::experimental::is_detected](https://en.cppreference.com/w/cpp/experimental/is_detected)
 	template <template <typename...> typename Trait, typename... Args>
 	inline constexpr auto is_detected = detail::is_detected_<Trait, Args...>;
 
 }
 
-#include "header_end.hpp"
+#include "../header_end.hpp"
```

### Comparing `soagen-0.0.1/src/soagen/hpp/header_end.hpp` & `soagen-0.1.0/src/soagen/hpp/header_end.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 
 //# note: this header is the exact reverse of header_start.hpp
 
-#include "preprocessor.hpp"
+#include "generated/preprocessor.hpp"
 
 //# reset optimizations
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
```

### Comparing `soagen-0.0.1/src/soagen/hpp/header_start.hpp` & `soagen-0.1.0/src/soagen/hpp/header_start.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 //# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 //# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 //# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 //# SPDX-License-Identifier: MIT
 
 //# note: any preprocessor/compiler state modified here must be undone in header_end.hpp
 
-#include "preprocessor.hpp"
+#include "generated/preprocessor.hpp"
 
 //# push the current warning state
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
 
 //# disable windows.h min/max macro crimes
 #if SOAGEN_MSVC_LIKE
```

### Comparing `soagen-0.0.1/src/soagen/hpp/preprocessor.hpp` & `soagen-0.1.0/src/soagen/hpp/generated/preprocessor.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,15 @@
 #ifndef SOAGEN_ARCH_X64
 	#if SOAGEN_ARCH_BITNESS == 64
 		#define SOAGEN_ARCH_X64 1
 	#else
 		#define SOAGEN_ARCH_X64 0
 	#endif
 #endif
+/// \brief `1` when targeting any 64-bit architecture, otherwise `0`.
 
 #ifdef _WIN32
 	#define SOAGEN_WINDOWS 1
 #else
 	#define SOAGEN_WINDOWS 0
 #endif
 #ifdef __unix__
@@ -409,24 +410,20 @@
 	#elif SOAGEN_CPP >= 20 && SOAGEN_HAS_CPP_ATTR(no_unique_address) >= 201803
 		#define SOAGEN_NO_UNIQUE_ADDRESS [[no_unique_address]]
 	#else
 		#define SOAGEN_NO_UNIQUE_ADDRESS
 	#endif
 #endif
 
-#ifndef SOAGEN_COLUMN
-	#define SOAGEN_COLUMN(I)                                                                                           \
-		SOAGEN_PURE_INLINE_GETTER                                                                                      \
-		SOAGEN_ATTR(returns_nonnull)
-#endif
-
-#ifndef SOAGEN_ALIGNED_COLUMN
-	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
-		SOAGEN_COLUMN(I)                                                                                               \
-		SOAGEN_ATTR(assume_aligned(soagen::detail::actual_column_alignment<table_traits, allocator_type, I>))
+#ifndef SOAGEN_HAS_EXCEPTIONS
+	#if defined(__EXCEPTIONS) || defined(_CPPUNWIND) || defined(__cpp_exceptions)
+		#define SOAGEN_HAS_EXCEPTIONS 1
+	#else
+		#define SOAGEN_HAS_EXCEPTIONS 0
+	#endif
 #endif
 
 #if defined(__cpp_constexpr) && __cpp_constexpr >= 202002L
 	#define SOAGEN_CPP20_CONSTEXPR constexpr
 #else
 	#define SOAGEN_CPP20_CONSTEXPR
 #endif
@@ -453,16 +450,18 @@
 	#else
 		#define SOAGEN_STD_CONCEPT(...) true
 	#endif
 #endif
 
 #ifndef SOAGEN_ENABLE_IF
 	#if !SOAGEN_DOXYGEN
-		#define SOAGEN_ENABLE_IF(...) , typename std::enable_if<!!(__VA_ARGS__), int>::type = 0
+		#define SOAGEN_ENABLE_IF_T(T, ...) std::enable_if_t<!!(__VA_ARGS__), T>
+		#define SOAGEN_ENABLE_IF(...)	   , SOAGEN_ENABLE_IF_T(int, __VA_ARGS__) = 0
 	#else
+		#define SOAGEN_ENABLE_IF_T(T, ...)
 		#define SOAGEN_ENABLE_IF(...)
 	#endif
 #endif
 
 #ifndef SOAGEN_CONSTRAINED_TEMPLATE
 	#if !SOAGEN_DOXYGEN
 		#define SOAGEN_CONSTRAINED_TEMPLATE(condition, ...)                                                            \
@@ -477,18 +476,20 @@
 	#if !SOAGEN_DOXYGEN
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...) SOAGEN_CONSTRAINED_TEMPLATE(condition, __VA_ARGS__)
 	#else
 		#define SOAGEN_HIDDEN_CONSTRAINT(condition, ...)
 	#endif
 #endif
 
+/// @cond
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)                                                                          \
 		SOAGEN_CONSTRAINED_TEMPLATE(sfinae_col_idx == (I) && (__VA_ARGS__), size_t sfinae_col_idx = (I))
 #endif
+/// @endcond
 #ifndef SOAGEN_CONSTRAINED_COLUMN
 	#define SOAGEN_CONSTRAINED_COLUMN(I, ...)
 #endif
 
 #ifndef SOAGEN_PUSH_WARNINGS
 	#if SOAGEN_CLANG
 		#define SOAGEN_PUSH_WARNINGS                                                                                   \
@@ -669,29 +670,26 @@
 			_Pragma("clang diagnostic ignored \"-Wtautological-pointer-compare\"")                                     \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_8;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_9;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13;                                                                     \
 			static_assert(true)
 	#elif SOAGEN_MSVC
 		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                           \
-			__pragma(warning(disable : 4127)) /* conditional expr is constant */                                       \
-			__pragma(warning(disable : 4324)) /* structure was padded due to alignment specifier */                    \
+			__pragma(warning(disable : 4127))  /* conditional expr is constant */                                      \
+			__pragma(warning(disable : 4324))  /* structure was padded due to alignment specifier */                   \
 			__pragma(warning(disable : 4348))                                                                          \
-			__pragma(warning(disable : 4464)) /* relative include path contains '..' */                                \
-			__pragma(warning(disable : 4505)) /* unreferenced local function removed */                                \
-			__pragma(warning(disable : 4514)) /* unreferenced inline function has been removed */                      \
-			__pragma(warning(disable : 4582)) /* constructor is not implicitly called */                               \
-			__pragma(warning(disable : 4619)) /* there is no warning number 'XXXX' */                                  \
-			__pragma(warning(disable : 4623)) /* default constructor was implicitly defined as deleted */              \
-			__pragma(warning(disable : 4625)) /* copy constructor was implicitly defined as deleted */                 \
-			__pragma(warning(disable : 4626)) /* assignment operator was implicitly defined as deleted */              \
-			__pragma(                                                                                                  \
-				warning(disable : 4686)) /* possible change in behavior, change in UDT return calling convention \     \
-										  * \                                                                    \     \
-										  */                                                                           \
+			__pragma(warning(disable : 4464))  /* relative include path contains '..' */                               \
+			__pragma(warning(disable : 4505))  /* unreferenced local function removed */                               \
+			__pragma(warning(disable : 4514))  /* unreferenced inline function has been removed */                     \
+			__pragma(warning(disable : 4582))  /* constructor is not implicitly called */                              \
+			__pragma(warning(disable : 4619))  /* there is no warning number 'XXXX' */                                 \
+			__pragma(warning(disable : 4623))  /* default constructor was implicitly defined as deleted */             \
+			__pragma(warning(disable : 4625))  /* copy constructor was implicitly defined as deleted */                \
+			__pragma(warning(disable : 4626))  /* assignment operator was implicitly defined as deleted */             \
+			__pragma(warning(disable : 4686))  /* possible change in behavior, change in UDT return callconv */        \
 			__pragma(warning(disable : 4710))  /* function not inlined */                                              \
 			__pragma(warning(disable : 4711))  /* function selected for automatic expansion */                         \
 			__pragma(warning(disable : 4820))  /* N bytes padding added */                                             \
 			__pragma(warning(disable : 4866))  /* compiler may not enforce left-to-right evaluation order for call */  \
 			__pragma(warning(disable : 4946))  /* reinterpret_cast used between related classes */                     \
 			__pragma(warning(disable : 5026))  /* move constructor was implicitly defined as deleted */                \
 			__pragma(warning(disable : 5027))  /* move assignment operator was implicitly defined as deleted */        \
@@ -711,14 +709,15 @@
 			__pragma(warning(disable : 1011)) /* missing return (false-positive) */                                    \
 			__pragma(warning(disable : 2261)) /* assume expr side-effects discarded */                                 \
 			static_assert(true)
 	#elif SOAGEN_GCC
 		#if SOAGEN_GCC >= 9
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_GCC_9                                                                 \
 				_Pragma("GCC diagnostic ignored \"-Wattributes\"")                                                     \
+				_Pragma("GCC diagnostic ignored \"-Wctor-dtor-privacy\"")                                              \
 				static_assert(true)
 		#else
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_GCC_9 static_assert(true)
 		#endif
 		#if SOAGEN_GCC >= 12
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_GCC_12                                                                \
 				_Pragma("GCC diagnostic ignored \"-Winterference-size\"")                                              \
@@ -833,14 +832,16 @@
 			SOAGEN_POP_WARNINGS;                                                                                       \
 			static_assert(true)
 	#else
 		#define SOAGEN_ENABLE_WARNINGS static_assert(true)
 	#endif
 #endif
 
+/// \brief Re-enables compiler warnings again after using #SOAGEN_DISABLE_WARNINGS.
+
 #ifndef SOAGEN_HAS_CONSTEVAL
 	#if defined(__cpp_consteval) && __cpp_consteval >= 201811 && (!SOAGEN_MSVC || SOAGEN_MSVC >= 1934)                 \
 		&& (!SOAGEN_CLANG || SOAGEN_CLANG >= 15)
 		#define SOAGEN_HAS_CONSTEVAL 1
 	#else
 		#define SOAGEN_HAS_CONSTEVAL SOAGEN_DOXYGEN
 	#endif
@@ -919,23 +920,49 @@
 					}                                                                                                  \
 				}                                                                                                      \
 			}                                                                                                          \
 			while (false)
 	#endif
 #endif
 
-#ifndef NDEBUG
-	#undef SOAGEN_ASSUME
-	#define SOAGEN_ASSUME(cond) SOAGEN_CONSTEXPR_SAFE_ASSERT(cond)
+#ifndef SOAGEN_COLUMN
+	#define SOAGEN_COLUMN(I)                                                                                           \
+		SOAGEN_PURE_INLINE_GETTER                                                                                      \
+		SOAGEN_ATTR(returns_nonnull)
+#endif
+
+#ifndef SOAGEN_ALIGNED_COLUMN
+	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
+		SOAGEN_COLUMN(I)                                                                                               \
+		SOAGEN_ATTR(assume_aligned(soagen::detail::actual_column_alignment<table_traits, allocator_type, I>))
 #endif
 
 #ifndef SOAGEN_ALWAYS_OPTIMIZE
 	#define SOAGEN_ALWAYS_OPTIMIZE 1
 #endif
 
+#ifndef SOAGEN_COMMA
+	#define SOAGEN_COMMA ,
+#endif
+
+#ifndef SOAGEN_HIDDEN
+	#if SOAGEN_DOXYGEN
+		#define SOAGEN_HIDDEN(...)
+		#define SOAGEN_HIDDEN_BASE(...)
+		#define SOAGEN_DOXYGEN_ONLY(...) __VA_ARGS__
+		#define SOAGEN_IF_DOXYGEN(A, B)	 A
+	#else
+		#define SOAGEN_HIDDEN(...) __VA_ARGS__
+		#define SOAGEN_HIDDEN_BASE(...)	: __VA_ARGS__
+		#define SOAGEN_DOXYGEN_ONLY(...)
+		#define SOAGEN_IF_DOXYGEN(A, B) B
+	#endif
+#endif
+#define SOAGEN_HIDDEN_PARAM(...) SOAGEN_HIDDEN(SOAGEN_COMMA __VA_ARGS__)
+
 #ifndef SOAGEN_DELETE_COPY
 	#define SOAGEN_DELETE_COPY(T)                                                                                      \
 		T(const T&)			   = delete;                                                                               \
 		T& operator=(const T&) = delete
 #endif
 
 #ifndef SOAGEN_DELETE_MOVE
@@ -964,8 +991,10 @@
 
 #ifndef SOAGEN_DEFAULT_RULE_OF_FIVE
 	#define SOAGEN_DEFAULT_RULE_OF_FIVE(T)                                                                             \
 		T() = default;                                                                                                 \
 		SOAGEN_DEFAULT_RULE_OF_FOUR(T)
 #endif
 
-#include "version.hpp"
+#if !defined(__POXY__) && !defined(POXY_IMPLEMENTATION_DETAIL)
+	#define POXY_IMPLEMENTATION_DETAIL(...) __VA_ARGS__
+#endif
```

### Comparing `soagen-0.0.1/src/soagen/hpp/soagen.hpp` & `soagen-0.1.0/src/soagen/hpp/single/soagen.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //----------------------------------------------------------------------------------------------------------------------
 //
-// soagen.hpp
+// soagen.hpp v0.1.0
 // https://github.com/marzer/soagen
 // SPDX-License-Identifier: MIT
 //
 //----------------------------------------------------------------------------------------------------------------------
 //     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //----------------------------------------------------------------------------------------------------------------------
 //
@@ -13,35 +13,34 @@
 // Copyright (c) Mark Gillard
 //
 // Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 // documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 // rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 // permit persons to whom the Software is furnished to do so, subject to the following conditions:
 //
-// The above copyright notice and this permission notice shall be included in all copies or substantial portions of
-// the Software.
+// The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
+// Software.
 //
-// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
-// THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-// AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
-// TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-// SOFTWARE.
+// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
+// WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+// COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+// OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 //
 //----------------------------------------------------------------------------------------------------------------------
 #ifndef SOAGEN_HPP
 #define SOAGEN_HPP
 
-//********  version.hpp  ***********************************************************************************************
+//********  generated/version.hpp  *************************************************************************************
 
 #define SOAGEN_VERSION_MAJOR  0
-#define SOAGEN_VERSION_MINOR  0
-#define SOAGEN_VERSION_PATCH  1
-#define SOAGEN_VERSION_STRING "0.0.1"
+#define SOAGEN_VERSION_MINOR  1
+#define SOAGEN_VERSION_PATCH  0
+#define SOAGEN_VERSION_STRING "0.1.0"
 
-//********  preprocessor.hpp  ******************************************************************************************
+//********  generated/preprocessor.hpp  ********************************************************************************
 
 #ifndef SOAGEN_CPP
 	#ifdef _MSVC_LANG
 		#if _MSVC_LANG > __cplusplus
 			#define SOAGEN_CPP _MSVC_LANG
 		#endif
 	#endif
@@ -444,24 +443,20 @@
 	#elif SOAGEN_CPP >= 20 && SOAGEN_HAS_CPP_ATTR(no_unique_address) >= 201803
 		#define SOAGEN_NO_UNIQUE_ADDRESS [[no_unique_address]]
 	#else
 		#define SOAGEN_NO_UNIQUE_ADDRESS
 	#endif
 #endif
 
-#ifndef SOAGEN_COLUMN
-	#define SOAGEN_COLUMN(I)                                                                                           \
-		SOAGEN_PURE_INLINE_GETTER                                                                                      \
-		SOAGEN_ATTR(returns_nonnull)
-#endif
-
-#ifndef SOAGEN_ALIGNED_COLUMN
-	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
-		SOAGEN_COLUMN(I)                                                                                               \
-		SOAGEN_ATTR(assume_aligned(soagen::detail::actual_column_alignment<table_traits, allocator_type, I>))
+#ifndef SOAGEN_HAS_EXCEPTIONS
+	#if defined(__EXCEPTIONS) || defined(_CPPUNWIND) || defined(__cpp_exceptions)
+		#define SOAGEN_HAS_EXCEPTIONS 1
+	#else
+		#define SOAGEN_HAS_EXCEPTIONS 0
+	#endif
 #endif
 
 #if defined(__cpp_constexpr) && __cpp_constexpr >= 202002L
 	#define SOAGEN_CPP20_CONSTEXPR constexpr
 #else
 	#define SOAGEN_CPP20_CONSTEXPR
 #endif
@@ -488,16 +483,18 @@
 	#else
 		#define SOAGEN_STD_CONCEPT(...) true
 	#endif
 #endif
 
 #ifndef SOAGEN_ENABLE_IF
 	#if !SOAGEN_DOXYGEN
-		#define SOAGEN_ENABLE_IF(...) , typename std::enable_if<!!(__VA_ARGS__), int>::type = 0
+		#define SOAGEN_ENABLE_IF_T(T, ...) std::enable_if_t<!!(__VA_ARGS__), T>
+		#define SOAGEN_ENABLE_IF(...)	   , SOAGEN_ENABLE_IF_T(int, __VA_ARGS__) = 0
 	#else
+		#define SOAGEN_ENABLE_IF_T(T, ...)
 		#define SOAGEN_ENABLE_IF(...)
 	#endif
 #endif
 
 #ifndef SOAGEN_CONSTRAINED_TEMPLATE
 	#if !SOAGEN_DOXYGEN
 		#define SOAGEN_CONSTRAINED_TEMPLATE(condition, ...)                                                            \
@@ -703,58 +700,55 @@
 			_Pragma("clang diagnostic ignored \"-Wcovered-switch-default\"")                                           \
 			_Pragma("clang diagnostic ignored \"-Wtautological-pointer-compare\"")                                     \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_8;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_9;                                                                      \
 			SOAGEN_DISABLE_SPAM_WARNINGS_CLANG_13;                                                                     \
 			static_assert(true)
 	#elif SOAGEN_MSVC
-		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                             \
-			__pragma(warning(disable : 4127))  /* conditional expr is constant */                                        \
-			__pragma(warning(disable : 4324))  /* structure was padded due to alignment specifier */                     \
-			__pragma(warning(disable : 4348))                                                                            \
-			__pragma(warning(disable : 4464))  /* relative include path contains '..' */                                 \
-			__pragma(warning(disable : 4505))  /* unreferenced local function removed */                                 \
-			__pragma(warning(disable : 4514))  /* unreferenced inline function has been removed */                       \
-			__pragma(warning(disable : 4582))  /* constructor is not implicitly called */                                \
-			__pragma(warning(disable : 4619))  /* there is no warning number 'XXXX' */                                   \
-			__pragma(warning(disable : 4623))  /* default constructor was implicitly defined as deleted */               \
-			__pragma(warning(disable : 4625))  /* copy constructor was implicitly defined as deleted */                  \
-			__pragma(warning(disable : 4626))  /* assignment operator was implicitly defined as deleted */               \
-			__pragma(warning(disable : 4686))  /* possible change in behavior, change in UDT return calling convention   \
-												* \     \                                                                \
-												* \                                                                    \ \
-												* \                                                                      \
-												*/                                                                       \
-			__pragma(warning(disable : 4710))  /* function not inlined */                                                \
-			__pragma(warning(disable : 4711))  /* function selected for automatic expansion */                           \
-			__pragma(warning(disable : 4820))  /* N bytes padding added */                                               \
-			__pragma(warning(disable : 4866))  /* compiler may not enforce left-to-right evaluation order for call */    \
-			__pragma(warning(disable : 4946))  /* reinterpret_cast used between related classes */                       \
-			__pragma(warning(disable : 5026))  /* move constructor was implicitly defined as deleted */                  \
-			__pragma(warning(disable : 5027))  /* move assignment operator was implicitly defined as deleted */          \
-			__pragma(warning(disable : 5039))  /* potentially throwing function passed to 'extern "C"' function */       \
-			__pragma(warning(disable : 5045))  /* Compiler will insert Spectre mitigation */                             \
-			__pragma(warning(disable : 5246))  /* initialization of a subobject should be wrapped in braces */           \
-			__pragma(warning(disable : 5264))  /* const variable is not used (false-positive) */                         \
-			__pragma(warning(disable : 26490)) /* cg: dont use reinterpret_cast */                                       \
-			__pragma(warning(disable : 26812)) /* cg: Prefer 'enum class' over 'enum' */                                 \
-			__pragma(warning(disable : 4848))  /* msvc::no_unique_address in C++17 is a vendor extension */              \
+		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                           \
+			__pragma(warning(disable : 4127))  /* conditional expr is constant */                                      \
+			__pragma(warning(disable : 4324))  /* structure was padded due to alignment specifier */                   \
+			__pragma(warning(disable : 4348))                                                                          \
+			__pragma(warning(disable : 4464))  /* relative include path contains '..' */                               \
+			__pragma(warning(disable : 4505))  /* unreferenced local function removed */                               \
+			__pragma(warning(disable : 4514))  /* unreferenced inline function has been removed */                     \
+			__pragma(warning(disable : 4582))  /* constructor is not implicitly called */                              \
+			__pragma(warning(disable : 4619))  /* there is no warning number 'XXXX' */                                 \
+			__pragma(warning(disable : 4623))  /* default constructor was implicitly defined as deleted */             \
+			__pragma(warning(disable : 4625))  /* copy constructor was implicitly defined as deleted */                \
+			__pragma(warning(disable : 4626))  /* assignment operator was implicitly defined as deleted */             \
+			__pragma(warning(disable : 4686))  /* possible change in behavior, change in UDT return callconv */        \
+			__pragma(warning(disable : 4710))  /* function not inlined */                                              \
+			__pragma(warning(disable : 4711))  /* function selected for automatic expansion */                         \
+			__pragma(warning(disable : 4820))  /* N bytes padding added */                                             \
+			__pragma(warning(disable : 4866))  /* compiler may not enforce left-to-right evaluation order for call */  \
+			__pragma(warning(disable : 4946))  /* reinterpret_cast used between related classes */                     \
+			__pragma(warning(disable : 5026))  /* move constructor was implicitly defined as deleted */                \
+			__pragma(warning(disable : 5027))  /* move assignment operator was implicitly defined as deleted */        \
+			__pragma(warning(disable : 5039))  /* potentially throwing function passed to 'extern "C"' function */     \
+			__pragma(warning(disable : 5045))  /* Compiler will insert Spectre mitigation */                           \
+			__pragma(warning(disable : 5246))  /* initialization of a subobject should be wrapped in braces */         \
+			__pragma(warning(disable : 5264))  /* const variable is not used (false-positive) */                       \
+			__pragma(warning(disable : 26490)) /* cg: dont use reinterpret_cast */                                     \
+			__pragma(warning(disable : 26812)) /* cg: Prefer 'enum class' over 'enum' */                               \
+			__pragma(warning(disable : 4848))  /* msvc::no_unique_address in C++17 is a vendor extension */            \
 			static_assert(true)
 	#elif SOAGEN_ICC
 		#define SOAGEN_DISABLE_SPAM_WARNINGS                                                                           \
 			__pragma(warning(disable : 82))	  /* storage class is not first */                                         \
 			__pragma(warning(disable : 111))  /* statement unreachable (false-positive) */                             \
 			__pragma(warning(disable : 869))  /* unreferenced parameter */                                             \
 			__pragma(warning(disable : 1011)) /* missing return (false-positive) */                                    \
 			__pragma(warning(disable : 2261)) /* assume expr side-effects discarded */                                 \
 			static_assert(true)
 	#elif SOAGEN_GCC
 		#if SOAGEN_GCC >= 9
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_GCC_9                                                                 \
 				_Pragma("GCC diagnostic ignored \"-Wattributes\"")                                                     \
+				_Pragma("GCC diagnostic ignored \"-Wctor-dtor-privacy\"")                                              \
 				static_assert(true)
 		#else
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_GCC_9 static_assert(true)
 		#endif
 		#if SOAGEN_GCC >= 12
 			#define SOAGEN_DISABLE_SPAM_WARNINGS_GCC_12                                                                \
 				_Pragma("GCC diagnostic ignored \"-Winterference-size\"")                                              \
@@ -955,23 +949,49 @@
 					}                                                                                                  \
 				}                                                                                                      \
 			}                                                                                                          \
 			while (false)
 	#endif
 #endif
 
-#ifndef NDEBUG
-	#undef SOAGEN_ASSUME
-	#define SOAGEN_ASSUME(cond) SOAGEN_CONSTEXPR_SAFE_ASSERT(cond)
+#ifndef SOAGEN_COLUMN
+	#define SOAGEN_COLUMN(I)                                                                                           \
+		SOAGEN_PURE_INLINE_GETTER                                                                                      \
+		SOAGEN_ATTR(returns_nonnull)
+#endif
+
+#ifndef SOAGEN_ALIGNED_COLUMN
+	#define SOAGEN_ALIGNED_COLUMN(I)                                                                                   \
+		SOAGEN_COLUMN(I)                                                                                               \
+		SOAGEN_ATTR(assume_aligned(soagen::detail::actual_column_alignment<table_traits, allocator_type, I>))
 #endif
 
 #ifndef SOAGEN_ALWAYS_OPTIMIZE
 	#define SOAGEN_ALWAYS_OPTIMIZE 1
 #endif
 
+#ifndef SOAGEN_COMMA
+	#define SOAGEN_COMMA ,
+#endif
+
+#ifndef SOAGEN_HIDDEN
+	#if SOAGEN_DOXYGEN
+		#define SOAGEN_HIDDEN(...)
+		#define SOAGEN_HIDDEN_BASE(...)
+		#define SOAGEN_DOXYGEN_ONLY(...) __VA_ARGS__
+		#define SOAGEN_IF_DOXYGEN(A, B)	 A
+	#else
+		#define SOAGEN_HIDDEN(...) __VA_ARGS__
+		#define SOAGEN_HIDDEN_BASE(...)	: __VA_ARGS__
+		#define SOAGEN_DOXYGEN_ONLY(...)
+		#define SOAGEN_IF_DOXYGEN(A, B) B
+	#endif
+#endif
+#define SOAGEN_HIDDEN_PARAM(...) SOAGEN_HIDDEN(SOAGEN_COMMA __VA_ARGS__)
+
 #ifndef SOAGEN_DELETE_COPY
 	#define SOAGEN_DELETE_COPY(T)                                                                                      \
 		T(const T&)			   = delete;                                                                               \
 		T& operator=(const T&) = delete
 #endif
 
 #ifndef SOAGEN_DELETE_MOVE
@@ -1000,20 +1020,25 @@
 
 #ifndef SOAGEN_DEFAULT_RULE_OF_FIVE
 	#define SOAGEN_DEFAULT_RULE_OF_FIVE(T)                                                                             \
 		T() = default;                                                                                                 \
 		SOAGEN_DEFAULT_RULE_OF_FOUR(T)
 #endif
 
-//********  core.hpp  **************************************************************************************************
+#if !defined(__POXY__) && !defined(POXY_IMPLEMENTATION_DETAIL)
+	#define POXY_IMPLEMENTATION_DETAIL(...) __VA_ARGS__
+#endif
+
+//********  generated/core.hpp  ****************************************************************************************
 
 SOAGEN_DISABLE_WARNINGS;
 #include <cstdint>
 #include <cstddef>
 #include <cstdlib>
+#include <cstring>
 #include <numeric>
 #include <type_traits>
 #include <new>
 #include <utility>
 #include <memory>
 #include <optional>
 SOAGEN_ENABLE_WARNINGS;
@@ -1077,15 +1102,15 @@
 		template <typename T, typename... U>
 		struct type_at_index_impl<0, T, U...>
 		{
 			using type = T;
 		};
 	}
 	template <size_t I, typename... T>
-	using type_at_index = typename detail::type_at_index_impl<I, T...>::type;
+	using type_at_index = POXY_IMPLEMENTATION_DETAIL(typename detail::type_at_index_impl<I, T...>::type);
 
 #endif
 
 	namespace detail
 	{
 		template <template <typename...> typename Trait, typename Enabler, typename... Args>
 		struct is_detected_impl : std::false_type
@@ -1117,30 +1142,40 @@
 #endif
 
 SOAGEN_POP_WARNINGS;
 
 //********  meta.hpp  **************************************************************************************************
 
 SOAGEN_DISABLE_WARNINGS;
+
 #ifndef SOAGEN_COLUMN_SPAN_TYPE
-	#if SOAGEN_CPP >= 20
+	#if defined(MUU_SPAN_H) || defined(MUU_SPAN_HPP)
+		#define SOAGEN_COLUMN_SPAN_TYPE				  muu::span
+		#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 1
+	#elif SOAGEN_CPP >= 20 && SOAGEN_HAS_INCLUDE(<span>)
 		#include <span>
 		#define SOAGEN_COLUMN_SPAN_TYPE std::span
 	#elif SOAGEN_HAS_INCLUDE(<muu/span.h>)
 		#include <muu/span.h>
-		#define SOAGEN_COLUMN_SPAN_TYPE muu::span
+		#define SOAGEN_COLUMN_SPAN_TYPE				  muu::span
+		#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 1
 	#elif SOAGEN_HAS_INCLUDE(<tcb/span.hpp>)
 		#include <tcb/span.hpp>
 		#define SOAGEN_COLUMN_SPAN_TYPE TCB_SPAN_NAMESPACE_NAME::span
 	#endif
 #endif
+#if defined(SOAGEN_COLUMN_SPAN_TYPE) && !defined(SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT)
+	#define SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT 0
+#endif
+
 #ifndef SOAGEN_OPTIONAL_TYPE
 	#include <optional>
 	#define SOAGEN_OPTIONAL_TYPE std::optional
 #endif
+
 SOAGEN_ENABLE_WARNINGS;
 
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
 
 #if SOAGEN_MSVC_LIKE
 	#pragma push_macro("min")
@@ -1157,20 +1192,75 @@
 		#pragma strict_gs_check(push, off)
 	#elif SOAGEN_GCC
 		#pragma GCC push_options
 		#pragma GCC optimize("O2")
 	#endif
 #endif
 
+#ifndef SOAGEN_MAKE_NAME
+	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
+                                                                                                                       \
+		struct name_constant_##Name                                                                                    \
+		{                                                                                                              \
+			static constexpr const char value[] = #Name;                                                               \
+		};                                                                                                             \
+                                                                                                                       \
+		template <typename Ref>                                                                                        \
+		struct named_ref_##Name                                                                                        \
+		{                                                                                                              \
+			Ref Name;                                                                                                  \
+                                                                                                                       \
+		  protected:                                                                                                   \
+			SOAGEN_PURE_INLINE_GETTER                                                                                  \
+			constexpr Ref get_ref_impl() const noexcept                                                                \
+			{                                                                                                          \
+				return static_cast<Ref>(Name);                                                                         \
+			}                                                                                                          \
+		}
+#endif
+
+#ifndef SOAGEN_MAKE_COL
+	#define SOAGEN_MAKE_COL(Table, Column, Name)                                                                       \
+		template <>                                                                                                    \
+		struct col_name_<Table, Column> : name_constant_##Name                                                         \
+		{};                                                                                                            \
+                                                                                                                       \
+		template <>                                                                                                    \
+		struct col_ref_<Table&, Column>                                                                                \
+			: named_ref_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, Column>>>                         \
+		{};                                                                                                            \
+                                                                                                                       \
+		template <>                                                                                                    \
+		struct col_ref_<Table&&, Column>                                                                               \
+			: named_ref_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, Column>>>                         \
+		{};                                                                                                            \
+                                                                                                                       \
+		template <>                                                                                                    \
+		struct col_ref_<const Table&, Column>                                                                          \
+			: named_ref_##Name<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>       \
+		{};                                                                                                            \
+                                                                                                                       \
+		template <>                                                                                                    \
+		struct col_ref_<const Table&&, Column>                                                                         \
+			: named_ref_##Name<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>       \
+		{}
+#endif
+
 namespace soagen
 {
 	template <typename T>
 	using remove_cvref = std::remove_cv_t<std::remove_reference_t<T>>;
 
 	template <typename T>
+	using make_cref = std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>;
+
+	template <typename T>
+	using coerce_ref = std::conditional_t<std::is_reference_v<T>, T, std::add_lvalue_reference_t<T>>;
+
+	template <typename T>
 	inline constexpr bool is_cv = !std::is_same_v<std::remove_cv_t<T>, T>;
 
 	template <typename T>
 	inline constexpr bool is_cvref = !std::is_same_v<remove_cvref<T>, T>;
 
 	template <typename T>
 	inline constexpr bool is_integer = std::is_integral_v<T> && !std::is_same_v<T, bool>;
@@ -1181,63 +1271,103 @@
 	template <typename T>
 	inline constexpr bool is_unsigned = is_integer<T> && std::is_unsigned_v<T>;
 
 	template <typename T, typename... U>
 	inline constexpr bool any_same = (false || ... || std::is_same_v<T, U>);
 
 	template <typename T>
-	inline constexpr bool is_soa = false; // specialized in generated code
-
+	inline constexpr bool is_soa = POXY_IMPLEMENTATION_DETAIL(false); // specialized in generated code
+	template <typename T>
+	inline constexpr bool is_soa<const T> = is_soa<T>;
+	template <typename T>
+	inline constexpr bool is_soa<volatile T> = is_soa<T>;
+	template <typename T>
+	inline constexpr bool is_soa<const volatile T> = is_soa<T>;
 	template <typename T>
 	inline constexpr bool is_implicit_lifetime_type =
 		std::is_scalar_v<T> || std::is_array_v<T>
 		|| (std::is_aggregate_v<T> && std::is_trivially_constructible_v<T> && std::is_trivially_destructible_v<T>);
 
 	template <auto Value>
-	using index_tag = std::integral_constant<size_t, static_cast<size_t>(Value)>;
+	using index_constant = std::integral_constant<size_t, static_cast<size_t>(Value)>;
+
+	template <typename T>
+	using forward_type = POXY_IMPLEMENTATION_DETAIL(
+		std::conditional_t<std::is_lvalue_reference_v<T>, T, std::add_rvalue_reference_t<T>>);
 
 #ifdef SOAGEN_COLUMN_SPAN_TYPE
 
-	template <typename T, size_t N = static_cast<size_t>(-1)>
-	using column_span = SOAGEN_COLUMN_SPAN_TYPE<T, N>;
+	#if SOAGEN_COLUMN_SPAN_SUPPORTS_ALIGNMENT
+
+	template <typename T, size_t Align = alignof(T)>
+	using column_span = SOAGEN_COLUMN_SPAN_TYPE<T, static_cast<size_t>(-1), Align>;
+
+	#else
+
+	template <typename T, size_t Align = alignof(T)>
+	using column_span = SOAGEN_COLUMN_SPAN_TYPE<T>;
+
+	#endif
 
-	template <typename T, size_t N = static_cast<size_t>(-1)>
-	using const_column_span = column_span<std::add_const_t<T>, N>;
+	template <typename T, size_t Align = alignof(T)>
+	using const_column_span = column_span<std::add_const_t<T>, Align>;
 
 #endif
 
+#if SOAGEN_DOXYGEN
+#else
 	using SOAGEN_OPTIONAL_TYPE;
+#endif
 
 	namespace detail
 	{
 		template <typename T>
 		using has_swap_member_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
 
 		template <typename T, typename Arg>
 		using has_resize_member_ = decltype(std::declval<T&>().resize(std::declval<const Arg&>()));
 
 		template <typename T, typename Arg>
 		using has_erase_member_ = decltype(std::declval<T&>().erase(std::declval<const Arg&>()));
 
 		template <typename T, typename Arg>
 		using has_unordered_erase_member_ = decltype(std::declval<T&>().unordered_erase(std::declval<const Arg&>()));
-	}
 
+		template <typename T>
+		using has_data_member_ = decltype(std::declval<T&>().data());
+
+		template <typename T, typename U>
+		using is_equality_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
+												 == std::declval<const std::remove_reference_t<U>&>());
+
+		template <typename T, typename U>
+		using is_less_than_comparable_ = decltype(std::declval<const std::remove_reference_t<T>&>()
+												  < std::declval<const std::remove_reference_t<U>&>());
+	}
 	template <typename T>
 	inline constexpr bool has_swap_member = is_detected<detail::has_swap_member_, T>;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_resize_member = is_detected<detail::has_resize_member_, T, Arg>;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_erase_member = is_detected<detail::has_erase_member_, T, Arg>;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_unordered_erase_member = is_detected<detail::has_unordered_erase_member_, T, Arg>;
 
+	template <typename T>
+	inline constexpr bool has_data_member = is_detected<detail::has_data_member_, T>;
+
+	template <typename T, typename U = T>
+	inline constexpr bool is_equality_comparable = is_detected<detail::is_equality_comparable_, T, U>;
+
+	template <typename T, typename U = T>
+	inline constexpr bool is_less_than_comparable = is_detected<detail::is_less_than_comparable_, T, U>;
+
 	namespace detail
 	{
 		template <typename T, bool = has_swap_member<T>>
 		struct has_nothrow_swap_member_ : std::bool_constant<noexcept(std::declval<T&>().swap(std::declval<T&>()))>
 		{};
 		template <typename T>
 		struct has_nothrow_swap_member_<T, false> : std::false_type
@@ -1262,94 +1392,204 @@
 		template <typename T, typename Arg, bool = has_unordered_erase_member<T, Arg>>
 		struct has_nothrow_unordered_erase_member_
 			: std::bool_constant<noexcept(std::declval<T&>().unordered_erase(std::declval<const Arg&>()))>
 		{};
 		template <typename T, typename Arg>
 		struct has_nothrow_unordered_erase_member_<T, Arg, false> : std::false_type
 		{};
-	}
 
+		template <typename T, bool = has_data_member<T>>
+		struct has_nothrow_data_member_ : std::bool_constant<noexcept(std::declval<T&>().data())>
+		{};
+		template <typename T>
+		struct has_nothrow_data_member_<T, false> : std::false_type
+		{};
+
+		template <typename T, typename U, bool = is_equality_comparable<T, U>>
+		struct is_nothrow_equality_comparable_
+			: std::bool_constant<noexcept(std::declval<const std::remove_reference_t<T>&>()
+										  == std::declval<const std::remove_reference_t<U>&>())>
+		{};
+		template <typename T, typename U>
+		struct is_nothrow_equality_comparable_<T, U, false> : std::false_type
+		{};
+
+		template <typename T, typename U, bool = is_less_than_comparable<T, U>>
+		struct is_nothrow_less_than_comparable_
+			: std::bool_constant<noexcept(std::declval<const std::remove_reference_t<T>&>()
+										  < std::declval<const std::remove_reference_t<U>&>())>
+		{};
+		template <typename T, typename U>
+		struct is_nothrow_less_than_comparable_<T, U, false> : std::false_type
+		{};
+	}
 	template <typename T>
 	inline constexpr bool has_nothrow_swap_member = detail::has_nothrow_swap_member_<T>::value;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_nothrow_resize_member = detail::has_nothrow_resize_member_<T, Arg>::value;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_nothrow_erase_member = detail::has_nothrow_erase_member_<T, Arg>::value;
 
 	template <typename T, typename Arg = size_t>
 	inline constexpr bool has_nothrow_unordered_erase_member =
 		detail::has_nothrow_unordered_erase_member_<T, Arg>::value;
 
-	// trait for determining the actual storage type for a column.
-	// we can strip off const/volatile and coerce all pointers to be void* to reduce template instantiation burden
+	template <typename T>
+	inline constexpr bool has_nothrow_data_member = detail::has_nothrow_data_member_<T>::value;
+
+	template <typename T, typename U = T>
+	inline constexpr bool is_nothrow_equality_comparable = detail::is_nothrow_equality_comparable_<T, U>::value;
+
+	template <typename T, typename U = T>
+	inline constexpr bool is_nothrow_less_than_comparable = detail::is_nothrow_less_than_comparable_<T, U>::value;
+
+	namespace detail
+	{
+		template <typename T>
+		struct table_type_
+		{
+			using type = typename T::table_type;
+		};
+	}
+	template <typename T>
+	using table_type = POXY_IMPLEMENTATION_DETAIL(typename detail::table_type_<std::remove_cv_t<T>>::type);
+
+	namespace detail
+	{
+		template <typename T>
+		struct table_traits_type_
+		{
+			using type = typename T::table_traits;
+		};
+	}
+	template <typename T>
+	using table_traits_type =
+		POXY_IMPLEMENTATION_DETAIL(typename detail::table_traits_type_<std::remove_cv_t<T>>::type);
+
+	namespace detail
+	{
+		template <typename T>
+		struct allocator_type_
+		{
+			using type = typename T::allocator_type;
+		};
+	}
+	template <typename T>
+	using allocator_type = POXY_IMPLEMENTATION_DETAIL(typename detail::allocator_type_<std::remove_cv_t<T>>::type);
+
+	template <typename T, size_t Column>
+	using value_type = POXY_IMPLEMENTATION_DETAIL(typename table_traits_type<T>::template column<Column>::value_type);
+
 	namespace detail
 	{
 		template <typename ValueType>
 		struct storage_type_
 		{
 			using type = ValueType;
 		};
+		// store all pointers as void*
 		template <typename T>
 		struct storage_type_<T*>
 		{
 			using type = void*;
 		};
 		template <typename T>
 		struct storage_type_<const T*> : public storage_type_<T*>
 		{};
 		template <typename T>
 		struct storage_type_<volatile T*> : public storage_type_<T*>
 		{};
 		template <typename T>
 		struct storage_type_<const volatile T*> : public storage_type_<T*>
 		{};
+		// strip off const and volatile
 		template <typename T>
 		struct storage_type_<const T> : public storage_type_<T>
 		{};
 		template <typename T>
 		struct storage_type_<volatile T> : public storage_type_<T>
 		{};
 		template <typename T>
 		struct storage_type_<const volatile T> : public storage_type_<T>
 		{};
+		// store byte-like types as std::byte (since these pointers can legally alias each other)
+		template <>
+		struct storage_type_<char> : public storage_type_<std::byte>
+		{};
+		template <>
+		struct storage_type_<unsigned char> : public storage_type_<std::byte>
+		{};
 	}
 	template <typename ValueType>
-	using storage_type = typename detail::storage_type_<ValueType>::type;
+	using storage_type = POXY_IMPLEMENTATION_DETAIL(typename detail::storage_type_<ValueType>::type);
 
-	// trait for determining the default parameter type for a column.
-	// ideally we want to pass small+fast things by value, move-only things by rvalue,
-	// and everything else as const lvalue.
 	namespace detail
 	{
-		template <typename ValueType,
-				  bool Value = std::is_scalar_v<ValueType>		//
-							|| std::is_fundamental_v<ValueType> //
-							|| (std::is_trivially_copyable_v<ValueType> && sizeof(ValueType) <= sizeof(void*) * 2),
-				  bool Move = !std::is_copy_constructible_v<ValueType> && std::is_move_constructible_v<ValueType>>
+		template <typename T>
 		struct param_type_
 		{
-			using type = ValueType;
+			static_assert(!std::is_reference_v<T>);
+
+			using type = std::conditional_t<
+				// move-only types
+				!std::is_copy_constructible_v<T> && std::is_move_constructible_v<T>,
+				std::add_rvalue_reference_t<std::remove_cv_t<T>>,
+				std::conditional_t<
+					// small + trivial types
+					std::is_scalar_v<T> || std::is_fundamental_v<T>
+						|| (std::is_trivially_copyable_v<T> && sizeof(T) <= sizeof(void*) * 2),
+					std::remove_cv_t<T>,
+					// everything else
+					std::add_lvalue_reference_t<std::add_const_t<T>>>>;
 		};
-		template <typename ValueType>
-		struct param_type_<ValueType, false, true>
+		// references are kept as-is
+		template <typename T>
+		struct param_type_<T&>
 		{
-			using type = std::add_rvalue_reference_t<ValueType>;
+			using type = T&;
 		};
-		template <typename ValueType>
-		struct param_type_<ValueType, false, false>
+		template <typename T>
+		struct param_type_<T&&>
 		{
-			using type = std::add_lvalue_reference_t<std::add_const_t<ValueType>>;
+			using type = T&&;
 		};
+		// ... except const rvalues, which are converted to const lvalues (because const T&& is nonsense)
+		template <typename T>
+		struct param_type_<const T&&> : param_type_<const T&>
+		{};
+		template <typename T>
+		struct param_type_<const volatile T&&> : param_type_<const volatile T&>
+		{};
 	}
 	template <typename ValueType>
-	using param_type = typename detail::param_type_<ValueType>::type;
+	using param_type = POXY_IMPLEMENTATION_DETAIL(typename detail::param_type_<ValueType>::type);
+
+	namespace detail
+	{
+		template <typename T>
+		struct rvalue_type_
+		{
+			using type = std::conditional_t<
+				// if the param_type of unreferenced, unqualified T would be a value or an rvalue, use that
+				std::is_rvalue_reference_v<param_type<remove_cvref<T>>>
+					|| !std::is_reference_v<param_type<remove_cvref<T>>>,
+				param_type<remove_cvref<T>>,
+				std::conditional_t<
+					// copy-only things
+					!std::is_move_constructible_v<remove_cvref<T>>,
+					std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>,
+					// rvalues
+					std::add_rvalue_reference_t<remove_cvref<T>>>>;
+		};
+	}
+	template <typename ParamType>
+	using rvalue_type = POXY_IMPLEMENTATION_DETAIL(typename detail::rvalue_type_<ParamType>::type);
 
-	// utility class for passing multiple variadic packs through to emplace
 	template <typename... Args>
 	struct emplacer
 	{
 		static_assert(sizeof...(Args));
 		static_assert((std::is_reference_v<Args> && ...));
 
 		void* ptrs[sizeof...(Args)];
@@ -1357,23 +1597,290 @@
 		SOAGEN_DEFAULT_RULE_OF_FIVE(emplacer);
 
 		SOAGEN_NODISCARD_CTOR
 		constexpr emplacer(Args&&... args) noexcept //
 			: ptrs{ const_cast<void*>(static_cast<const volatile void*>(&args))... }
 		{}
 	};
+
 	template <>
 	struct emplacer<>
 	{};
 	template <typename... Args>
 	emplacer(Args&&...) -> emplacer<Args&&...>;
 	template <typename T>
-	inline constexpr bool is_emplacer = false;
+	inline constexpr bool is_emplacer = POXY_IMPLEMENTATION_DETAIL(false);
 	template <typename... T>
 	inline constexpr bool is_emplacer<emplacer<T...>> = true;
+	template <typename T>
+	inline constexpr bool is_emplacer<const T> = is_emplacer<T>;
+	template <typename T>
+	inline constexpr bool is_emplacer<volatile T> = is_emplacer<T>;
+	template <typename T>
+	inline constexpr bool is_emplacer<const volatile T> = is_emplacer<T>;
+	template <typename Func, typename Arg, typename OptArg>
+	inline constexpr bool is_invocable_with_optarg = std::is_invocable_v<Func, Arg, OptArg> //
+												  || std::is_invocable_v<Func, OptArg, Arg> //
+												  || std::is_invocable_v<Func, Arg>;
+
+	template <typename Func, typename Arg, typename OptArg>
+	inline constexpr bool is_nothrow_invocable_with_optarg =
+		std::is_invocable_v<Func, Arg, OptArg>
+			? std::is_nothrow_invocable_v<Func, Arg, OptArg>
+			: (std::is_invocable_v<Func, OptArg, Arg> ? std::is_nothrow_invocable_v<Func, OptArg, Arg>
+													  : std::is_nothrow_invocable_v<Func, Arg>);
+
+	template <typename Func, typename Arg, typename OptArg>
+	SOAGEN_ALWAYS_INLINE
+	constexpr decltype(auto) invoke_with_optarg(Func&& func, Arg&& arg, [[maybe_unused]] OptArg&& optarg) //
+		noexcept(is_nothrow_invocable_with_optarg<Func&&, Arg&&, OptArg&&>)
+	{
+		if constexpr (std::is_invocable_v<Func&&, Arg&&, OptArg&&>)
+		{
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg), static_cast<OptArg&&>(optarg));
+		}
+		else if constexpr (std::is_invocable_v<Func&&, OptArg&&, Arg&&>)
+		{
+			return static_cast<Func&&>(func)(static_cast<OptArg&&>(optarg), static_cast<Arg&&>(arg));
+		}
+		else
+		{
+			static_assert(std::is_invocable_v<Func&&, Arg&&>);
+
+			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
+		}
+	}
+
+	namespace detail
+	{
+		template <typename Table, size_t ColumnIndex>
+		struct col_name_;
+		template <typename Table, size_t ColumnIndex>
+		struct col_ref_;
+
+		template <typename A, typename B>
+		inline constexpr bool same_table_type =
+			std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>;
+	}
+}
+
+namespace std
+{
+	template <typename... Args>
+	struct tuple_size<soagen::emplacer<Args...>> //
+		: std::integral_constant<size_t, sizeof...(Args)>
+	{};
+}
+
+#if SOAGEN_ALWAYS_OPTIMIZE
+	#if SOAGEN_MSVC
+		#pragma strict_gs_check(pop)
+		#pragma runtime_checks("", restore)
+		#pragma optimize("", on)
+		#pragma inline_recursion(off)
+	#elif SOAGEN_GCC
+		#pragma GCC pop_options
+	#endif
+#endif
+
+#if SOAGEN_MSVC_LIKE
+	#pragma pop_macro("min")
+	#pragma pop_macro("max")
+#endif
+
+SOAGEN_POP_WARNINGS;
+
+//********  row.hpp  ***************************************************************************************************
+
+SOAGEN_PUSH_WARNINGS;
+SOAGEN_DISABLE_SPAM_WARNINGS;
+
+#if SOAGEN_MSVC_LIKE
+	#pragma push_macro("min")
+	#pragma push_macro("max")
+	#undef min
+	#undef max
+#endif
+
+#if SOAGEN_ALWAYS_OPTIMIZE
+	#if SOAGEN_MSVC
+		#pragma inline_recursion(on)
+		#pragma optimize("gt", on)
+		#pragma runtime_checks("", off)
+		#pragma strict_gs_check(push, off)
+	#elif SOAGEN_GCC
+		#pragma GCC push_options
+		#pragma GCC optimize("O2")
+	#endif
+#endif
+
+namespace soagen
+{
+	template <typename Table, size_t... Columns>
+	struct SOAGEN_EMPTY_BASES row //
+	SOAGEN_HIDDEN_BASE(public detail::col_ref_<Table, Columns>...)
+	{
+		static_assert(std::is_reference_v<Table>,
+					  "Table must be a reference so row members can derive their reference category");
+
+		// columns:
+
+		template <size_t Column>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr decltype(auto) column() const noexcept
+		{
+			static_assert(Column < table_traits_type<remove_cvref<Table>>::column_count, "column index out of range");
+
+			return detail::col_ref_<Table, Column>::get_ref_impl();
+		}
+
+		// tuple protocol:
+
+		template <size_t Member>
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr decltype(auto) get() const noexcept
+		{
+			static_assert(Member < sizeof...(Columns), "member index out of range");
+
+			return type_at_index<Member, detail::col_ref_<Table, Columns>...>::get_ref_impl();
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
+									typename T)
+		SOAGEN_NODISCARD
+		friend constexpr bool operator==(const row& lhs, const row<T, Columns...>& rhs) //
+			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
+		{
+			return ((lhs.template column<Columns>() == rhs.template column<Columns>()) && ...);
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
+									typename T)
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator!=(const row& lhs, const row<T, Columns...>& rhs) //
+			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_equality_comparable)
+		{
+			return !(lhs == rhs);
+		}
+
+	  private:
+		template <size_t Member, typename T>
+		SOAGEN_NODISCARD
+		static constexpr int row_compare_impl(const row& lhs, const row<T, Columns...>& rhs) //
+			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+		{
+			if (lhs.template get<Member>() < rhs.template get<Member>())
+				return -1;
+
+			if (rhs.template get<Member>() < lhs.template get<Member>())
+				return 1;
+
+			if constexpr (Member + 1u == sizeof...(Columns))
+				return 0;
+			else
+				return row_compare_impl<Member + 1u>(lhs, rhs);
+		}
+
+	  public:
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+									typename T)
+		SOAGEN_NODISCARD
+		friend constexpr bool operator<(const row& lhs, const row<T, Columns...>& rhs) //
+			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+		{
+			return row_compare_impl<0>(lhs, rhs) < 0;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+									typename T)
+		SOAGEN_NODISCARD
+		friend constexpr bool operator<=(const row& lhs, const row<T, Columns...>& rhs) //
+			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+		{
+			return row_compare_impl<0>(lhs, rhs) <= 0;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+									typename T)
+		SOAGEN_NODISCARD
+		friend constexpr bool operator>(const row& lhs, const row<T, Columns...>& rhs) //
+			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+		{
+			return row_compare_impl<0>(lhs, rhs) > 0;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
+									 && table_traits_type<remove_cvref<Table>>::all_less_than_comparable),
+									typename T)
+		SOAGEN_NODISCARD
+		friend constexpr bool operator>=(const row& lhs, const row<T, Columns...>& rhs) //
+			noexcept(table_traits_type<remove_cvref<Table>>::all_nothrow_less_than_comparable)
+		{
+			return row_compare_impl<0>(lhs, rhs) >= 0;
+		}
+	};
+
+	template <typename T>
+	inline constexpr bool is_row = POXY_IMPLEMENTATION_DETAIL(false);
+	template <typename Table, size_t... Columns>
+	inline constexpr bool is_row<row<Table, Columns...>> = true;
+	template <typename T>
+	inline constexpr bool is_row<const T> = is_row<T>;
+	template <typename T>
+	inline constexpr bool is_row<volatile T> = is_row<T>;
+	template <typename T>
+	inline constexpr bool is_row<const volatile T> = is_row<T>;
+	namespace detail
+	{
+		template <typename Table, size_t... Columns>
+		struct table_type_<row<Table, Columns...>>
+		{
+			using type = remove_cvref<Table>;
+		};
+		template <typename Table, size_t... Columns>
+		struct table_traits_type_<row<Table, Columns...>>
+		{
+			using type = table_traits_type<remove_cvref<Table>>;
+		};
+
+		template <typename Table, typename IndexSequence>
+		struct row_type_;
+		template <typename Table, size_t... Columns>
+		struct row_type_<Table, std::index_sequence<Columns...>>
+		{
+			using type = row<Table, Columns...>;
+		};
+		template <typename Table>
+		struct row_type_<Table, std::index_sequence<>>
+			: row_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
+		{};
+	}
+	template <typename Table, size_t... Columns>
+	using row_type = POXY_IMPLEMENTATION_DETAIL(
+		typename detail::row_type_<coerce_ref<Table>, std::index_sequence<Columns...>>::type);
+}
+
+namespace std
+{
+	template <typename Table, size_t... Columns>
+	struct tuple_size<soagen::row<Table, Columns...>> //
+		: std::integral_constant<size_t, sizeof...(Columns)>
+	{};
+
+	template <size_t Member, typename Table, size_t... Columns>
+	struct tuple_element<Member, soagen::row<Table, Columns...>>
+	{
+		using type = decltype(std::declval<soagen::row<Table, Columns...>>().template get<Member>());
+	};
 }
 
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
@@ -1386,15 +1893,15 @@
 #if SOAGEN_MSVC_LIKE
 	#pragma pop_macro("min")
 	#pragma pop_macro("max")
 #endif
 
 SOAGEN_POP_WARNINGS;
 
-//********  compressed_pair.hpp  ***************************************************************************************
+//********  generated/compressed_pair.hpp  *****************************************************************************
 
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
 
 #if SOAGEN_MSVC_LIKE
 	#pragma push_macro("min")
 	#pragma push_macro("max")
@@ -1674,15 +2181,15 @@
 #if SOAGEN_MSVC_LIKE
 	#pragma pop_macro("min")
 	#pragma pop_macro("max")
 #endif
 
 SOAGEN_POP_WARNINGS;
 
-//********  functions.hpp  *********************************************************************************************
+//********  generated/functions.hpp  ***********************************************************************************
 
 #if SOAGEN_CPP >= 20 && defined(__cpp_lib_bit_cast) && __cpp_lib_bit_cast >= 201806
 	#include <bit>
 #endif
 
 SOAGEN_PUSH_WARNINGS;
 SOAGEN_DISABLE_SPAM_WARNINGS;
@@ -1966,63 +2473,76 @@
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 namespace soagen
 {
 	struct allocator
 	{
-		using value_type							 = std::byte;
-		using pointer								 = value_type*;
-		using const_pointer							 = const value_type*;
-		using void_pointer							 = std::byte*;
-		using const_void_pointer					 = const std::byte*;
-		using size_type								 = size_t;
-		using difference_type						 = ptrdiff_t;
-		using is_always_equal						 = std::true_type;
+		using value_type		 = std::byte;
+		using pointer			 = value_type*;
+		using const_pointer		 = const value_type*;
+		using void_pointer		 = std::byte*;
+		using const_void_pointer = const std::byte*;
+		using size_type			 = size_t;
+		using difference_type	 = ptrdiff_t;
+
+		using is_always_equal = std::true_type;
+
 		using propagate_on_container_copy_assignment = std::false_type;
+
 		using propagate_on_container_move_assignment = std::false_type;
-		using propagate_on_container_swap			 = std::false_type;
+
+		using propagate_on_container_swap = std::false_type;
 
 		static constexpr size_t min_alignment =
 			max(size_t{ __STDCPP_DEFAULT_NEW_ALIGNMENT__ }, alignof(std::max_align_t), alignof(value_type));
+		static_assert(has_single_bit(min_alignment));
 
 		SOAGEN_NODISCARD
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_DECLSPEC(noalias)
 		SOAGEN_DECLSPEC(restrict)
 		SOAGEN_ATTR(assume_aligned(min_alignment))
 		SOAGEN_ATTR(returns_nonnull)
 		SOAGEN_ATTR(malloc)
 		value_type* allocate(size_t size, std::align_val_t alignment = std::align_val_t{ min_alignment })
 		{
+			SOAGEN_ASSUME(size);
+			SOAGEN_ASSUME(static_cast<size_t>(alignment));
+
+			size	  = (size + static_cast<size_t>(alignment) - 1u) & ~(static_cast<size_t>(alignment) - 1u);
+			alignment = std::align_val_t{ max(static_cast<size_t>(alignment), min_alignment) };
+
+			SOAGEN_ASSUME((static_cast<size_t>(alignment) & (static_cast<size_t>(alignment) - 1u)) == 0u);
+
 #if SOAGEN_WINDOWS
-			auto ptr = _aligned_malloc(size, max(static_cast<size_t>(alignment), min_alignment));
+			auto ptr = _aligned_malloc(size, static_cast<size_t>(alignment));
 #else
-			auto ptr = std::aligned_alloc(max(static_cast<size_t>(alignment), min_alignment), size);
+			auto ptr = std::aligned_alloc(static_cast<size_t>(alignment), size);
 #endif
-			if (!ptr)
+			if SOAGEN_UNLIKELY(!ptr)
 				throw std::bad_alloc{};
 
 			return soagen::assume_aligned<min_alignment>(static_cast<pointer>(ptr));
 		}
 
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_ATTR(nonnull)
-		void deallocate(value_type* ptr, size_t /* size */) noexcept
+		void deallocate(value_type* ptr, [[maybe_unused]] size_t size) noexcept
 		{
 			SOAGEN_ASSUME(ptr != nullptr);
+			SOAGEN_ASSUME(size);
 
 #if SOAGEN_WINDOWS
 			_aligned_free(ptr);
 #else
 			std::free(ptr);
 #endif
 		}
 
-	  private:
 		SOAGEN_CONST_INLINE_GETTER
 		friend bool operator==(const allocator&, const allocator&) noexcept
 		{
 			return true;
 		}
 
 		SOAGEN_CONST_INLINE_GETTER
@@ -2097,15 +2617,16 @@
 			static constexpr bool container_move_assign_always_takes_ownership =
 				base_traits::propagate_on_container_move_assignment::value || base_traits::is_always_equal::value;
 		};
 	}
 
 	// primary template - allocator has an aligned-allocation overload
 	template <typename Allocator, bool = detail::has_aligned_allocate<Allocator>>
-	struct allocator_traits : public detail::allocator_traits_base<Allocator>
+	struct allocator_traits //
+		: public detail::allocator_traits_base<Allocator>
 	{
 		using base_traits = detail::allocator_traits_base<Allocator>;
 		using typename base_traits::value_type;
 		using typename base_traits::size_type;
 
 		SOAGEN_NODISCARD
 		SOAGEN_DECLSPEC(noalias)
@@ -2120,15 +2641,16 @@
 				alloc.allocate(num,
 							   std::align_val_t{ max(static_cast<size_t>(alignment), base_traits::min_alignment) }));
 		}
 	};
 
 	// secondary template - we have to implement the alignment management manually :(:(
 	template <typename Allocator>
-	struct allocator_traits<Allocator, false> : public detail::allocator_traits_base<Allocator>
+	struct allocator_traits<Allocator, false> //
+		: public detail::allocator_traits_base<Allocator>
 	{
 		using base_traits = detail::allocator_traits_base<Allocator>;
 		using typename base_traits::value_type;
 		using typename base_traits::size_type;
 		using typename base_traits::pointer;
 
 	  private:
@@ -2280,26 +2802,26 @@
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 202207
 			}
 #endif
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& default_construct_at(std::byte* buffer, size_t element_index) //
+		static constexpr storage_type& default_construct(std::byte* buffer, size_t element_index) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			return default_construct(buffer + element_index * sizeof(storage_type));
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_default_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
-		static void default_construct_at(std::byte* buffer, size_t start_index, size_t count) //
+		static void default_construct(std::byte* buffer, size_t start_index, size_t count) //
 			noexcept(std::is_nothrow_default_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 			SOAGEN_ASSUME(count);
 
 #if defined(__cpp_lib_start_lifetime_as) && __cpp_lib_start_lifetime_as >= 2022071
 			if constexpr (is_implicit_lifetime_type<storage_type>)
@@ -2309,121 +2831,172 @@
 			}
 			else
 #endif
 				if constexpr (std::is_nothrow_default_constructible_v<storage_type>
 							  || std::is_trivially_destructible_v<storage_type>)
 			{
 				for (const size_t e = start_index + count; start_index < e; start_index++)
-					default_construct_at(buffer, start_index);
+					default_construct(buffer, start_index);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = start_index;
 
 				try
 				{
 					for (const size_t e = start_index + count; i < e; i++)
-						default_construct_at(buffer, i);
+						default_construct(buffer, i);
 				}
 				catch (...)
 				{
 					for (; i-- > start_index;)
-						destruct_at(buffer, i);
+						destruct(buffer, i);
 					throw;
 				}
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_copyable = std::is_trivially_copyable_v<storage_type>;
+
+	  private:
+		// note: these *should* just be regular variable templates but evidently GCC
+		// chokes on partial variable template specialization at class scope:
+		// https://gcc.gnu.org/bugzilla/show_bug.cgi?id=71954
+
+		template <typename... Args>
+		struct is_constructible_with_memcpy_ : std::false_type
+		{};
+		template <typename Arg>
+		struct is_constructible_with_memcpy_<Arg>
+			: std::bool_constant<sizeof(storage_type) == sizeof(remove_cvref<Arg>)	//
+								 && is_trivially_copyable							//
+								 && is_implicit_lifetime_type<storage_type>			//
+								 && std::is_trivially_copyable_v<remove_cvref<Arg>> //
+								 && (std::is_same_v<storage_type, remove_cvref<Arg>>
+									 || (any_same<storage_type, char, unsigned char, std::byte>
+										 && any_same<remove_cvref<Arg>, char, unsigned char, std::byte>)
+									 || (std::is_same_v<storage_type, void*> && std::is_pointer_v<remove_cvref<Arg>>))>
+		{};
+
+	  public:
+		template <typename... Args>
+		static constexpr bool is_constructible_with_memcpy = is_constructible_with_memcpy_<Args...>::value;
+
 		template <typename... Args>
-		static constexpr bool is_constructible = std::is_constructible_v<storage_type, Args&&...>;
+		static constexpr bool is_trivially_constructible =
+			is_constructible_with_memcpy<Args...>
+			|| std::is_trivially_constructible_v<storage_type, remove_cvref<Args>...>;
+
+	  private:
+		template <typename... Args>
+		struct is_constructible_
+			: std::bool_constant<is_trivially_constructible<Args...> || std::is_constructible_v<storage_type, Args...>>
+		{};
 		template <typename T>
-		static constexpr bool is_constructible<T*&> = std::is_same_v<storage_type, void*>;
+		struct is_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
+														  || is_trivially_constructible<T*>	  //
+														  || std::is_constructible_v<storage_type, T*>>
+		{};
+		template <typename T>
+		struct is_constructible_<T*&> : std::bool_constant<std::is_same_v<storage_type, void*> //
+														   || is_trivially_constructible<T*&>  //
+														   || std::is_constructible_v<storage_type, T*&>>
+		{};
 		template <typename T>
-		static constexpr bool is_constructible<T*&&> = std::is_same_v<storage_type, void*>;
+		struct is_constructible_<T*&&> : std::bool_constant<std::is_same_v<storage_type, void*> //
+															|| is_trivially_constructible<T*&&> //
+															|| std::is_constructible_v<storage_type, T*&&>>
+		{};
+		template <typename... Args>
+		struct is_constructible_<emplacer<Args...>&&> : is_constructible_<Args...>
+		{};
+
+	  public:
 		template <typename... Args>
-		static constexpr bool is_constructible<emplacer<Args...>&&> = is_constructible<Args...>;
+		static constexpr bool is_constructible = is_constructible_<Args...>::value;
 
+	  private:
 		template <typename... Args>
-		static constexpr bool is_nothrow_constructible = std::is_nothrow_constructible_v<storage_type, Args&&...>;
+		struct is_nothrow_constructible_ : std::bool_constant<is_trivially_constructible<Args...>
+															  || std::is_nothrow_constructible_v<storage_type, Args...>>
+		{};
 		template <typename T>
-		static constexpr bool is_nothrow_constructible<T*&> = std::is_same_v<storage_type, void*>;
+		struct is_nothrow_constructible_<T*> : std::bool_constant<std::is_same_v<storage_type, void*> //
+																  || is_trivially_constructible<T*>	  //
+																  || std::is_nothrow_constructible_v<storage_type, T*>>
+		{};
+		template <typename T>
+		struct is_nothrow_constructible_<T*&>
+			: std::bool_constant<std::is_same_v<storage_type, void*> //
+								 || is_trivially_constructible<T*&>	 //
+								 || std::is_nothrow_constructible_v<storage_type, T*&>>
+		{};
 		template <typename T>
-		static constexpr bool is_nothrow_constructible<T*&&> = std::is_same_v<storage_type, void*>;
+		struct is_nothrow_constructible_<T*&&>
+			: std::bool_constant<std::is_same_v<storage_type, void*> //
+								 || is_trivially_constructible<T*&&> //
+								 || std::is_nothrow_constructible_v<storage_type, T*&&>>
+		{};
 		template <typename... Args>
-		static constexpr bool is_nothrow_constructible<emplacer<Args...>&&> = is_constructible<Args...>;
+		struct is_nothrow_constructible_<emplacer<Args...>&&> : is_nothrow_constructible_<Args...>
+		{};
+
+	  public:
+		template <typename... Args>
+		static constexpr bool is_nothrow_constructible = is_nothrow_constructible_<Args...>::value;
 
 	  private:
 		template <typename... Args, size_t... Indices>
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct_from_emplacer(std::byte* destination,
 															   emplacer<Args...>&& args,
 															   std::index_sequence<Indices...>) //
 			noexcept(is_nothrow_constructible<Args...>)
 		{
-			static_assert(sizeof...(Args) == sizeof...(Indices));
 			static_assert((std::is_reference_v<Args> && ...));
+			static_assert(sizeof...(Args) == sizeof...(Indices));
+			SOAGEN_ASSUME(destination != nullptr);
 
-			if constexpr (std::is_aggregate_v<storage_type>)
-			{
-				return *(
-					::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-						storage_type{ static_cast<Args>(
-							*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(args.ptrs[Indices]))... });
-			}
-			else
-			{
-				return *(
-					::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-						storage_type(static_cast<Args>(
-							*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(args.ptrs[Indices]))...));
-			}
+			return construct(destination,
+							 static_cast<Args>(*static_cast<std::add_pointer_t<std::remove_reference_t<Args>>>(
+								 args.ptrs[Indices]))...);
 		}
 
 	  public:
-		template <typename... Args>
-		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& construct_from_emplacer(std::byte* destination,
-															   emplacer<Args...>&& args) //
-			noexcept(is_nothrow_constructible<Args...>)
-		{
-			static_assert((std::is_reference_v<Args> && ...));
-
-			return construct_from_emplacer(destination,
-										   static_cast<emplacer<Args...>&&>(args),
-										   std::make_index_sequence<sizeof...(Args)>{});
-		}
-
 		SOAGEN_CONSTRAINED_TEMPLATE(is_constructible<Args&&...>, typename... Args)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& construct(std::byte* destination, Args&&... args) //
 			noexcept(is_nothrow_constructible<Args&&...>)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 
 			if constexpr (sizeof...(Args) == 0)
 			{
 				return default_construct(destination);
 			}
 			else
 			{
-				if constexpr (sizeof...(Args) == 1										   //
-							  && (std::is_pointer_v<std::remove_reference_t<Args>> && ...) //
-							  && std::is_same_v<storage_type, void*>)
+				if constexpr (sizeof...(Args) == 1 && (is_emplacer<std::remove_reference_t<Args>> && ...))
 				{
-					return *(
-						::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
-							storage_type{ const_cast<storage_type>(reinterpret_cast<const volatile void*>(args))... });
+					return construct_from_emplacer(
+						destination,
+						static_cast<Args&&>(args)...,
+						std::make_index_sequence<std::tuple_size_v<remove_cvref<Args>>>{}...);
 				}
-				else if constexpr (sizeof...(Args) == 1 && (is_emplacer<std::remove_reference_t<Args>> && ...))
+				else if constexpr (is_constructible_with_memcpy<Args&&...>)
 				{
-					return construct_from_emplacer(destination, static_cast<Args&&>(args)...);
+					std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
+								soagen::assume_aligned<alignof(storage_type)>(&args)...,
+								sizeof(storage_type));
+
+					return get(destination);
 				}
 				else if constexpr (std::is_aggregate_v<storage_type>)
 				{
 					return *(::new (static_cast<void*>(soagen::assume_aligned<alignof(storage_type)>(destination)))
 								 storage_type{ static_cast<Args&&>(args)... });
 				}
 				else
@@ -2449,39 +3022,39 @@
 			{
 				return construct(buffer + element_index * sizeof(storage_type), static_cast<Args&&>(args)...);
 			}
 		}
 
 		//--- move-construction ----------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_move_constructible = is_trivially_constructible<storage_type&&>;
+
 		static constexpr bool is_move_constructible =
-			std::is_move_constructible_v<storage_type>
+			is_trivially_move_constructible				  //
+			|| std::is_move_constructible_v<storage_type> //
 			|| (std::is_default_constructible_v<storage_type> && std::is_move_assignable_v<storage_type>);
 
-		static constexpr bool is_nothrow_move_constructible = std::is_move_constructible_v<storage_type>
-																? std::is_nothrow_move_constructible_v<storage_type>
-																: (std::is_nothrow_default_constructible_v<storage_type>
-																   && std::is_nothrow_move_assignable_v<storage_type>);
-
-		static constexpr bool is_trivially_move_constructible =
-			std::is_move_constructible_v<storage_type> ? std::is_trivially_move_constructible_v<storage_type>
-													   : (std::is_trivially_default_constructible_v<storage_type>
-														  && std::is_trivially_move_assignable_v<storage_type>);
+		static constexpr bool is_nothrow_move_constructible =
+			is_trivially_move_constructible
+				? true
+				: (std::is_move_constructible_v<storage_type> ? std::is_nothrow_move_constructible_v<storage_type>
+															  : std::is_nothrow_default_constructible_v<storage_type>
+																	&& std::is_nothrow_move_assignable_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_constructible)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
 		static storage_type& move_construct(std::byte* destination, std::byte* source) //
 			noexcept(is_nothrow_move_constructible)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_move_constructible_v<storage_type>)
+			if constexpr (is_trivially_move_constructible || std::is_move_constructible_v<storage_type>)
 			{
 				return construct(destination, static_cast<storage_type&&>(get(source)));
 			}
 			else
 			{
 				static_assert(std::is_default_constructible_v<storage_type>);
 				static_assert(std::is_move_assignable_v<storage_type>);
@@ -2505,54 +3078,54 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_move_constructible_v<storage_type>)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_construct_at(std::byte* dest_buffer,
-														 size_t dest_element_index,
-														 std::byte* source_buffer,
-														 size_t source_element_index) //
+		static constexpr storage_type& move_construct(std::byte* dest_buffer,
+													  size_t dest_element_index,
+													  std::byte* source_buffer,
+													  size_t source_element_index) //
 			noexcept(std::is_nothrow_move_constructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return move_construct(dest_buffer + dest_element_index * sizeof(storage_type),
 								  source_buffer + source_element_index * sizeof(storage_type));
 		}
 
 		//--- copy-construction ----------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_copy_constructible = is_trivially_constructible<const storage_type&>;
+
 		static constexpr bool is_copy_constructible =
-			std::is_copy_constructible_v<storage_type>
+			is_trivially_copy_constructible				  //
+			|| std::is_copy_constructible_v<storage_type> //
 			|| (std::is_default_constructible_v<storage_type> && std::is_copy_assignable_v<storage_type>);
 
-		static constexpr bool is_nothrow_copy_constructible = std::is_copy_constructible_v<storage_type>
-																? std::is_nothrow_copy_constructible_v<storage_type>
-																: (std::is_nothrow_default_constructible_v<storage_type>
-																   && std::is_nothrow_copy_assignable_v<storage_type>);
-
-		static constexpr bool is_trivially_copy_constructible =
-			std::is_copy_constructible_v<storage_type> ? std::is_trivially_copy_constructible_v<storage_type>
-													   : (std::is_trivially_default_constructible_v<storage_type>
-														  && std::is_trivially_copy_assignable_v<storage_type>);
+		static constexpr bool is_nothrow_copy_constructible =
+			is_trivially_copy_constructible
+				? true
+				: (std::is_copy_constructible_v<storage_type> ? std::is_nothrow_copy_constructible_v<storage_type>
+															  : std::is_nothrow_default_constructible_v<storage_type>
+																	&& std::is_nothrow_copy_assignable_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_constructible)
 		SOAGEN_ATTR(nonnull)
 		SOAGEN_CPP20_CONSTEXPR
 		static storage_type& copy_construct(std::byte* destination, const std::byte* source) //
 			noexcept(is_nothrow_copy_constructible)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_copy_constructible_v<storage_type>)
+			if constexpr (is_trivially_copy_constructible || std::is_copy_constructible_v<storage_type>)
 			{
 				return construct(destination, static_cast<const storage_type&>(get(source)));
 			}
 			else
 			{
 				static_assert(std::is_default_constructible_v<storage_type>);
 				static_assert(std::is_copy_assignable_v<storage_type>);
@@ -2576,18 +3149,18 @@
 					}
 				}
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_constructible)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_construct_at(std::byte* dest_buffer,
-														 size_t dest_element_index,
-														 const std::byte* source_buffer,
-														 size_t source_element_index) //
+		static constexpr storage_type& copy_construct(std::byte* dest_buffer,
+													  size_t dest_element_index,
+													  const std::byte* source_buffer,
+													  size_t source_element_index) //
 			noexcept(is_nothrow_copy_constructible)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return copy_construct(dest_buffer + dest_element_index * sizeof(storage_type),
 								  source_buffer + source_element_index * sizeof(storage_type));
@@ -2604,108 +3177,126 @@
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
 				get(target).~storage_type();
 			}
 		}
 
 		SOAGEN_ATTR(nonnull)
-		static constexpr void destruct_at([[maybe_unused]] std::byte* buffer,	 //
-										  [[maybe_unused]] size_t element_index) //
+		static constexpr void destruct([[maybe_unused]] std::byte* buffer,	  //
+									   [[maybe_unused]] size_t element_index) //
 			noexcept(std::is_nothrow_destructible_v<storage_type>)
 		{
 			SOAGEN_ASSUME(buffer != nullptr);
 
 			if constexpr (!std::is_trivially_destructible_v<storage_type>)
 			{
 				destruct(buffer + element_index * sizeof(storage_type));
 			}
 		}
 
 		//--- move-assignment ------------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_move_assignable =
+			is_constructible_with_memcpy<storage_type&&> || std::is_trivially_move_assignable_v<storage_type>;
+
 		static constexpr bool is_move_assignable =
-			std::is_move_assignable_v<storage_type>
+			is_trivially_move_assignable			   //
+			|| std::is_move_assignable_v<storage_type> //
 			|| (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_move_constructible_v<storage_type>);
 
 		static constexpr bool is_nothrow_move_assignable =
-			std::is_move_assignable_v<storage_type>
-				? std::is_nothrow_move_assignable_v<storage_type>
-				: (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_move_constructible_v<storage_type>);
-
-		static constexpr bool is_trivially_move_assignable =
-			std::is_move_assignable_v<storage_type> ? std::is_trivially_move_assignable_v<storage_type>
-													: (std::is_trivially_destructible_v<storage_type>
-													   && std::is_trivially_move_constructible_v<storage_type>);
+			is_trivially_move_assignable
+				? true
+				: (std::is_move_assignable_v<storage_type> ? std::is_nothrow_move_assignable_v<storage_type>
+														   : std::is_nothrow_destructible_v<storage_type>
+																 && std::is_nothrow_move_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& move_assign(std::byte* destination, void* source) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_move_assignable_v<storage_type>)
+			if constexpr (is_constructible_with_memcpy<storage_type&&>)
+			{
+				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
+							soagen::assume_aligned<alignof(storage_type)>(static_cast<std::byte*>(source)),
+							sizeof(storage_type));
+
+				return get(destination);
+			}
+			else if constexpr (is_trivially_move_assignable || std::is_move_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<storage_type&&>(get(static_cast<std::byte*>(source)));
 			}
 			else
 			{
-				// note we only fallback to this if they're nothrow because we don't want to leave the destination
+				// note we only fall back to this if they're nothrow because we don't want to leave the destination
 				// in a half-constructed state (it existed before the assignment, it should still exist after)
 				static_assert(std::is_nothrow_destructible_v<storage_type>);
 				static_assert(std::is_nothrow_move_constructible_v<storage_type>);
 
 				destruct(destination);
 				return move_construct(destination, static_cast<std::byte*>(source));
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_move_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& move_assign_at(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  std::byte* source_buffer,
-													  size_t source_element_index) //
+		static constexpr storage_type& move_assign(std::byte* dest_buffer,
+												   size_t dest_element_index,
+												   std::byte* source_buffer,
+												   size_t source_element_index) //
 			noexcept(is_nothrow_move_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return move_assign(dest_buffer + dest_element_index * sizeof(storage_type),
 							   source_buffer + source_element_index * sizeof(storage_type));
 		}
 
 		//--- copy-assignment ------------------------------------------------------------------------------------------
 
+		static constexpr bool is_trivially_copy_assignable =
+			is_constructible_with_memcpy<const storage_type&> || std::is_trivially_copy_assignable_v<storage_type>;
+
 		static constexpr bool is_copy_assignable =
-			std::is_copy_assignable_v<storage_type>
+			is_trivially_copy_assignable			   //
+			|| std::is_copy_assignable_v<storage_type> //
 			|| (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_copy_constructible_v<storage_type>);
 
 		static constexpr bool is_nothrow_copy_assignable =
-			std::is_copy_assignable_v<storage_type>
-				? std::is_nothrow_copy_assignable_v<storage_type>
-				: (std::is_nothrow_destructible_v<storage_type> && std::is_nothrow_copy_constructible_v<storage_type>);
-
-		static constexpr bool is_trivially_copy_assignable =
-			std::is_copy_assignable_v<storage_type> ? std::is_trivially_copy_assignable_v<storage_type>
-													: (std::is_trivially_destructible_v<storage_type>
-													   && std::is_trivially_copy_constructible_v<storage_type>);
+			is_trivially_copy_assignable
+				? true
+				: (std::is_copy_assignable_v<storage_type> ? std::is_nothrow_copy_assignable_v<storage_type>
+														   : std::is_nothrow_destructible_v<storage_type>
+																 && std::is_nothrow_copy_constructible_v<storage_type>);
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
 		static constexpr storage_type& copy_assign(std::byte* destination, const std::byte* source) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(destination != nullptr);
 			SOAGEN_ASSUME(source != nullptr);
 			SOAGEN_ASSUME(destination != source);
 
-			if constexpr (std::is_copy_assignable_v<storage_type>)
+			if constexpr (is_constructible_with_memcpy<storage_type&&>)
+			{
+				std::memcpy(soagen::assume_aligned<alignof(storage_type)>(destination),
+							soagen::assume_aligned<alignof(storage_type)>(static_cast<const std::byte*>(source)),
+							sizeof(storage_type));
+
+				return get(destination);
+			}
+			else if constexpr (is_trivially_copy_assignable || std::is_copy_assignable_v<storage_type>)
 			{
 				return get(destination) = static_cast<const storage_type&>(get(source));
 			}
 			else
 			{
 				// note we only fallback to this if they're nothrow because we don't want to leave the destination
 				// in a half-constructed state (it existed before the assignment, it should still exist after)
@@ -2715,18 +3306,18 @@
 				destruct(destination);
 				return copy_construct(destination, source);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_copy_assignable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr storage_type& copy_assign_at(std::byte* dest_buffer,
-													  size_t dest_element_index,
-													  const std::byte* source_buffer,
-													  size_t source_element_index) //
+		static constexpr storage_type& copy_assign(std::byte* dest_buffer,
+												   size_t dest_element_index,
+												   const std::byte* source_buffer,
+												   size_t source_element_index) //
 			noexcept(is_nothrow_copy_assignable)
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			return copy_assign(dest_buffer + dest_element_index * sizeof(storage_type),
 							   source_buffer + source_element_index * sizeof(storage_type));
@@ -2761,82 +3352,170 @@
 				move_assign(lhs, rhs);
 				move_assign(rhs, &temp);
 			}
 		}
 
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_swappable)
 		SOAGEN_ATTR(nonnull)
-		static constexpr void swap_at(std::byte* lhs_buffer,
-									  size_t lhs_element_index,
-									  std::byte* rhs_buffer,
-									  size_t rhs_element_index) //
+		static constexpr void swap(std::byte* lhs_buffer,
+								   size_t lhs_element_index,
+								   std::byte* rhs_buffer,
+								   size_t rhs_element_index) //
 			noexcept(is_nothrow_swappable)
 		{
 			SOAGEN_ASSUME(lhs_buffer != nullptr);
 			SOAGEN_ASSUME(rhs_buffer != nullptr);
 
 			return swap(lhs_buffer + lhs_element_index * sizeof(storage_type),
 						rhs_buffer + rhs_element_index * sizeof(storage_type));
 		}
 
-		//--- trivially-copy (memmove) ---------------------------------------------------------------------------------
+		//--- memmove ---------------------------------------------------------------------------------
 
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = std::is_trivially_copyable_v<storage_type>)
-		static constexpr void trivially_copy(std::byte* dest_buffer,
-											 size_t dest_element_index,
-											 const std::byte* source_buffer,
-											 size_t source_element_index,
-											 size_t count) noexcept
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_trivially_copyable)
+		static constexpr void memmove(std::byte* dest_buffer,
+									  size_t dest_element_index,
+									  const std::byte* source_buffer,
+									  size_t source_element_index,
+									  size_t count) noexcept
 		{
 			SOAGEN_ASSUME(dest_buffer != nullptr);
 			SOAGEN_ASSUME(source_buffer != nullptr);
 
 			std::memmove(dest_buffer + dest_element_index * sizeof(storage_type),
 						 source_buffer + source_element_index * sizeof(storage_type),
 						 count * sizeof(storage_type));
 		}
+
+		//--- equality -------------------------------------------------------------------------------------------------
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool equal(const std::byte* lhs, const std::byte* rhs) //
+			noexcept(is_nothrow_equality_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs != nullptr);
+			SOAGEN_ASSUME(rhs != nullptr);
+
+			return get(lhs) == get(rhs);
+		}
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_equality_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool equal(const std::byte* lhs_buffer,
+									size_t lhs_start_index,
+									const std::byte* rhs_buffer,
+									size_t rhs_start_index,
+									size_t count = 1) //
+			noexcept(is_nothrow_equality_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs_buffer != nullptr);
+			SOAGEN_ASSUME(rhs_buffer != nullptr);
+
+			lhs_buffer += lhs_start_index * sizeof(storage_type);
+			rhs_buffer += rhs_start_index * sizeof(storage_type);
+			const auto end = lhs_buffer + count * sizeof(storage_type);
+
+			for (; lhs_buffer < end; lhs_buffer += sizeof(storage_type), rhs_buffer += sizeof(storage_type))
+			{
+				if (!equal(lhs_buffer, rhs_buffer))
+					return false;
+			}
+
+			return true;
+		}
+
+		//--- less-than ------------------------------------------------------------------------------------------------
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_less_than_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool less_than(const std::byte* lhs, const std::byte* rhs) //
+			noexcept(is_nothrow_less_than_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs != nullptr);
+			SOAGEN_ASSUME(rhs != nullptr);
+
+			return get(lhs) < get(rhs);
+		}
+
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = is_less_than_comparable<storage_type>)
+		SOAGEN_NODISCARD
+		SOAGEN_ATTR(nonnull)
+		static constexpr bool less_than(const std::byte* lhs_buffer,
+										size_t lhs_element_index,
+										const std::byte* rhs_buffer,
+										size_t rhs_element_index) //
+			noexcept(is_nothrow_less_than_comparable<storage_type>)
+		{
+			SOAGEN_ASSUME(lhs_buffer != nullptr);
+			SOAGEN_ASSUME(rhs_buffer != nullptr);
+
+			return less_than(lhs_buffer + lhs_element_index * sizeof(storage_type),
+							 rhs_buffer + rhs_element_index * sizeof(storage_type));
+		}
 	};
 }
 
 namespace soagen
 {
 	template <typename ValueType,
-			  typename ParamType = param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType),
-			  typename Base		 = detail::column_traits_base<storage_type<ValueType>>>
-	struct column_traits : public Base
+			  typename ParamType = soagen::param_type<ValueType>,
+			  size_t Align		 = alignof(ValueType)
+				  SOAGEN_HIDDEN_PARAM(typename Base = detail::column_traits_base<storage_type<ValueType>>)>
+	struct SOAGEN_EMPTY_BASES column_traits //
+		SOAGEN_HIDDEN_BASE(public Base)
 	{
+#if SOAGEN_DOXYGEN
+
+		using storage_type = POXY_IMPLEMENTATION_DETAIL(dummy);
+
+#endif
+
 		using value_type = ValueType;
 		static_assert(!std::is_reference_v<value_type>, "column value_type may not be a reference");
 		static_assert(!std::is_void_v<value_type>, "column value_type may not be void");
 		static_assert(alignof(value_type) == alignof(typename Base::storage_type));
 		static_assert(sizeof(value_type) == sizeof(typename Base::storage_type));
 
 		using param_type = ParamType;
 		static_assert(!std::is_void_v<param_type>, "column param_type may not be void");
-		static_assert(std::is_convertible_v<param_type, value_type> || std::is_constructible_v<value_type, param_type>
-						  || (std::is_pointer_v<param_type> && std::is_same_v<typename Base::storage_type, void*>),
-					  "column value_type must be constructible or convertible from param_type");
+		static_assert(std::is_reference_v<param_type> || !is_cv<param_type>,
+					  "value parameters may not be cv-qualified");
+		static_assert(Base::template is_constructible<param_type>);
+
+		using param_forward_type = forward_type<param_type>;
+
+		using rvalue_type = soagen::rvalue_type<param_type>;
+		static_assert(Base::template is_constructible<rvalue_type>);
+
+		using rvalue_forward_type = forward_type<rvalue_type>;
+
+		using default_emplace_type = make_cref<rvalue_type>;
 
 		static constexpr size_t alignment = max(Align, alignof(value_type));
 		static_assert(has_single_bit(alignment), "column alignment must be a power of two");
 
-		static constexpr size_t max_capacity = static_cast<size_t>(-1) / sizeof(value_type);
-
 		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
 	};
 
-	template <typename>
-	inline constexpr bool is_column_traits = false;
-
+	template <typename T>
+	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
 	template <typename StorageType>
 	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
-
 	template <typename ValueType, typename ParamType, size_t Align, typename Base>
 	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align, Base>> = is_column_traits<Base>;
+	template <typename T>
+	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
+	template <typename T>
+	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
+	template <typename T>
+	inline constexpr bool is_column_traits<const volatile T> = is_column_traits<T>;
 }
 
 namespace soagen::detail
 {
 	template <typename T>
 	struct to_base_traits_;
 
@@ -2846,14 +3525,21 @@
 		using type = column_traits_base<storage_type<ValueType>>;
 
 		static_assert(std::is_base_of_v<type, column_traits<ValueType, ParamType, Align>>);
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
+
+	template <typename ValueType, //
+			  typename ParamType = param_type<ValueType>,
+			  size_t Align		 = alignof(ValueType)>
+	using make_column = soagen::column_traits<ValueType, //
+											  ParamType,
+											  soagen::max(Align, alignof(ValueType))>;
 }
 
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
@@ -2910,90 +3596,70 @@
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		// columns
 
 		template <size_t Index>
 		using column = type_at_index<Index, Columns...>;
 
-		template <typename IntegralConstant>
-		using column_from_ic = type_at_index<IntegralConstant::value, Columns...>;
-
-		template <size_t Index>
-		using column_storage_type = typename column<Index>::storage_type;
-
-		template <typename IntegralConstant>
-		using column_storage_type_from_ic = typename column_from_ic<IntegralConstant>::storage_type;
+		template <typename IndexConstant>
+		using column_from_ic = type_at_index<IndexConstant::value, Columns...>;
 
 		using column_pointers		= std::byte* [column_count];
 		using const_column_pointers = std::byte* const[column_count];
 
 		static constexpr size_t column_sizes[column_count] = { sizeof(typename Columns::storage_type)... };
 
-		// implicit lifetime types (C++23's std::start_lifetime_as)
-
-		static constexpr bool all_implicit_lifetime_types =
-			(is_implicit_lifetime_type<typename Columns::storage_type> && ...);
-
 		// default constructibility
 
 		static constexpr bool all_default_constructible =
 			(std::is_default_constructible_v<typename Columns::storage_type> && ...);
 
 		static constexpr bool all_nothrow_default_constructible =
 			(std::is_nothrow_default_constructible_v<typename Columns::storage_type> && ...);
 
 		static constexpr bool all_trivially_default_constructible =
 			(std::is_trivially_default_constructible_v<typename Columns::storage_type> && ...);
 
-		// trivial-copyability (memcpy)
+		// trivial-copyability (memcpy + memmove)
+
+		static constexpr bool all_trivially_copyable = (Columns::is_trivially_copyable && ...);
 
-		static constexpr bool all_trivially_copyable =
-			(std::is_trivially_copyable_v<typename Columns::storage_type> && ...);
+		static constexpr bool any_trivially_copyable = (false || ... || Columns::is_trivially_copyable);
 
 		// copy-constructibility
 
-		static constexpr bool all_copy_constructible =
-			all_trivially_copyable || (Columns::is_copy_constructible && ...);
+		static constexpr bool all_copy_constructible = (Columns::is_copy_constructible && ...);
 
-		static constexpr bool all_nothrow_copy_constructible =
-			all_trivially_copyable || (Columns::is_nothrow_copy_constructible && ...);
+		static constexpr bool all_nothrow_copy_constructible = (Columns::is_nothrow_copy_constructible && ...);
 
-		static constexpr bool all_trivially_copy_constructible =
-			all_trivially_copyable || (Columns::is_trivially_copy_constructible && ...);
+		static constexpr bool all_trivially_copy_constructible = (Columns::is_trivially_copy_constructible && ...);
 
 		// move-constructibility
 
-		static constexpr bool all_move_constructible =
-			all_trivially_copyable || (Columns::is_move_constructible && ...);
+		static constexpr bool all_move_constructible = (Columns::is_move_constructible && ...);
 
-		static constexpr bool all_nothrow_move_constructible =
-			all_trivially_copyable || (Columns::is_nothrow_move_constructible && ...);
+		static constexpr bool all_nothrow_move_constructible = (Columns::is_nothrow_move_constructible && ...);
 
-		static constexpr bool all_trivially_move_constructible =
-			all_trivially_copyable || (Columns::is_trivially_move_constructible && ...);
+		static constexpr bool all_trivially_move_constructible = (Columns::is_trivially_move_constructible && ...);
 
 		// copy-assignability
 
-		static constexpr bool all_copy_assignable = all_trivially_copyable || (Columns::is_copy_assignable && ...);
+		static constexpr bool all_copy_assignable = (Columns::is_copy_assignable && ...);
 
-		static constexpr bool all_nothrow_copy_assignable =
-			all_trivially_copyable || (Columns::is_nothrow_copy_assignable && ...);
+		static constexpr bool all_nothrow_copy_assignable = (Columns::is_nothrow_copy_assignable && ...);
 
-		static constexpr bool all_trivially_copy_assignable =
-			all_trivially_copyable || (Columns::is_trivially_copy_assignable && ...);
+		static constexpr bool all_trivially_copy_assignable = (Columns::is_trivially_copy_assignable && ...);
 
 		// move-assignability
 
-		static constexpr bool all_move_assignable = all_trivially_copyable || (Columns::is_move_assignable && ...);
+		static constexpr bool all_move_assignable = (Columns::is_move_assignable && ...);
 
-		static constexpr bool all_nothrow_move_assignable =
-			all_trivially_copyable || (Columns::is_nothrow_move_assignable && ...);
+		static constexpr bool all_nothrow_move_assignable = (Columns::is_nothrow_move_assignable && ...);
 
-		static constexpr bool all_trivially_move_assignable =
-			all_trivially_copyable || (Columns::is_trivially_move_assignable && ...);
+		static constexpr bool all_trivially_move_assignable = (Columns::is_trivially_move_assignable && ...);
 
 		// destructibility
 
 		static constexpr bool all_destructible = (std::is_destructible_v<typename Columns::storage_type> && ...);
 
 		static constexpr bool all_nothrow_destructible =
 			(std::is_nothrow_destructible_v<typename Columns::storage_type> && ...);
@@ -3003,60 +3669,142 @@
 
 		// swappability
 
 		static constexpr bool all_swappable = (Columns::is_swappable && ...);
 
 		static constexpr bool all_nothrow_swappable = (Columns::is_nothrow_swappable && ...);
 
+		// equality comparability
+
+		static constexpr bool all_equality_comparable = (is_equality_comparable<typename Columns::storage_type> && ...);
+
+		static constexpr bool all_nothrow_equality_comparable =
+			(is_nothrow_equality_comparable<typename Columns::storage_type> && ...);
+
+		// less-than comparability
+
+		static constexpr bool all_less_than_comparable =
+			(is_less_than_comparable<typename Columns::storage_type> && ...);
+
+		static constexpr bool all_nothrow_less_than_comparable =
+			(is_nothrow_less_than_comparable<typename Columns::storage_type> && ...);
+
 		// row constructibility
 
+	  private:
+		template <size_t, typename...>
+		struct row_constructible_from_row_ : std::false_type
+		{};
+		template <typename Table, size_t... RowCols, size_t... RowMembers>
+		struct row_constructible_from_row_<column_count, row<Table, RowCols...>, std::index_sequence<RowMembers...>>
+			: std::bool_constant<(Columns::template is_constructible<
+									  decltype(std::declval<row<Table, RowCols...>>().template get<RowMembers>())>
+								  && ...)>
+		{
+			static_assert(sizeof...(RowCols) == column_count);
+			static_assert(sizeof...(RowMembers) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<RowMembers...>, std::make_index_sequence<column_count>>);
+		};
+
+		template <bool, size_t, typename... Args>
+		struct row_constructible_from_ : std::false_type
+		{};
+		template <typename... Args>
+		struct row_constructible_from_<false, column_count, Args...>
+			: std::bool_constant<(Columns::template is_constructible<Args> && ...)>
+		{
+			static_assert(sizeof...(Args) == column_count);
+		};
+		template <typename Row>
+		struct row_constructible_from_<true, 1, Row>
+			: row_constructible_from_row_<std::tuple_size_v<remove_cvref<Row>>,
+										  remove_cvref<Row>,
+										  std::make_index_sequence<std::tuple_size_v<remove_cvref<Row>>>>
+		{};
+
+	  public:
 		template <typename... Args>
 		static constexpr bool row_constructible_from =
-			sizeof...(Args) == column_count && (Columns::template is_constructible<Args> && ...);
+			row_constructible_from_<(is_row<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
+		// row constructibility (nothrow)
+
+	  private:
+		template <size_t, typename...>
+		struct row_nothrow_constructible_from_row_ : std::false_type
+		{};
+		template <typename Table, size_t... RowCols, size_t... RowMembers>
+		struct row_nothrow_constructible_from_row_<column_count,
+												   row<Table, RowCols...>,
+												   std::index_sequence<RowMembers...>>
+			: std::bool_constant<(Columns::template is_nothrow_constructible<
+									  decltype(std::declval<row<Table, RowCols...>>().template get<RowMembers>())>
+								  && ...)>
+		{
+			static_assert(sizeof...(RowCols) == column_count);
+			static_assert(sizeof...(RowMembers) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<RowMembers...>, std::make_index_sequence<column_count>>);
+		};
+
+		template <bool, size_t, typename... Args>
+		struct row_nothrow_constructible_from_ : std::false_type
+		{};
+		template <typename... Args>
+		struct row_nothrow_constructible_from_<false, column_count, Args...>
+			: std::bool_constant<(Columns::template is_nothrow_constructible<Args> && ...)>
+		{
+			static_assert(sizeof...(Args) == column_count);
+		};
+		template <typename Row>
+		struct row_nothrow_constructible_from_<true, 1, Row>
+			: row_nothrow_constructible_from_row_<std::tuple_size_v<remove_cvref<Row>>,
+												  remove_cvref<Row>,
+												  std::make_index_sequence<std::tuple_size_v<remove_cvref<Row>>>>
+		{};
+
+	  public:
 		template <typename... Args>
 		static constexpr bool row_nothrow_constructible_from =
-			sizeof...(Args) == column_count && (Columns::template is_nothrow_constructible<Args> && ...);
+			row_nothrow_constructible_from_<(is_row<remove_cvref<Args>> && ...), sizeof...(Args), Args...>::value;
 
-		//--- trivially-copy (memmove) ---------------------------------------------------------------------------------
+		//--- memmove --------------------------------------------------------------------------------------------------
 
 	  private:
 		template <size_t... Cols>
 		SOAGEN_CPP20_CONSTEXPR
-		static void trivially_copy_rows(column_pointers& dest_columns,
-										size_t dest_start,
-										column_pointers& source_columns,
-										size_t source_start,
-										size_t count,
-										std::index_sequence<Cols...>) //
+		static void memmove(column_pointers& dest_columns,
+							size_t dest_start,
+							column_pointers& source_columns,
+							size_t source_start,
+							size_t count,
+							std::index_sequence<Cols...>) //
 			noexcept
 		{
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
 
-			(column<Cols>::trivially_copy(dest_columns[Cols], dest_start, source_columns[Cols], source_start, count),
-			 ...);
+			(column<Cols>::memmove(dest_columns[Cols], dest_start, source_columns[Cols], source_start, count), ...);
 		}
 
 	  public:
-		SOAGEN_HIDDEN_CONSTRAINT(sfinae, bool sfinae = all_trivially_copyable)
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_trivially_copyable)
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
-		static void trivially_copy_rows(column_pointers& dest_columns,
-										size_t dest_start,
-										column_pointers& source_columns,
-										size_t source_start,
-										size_t count) //
+		static void memmove(column_pointers& dest_columns,
+							size_t dest_start,
+							column_pointers& source_columns,
+							size_t source_start,
+							size_t count) //
 			noexcept
 		{
-			trivially_copy_rows(dest_columns,
-								dest_start,
-								source_columns,
-								source_start,
-								count,
-								std::make_index_sequence<column_count>{});
+			memmove(dest_columns,
+					dest_start,
+					source_columns,
+					source_start,
+					count,
+					std::make_index_sequence<column_count>{});
 		}
 
 		//--- destruction ----------------------------------------------------------------------------------------------
 
 	  private:
 		template <size_t... Cols>
 		SOAGEN_CPP20_CONSTEXPR
@@ -3074,27 +3822,27 @@
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
 					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
 
-					if constexpr (!std::is_trivially_destructible_v<column_storage_type<column_index>>)
+					if constexpr (!std::is_trivially_destructible_v<typename column<column_index>::storage_type>)
 					{
 						SOAGEN_ASSUME(columns[column_index]);
 						SOAGEN_ASSUME(leftmost_column <= rightmost_column);
 						SOAGEN_ASSUME(leftmost_column < column_count);
 						SOAGEN_ASSUME(rightmost_column < column_count);
 
 						if (column_index >= leftmost_column && column_index <= rightmost_column)
-							column<column_index>::destruct_at(columns[column_index], index);
+							column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
-				(destructor(index_tag<Cols>{}), ...);
+				(destructor(index_constant<Cols>{}), ...);
 			}
 		}
 
 		template <size_t... Cols>
 		SOAGEN_CPP20_CONSTEXPR
 		static void destruct_row([[maybe_unused]] column_pointers& columns,
 								 [[maybe_unused]] size_t index,
@@ -3108,23 +3856,23 @@
 			}
 			else
 			{
 				const auto destructor = [&](auto ic) noexcept
 				{
 					static constexpr size_t column_index = column_count - decltype(ic)::value - 1u;
 
-					if constexpr (!std::is_trivially_destructible_v<column_storage_type<column_index>>)
+					if constexpr (!std::is_trivially_destructible_v<typename column<column_index>::storage_type>)
 					{
 						SOAGEN_ASSUME(columns[column_index]);
 
-						column<column_index>::destruct_at(columns[column_index], index);
+						column<column_index>::destruct(columns[column_index], index);
 					}
 				};
 
-				(destructor(index_tag<Cols>{}), ...);
+				(destructor(index_constant<Cols>{}), ...);
 			}
 		}
 
 	  public:
 		SOAGEN_ALWAYS_INLINE
 		static constexpr void destruct_row(column_pointers& columns,
 										   size_t index,
@@ -3165,37 +3913,38 @@
 		static void default_construct_row(column_pointers& columns,
 										  size_t index,
 										  std::index_sequence<Cols...>) //
 			noexcept(all_nothrow_default_constructible)					//
 			SOAGEN_REQUIRES(all_default_constructible)
 		{
 			static_assert(all_default_constructible);
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
 
 			if constexpr (all_nothrow_default_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::default_construct_at(columns[Cols], index), ...);
+				(column<Cols>::default_construct(columns[Cols], index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor = [&](auto ic) //
-					noexcept(std::is_nothrow_default_constructible_v<column_storage_type<decltype(ic)::value>>)
+					noexcept(
+						std::is_nothrow_default_constructible_v<typename column<decltype(ic)::value>::storage_type>)
 				{
-					column_from_ic<decltype(ic)>::default_construct_at(columns[decltype(ic)::value], index);
+					column_from_ic<decltype(ic)>::default_construct(columns[decltype(ic)::value], index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_tag<Cols>{}), ...);
+					(constructor(index_constant<Cols>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
 						destruct_row(columns, index, 0u, constructed_columns - 1u);
 
 					throw;
@@ -3245,57 +3994,86 @@
 				}
 			}
 		}
 
 		//--- construction ---------------------------------------------------------------------------------------------
 
 	  private:
+		template <typename Row, size_t... Cols>
+		SOAGEN_CPP20_CONSTEXPR
+		static void construct_row_from_row(column_pointers& columns,
+										   size_t index,
+										   Row&& row,
+										   std::index_sequence<Cols...>) //
+			noexcept(row_nothrow_constructible_from<Row&&>)
+		{
+			static_assert(is_row<remove_cvref<Row>>);
+			static_assert(row_constructible_from<Row&&>);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+			static_assert(std::tuple_size_v<remove_cvref<Row>> == column_count);
+
+			construct_row(columns,
+						  index,
+						  std::index_sequence<Cols...>{},
+						  static_cast<Row&&>(row).template get<Cols>()...);
+		}
+
 		template <typename... Args, size_t... Cols>
 		SOAGEN_CPP20_CONSTEXPR
 		static void construct_row(column_pointers& columns,
 								  size_t index,
 								  std::index_sequence<Cols...>,
 								  Args&&... args) //
 			noexcept(row_nothrow_constructible_from<Args&&...>)
 		{
 			static_assert(row_constructible_from<Args&&...>);
-			static_assert(sizeof...(Cols) == sizeof...(Args));
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
 
-			if constexpr (row_nothrow_constructible_from<Args&&...> || all_trivially_destructible)
+			if constexpr (sizeof...(Args) == 1 && (is_row<remove_cvref<Args>> && ...))
 			{
-				(column<Cols>::construct_at(columns[Cols], index, static_cast<Args&&>(args)), ...);
+				construct_row_from_row(columns, index, static_cast<Args&&>(args)..., std::index_sequence<Cols...>{});
 			}
 			else
 			{
-				// machinery to provide strong-exception guarantee
-
-				size_t constructed_columns = {};
+				static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+				static_assert(sizeof...(Args) == sizeof...(Cols));
 
-				const auto constructor =
-					[&](auto ic, auto&& arg) noexcept(
-						std::is_nothrow_constructible_v<column_storage_type_from_ic<decltype(ic)>, decltype(arg)&&>)
+				if constexpr (row_nothrow_constructible_from<Args&&...> || all_trivially_destructible)
 				{
-					column_from_ic<decltype(ic)>::construct_at(columns[decltype(ic)::value],
-															   index,
-															   static_cast<decltype(arg)&&>(arg));
-
-					constructed_columns++;
-				};
-
-				try
-				{
-					(constructor(index_tag<Cols>{}, static_cast<Args&&>(args)), ...);
+					(column<Cols>::construct_at(columns[Cols], index, static_cast<Args&&>(args)), ...);
 				}
-				catch (...)
+				else
 				{
-					if (constructed_columns)
-						destruct_row(columns, index, 0u, constructed_columns - 1u);
+					// machinery to provide strong-exception guarantee
 
-					throw;
+					size_t constructed_columns = {};
+
+					const auto constructor =
+						[&](auto ic, auto&& arg) noexcept(
+							std::is_nothrow_constructible_v<typename column_from_ic<decltype(ic)>::storage_type,
+															decltype(arg)&&>)
+					{
+						column_from_ic<decltype(ic)>::construct_at(columns[decltype(ic)::value],
+																   index,
+																   static_cast<decltype(arg)&&>(arg));
+
+						constructed_columns++;
+					};
+
+					try
+					{
+						(constructor(index_constant<Cols>{}, static_cast<Args&&>(args)), ...);
+					}
+					catch (...)
+					{
+						if (constructed_columns)
+							destruct_row(columns, index, 0u, constructed_columns - 1u);
+
+						throw;
+					}
 				}
 			}
 		}
 
 	  public:
 		template <typename... Args>
 		SOAGEN_ALWAYS_INLINE
@@ -3324,42 +4102,43 @@
 		static void move_construct_row(column_pointers& dest_columns,
 									   size_t dest_index,
 									   column_pointers& source_columns,
 									   size_t source_index,
 									   std::index_sequence<Cols...>) //
 			noexcept(all_nothrow_move_constructible)
 		{
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
 
 			if constexpr (all_nothrow_move_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::move_construct_at(dest_columns[Cols], dest_index, source_columns[Cols], source_index),
-				 ...);
+				(column<Cols>::move_construct(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
 					[&](auto ic) noexcept(
-						std::is_nothrow_move_constructible_v<column_storage_type_from_ic<decltype(ic)>>)
+						std::is_nothrow_move_constructible_v<typename column_from_ic<decltype(ic)>::storage_type>)
 				{
-					column_from_ic<decltype(ic)>::move_construct_at(dest_columns[decltype(ic)::value],
-																	dest_index,
-																	source_columns[decltype(ic)::value],
-																	source_index);
+					column_from_ic<decltype(ic)>::move_construct(dest_columns[decltype(ic)::value],
+																 dest_index,
+																 source_columns[decltype(ic)::value],
+																 source_index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_tag<Cols>{}), ...);
+					(constructor(index_constant<Cols>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
 						destruct_row(dest_columns, dest_index, 0u, constructed_columns - 1u);
 
 					throw;
@@ -3389,38 +4168,64 @@
 		static void move_construct_rows(column_pointers& dest_columns,
 										size_t dest_start,
 										column_pointers& source_columns,
 										size_t source_start,
 										size_t count) //
 			noexcept(all_nothrow_move_constructible)
 		{
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+
 			if constexpr (all_trivially_copyable)
 			{
-				trivially_copy_rows(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest_columns, dest_start, source_columns, source_start, count);
 			}
 			else if constexpr (all_nothrow_move_constructible)
 			{
-				for (size_t i = 0; i < count; i++)
-					move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+				if (&dest_columns == &source_columns && dest_start > source_start)
+				{
+					for (size_t i = count; i-- > 0u;)
+						move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+				}
+				else
+				{
+					for (size_t i = 0; i < count; i++)
+						move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+				}
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = 0;
 
 				try
 				{
-					for (; i < count; i++)
-						move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+					if (&dest_columns == &source_columns && dest_start > source_start)
+					{
+						for (; i-- > 0u;)
+							move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+					}
+					else
+					{
+						for (; i < count; i++)
+							move_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+					}
 				}
 				catch (...)
 				{
-					for (; i-- > 0u;)
-						destruct_row(dest_columns, dest_start + i);
+					if (&dest_columns == &source_columns && dest_start > source_start)
+					{
+						for (; i < count; i++)
+							destruct_row(dest_columns, dest_start + i);
+					}
+					else
+					{
+						for (; i-- > 0u;)
+							destruct_row(dest_columns, dest_start + i);
+					}
 					throw;
 				}
 			}
 		}
 
 		//--- copy-construction ----------------------------------------------------------------------------------------
 
@@ -3430,42 +4235,43 @@
 		static void copy_construct_row(column_pointers& dest_columns,
 									   size_t dest_index,
 									   const const_column_pointers& source_columns,
 									   size_t source_index,
 									   std::index_sequence<Cols...>) //
 			noexcept(all_nothrow_copy_constructible)
 		{
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
 
 			if constexpr (all_nothrow_copy_constructible || all_trivially_destructible)
 			{
-				(column<Cols>::copy_construct_at(dest_columns[Cols], dest_index, source_columns[Cols], source_index),
-				 ...);
+				(column<Cols>::copy_construct(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t constructed_columns = {};
 
 				const auto constructor =
 					[&](auto ic) noexcept(
-						std::is_nothrow_copy_constructible_v<column_storage_type_from_ic<decltype(ic)>>)
+						std::is_nothrow_copy_constructible_v<typename column_from_ic<decltype(ic)>::storage_type>)
 				{
-					column_from_ic<decltype(ic)>::copy_construct_at(dest_columns[decltype(ic)::value],
-																	dest_index,
-																	source_columns[decltype(ic)::value],
-																	source_index);
+					column_from_ic<decltype(ic)>::copy_construct(dest_columns[decltype(ic)::value],
+																 dest_index,
+																 source_columns[decltype(ic)::value],
+																 source_index);
 
 					constructed_columns++;
 				};
 
 				try
 				{
-					(constructor(index_tag<Cols>{}), ...);
+					(constructor(index_constant<Cols>{}), ...);
 				}
 				catch (...)
 				{
 					if (constructed_columns)
 						destruct_row(dest_columns, dest_index, 0u, constructed_columns - 1u);
 
 					throw;
@@ -3495,38 +4301,64 @@
 		static void copy_construct_rows(column_pointers& dest_columns,
 										size_t dest_start,
 										const const_column_pointers& source_columns,
 										size_t source_start,
 										size_t count) //
 			noexcept(all_nothrow_copy_constructible)
 		{
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+
 			if constexpr (all_trivially_copyable)
 			{
-				trivially_copy_rows(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest_columns, dest_start, source_columns, source_start, count);
 			}
 			else if constexpr (all_nothrow_copy_constructible)
 			{
-				for (size_t i = 0; i < count; i++)
-					copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+				if (&dest_columns == &source_columns && dest_start > source_start)
+				{
+					for (size_t i = count; i-- > 0u;)
+						copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+				}
+				else
+				{
+					for (size_t i = 0; i < count; i++)
+						copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+				}
 			}
 			else
 			{
 				// machinery to provide strong-exception guarantee
 
 				size_t i = 0;
 
 				try
 				{
-					for (; i < count; i++)
-						copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+					if (&dest_columns == &source_columns && dest_start > source_start)
+					{
+						for (; i-- > 0u;)
+							copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+					}
+					else
+					{
+						for (; i < count; i++)
+							copy_construct_row(dest_columns, dest_start + i, source_columns, source_start + i);
+					}
 				}
 				catch (...)
 				{
-					for (; i-- > 0u;)
-						destruct_row(dest_columns, dest_start + i);
+					if (&dest_columns == &source_columns && dest_start > source_start)
+					{
+						for (; i < count; i++)
+							destruct_row(dest_columns, dest_start + i);
+					}
+					else
+					{
+						for (; i-- > 0u;)
+							destruct_row(dest_columns, dest_start + i);
+					}
 					throw;
 				}
 			}
 		}
 
 		//--- move-assignment ------------------------------------------------------------------------------------------
 
@@ -3536,19 +4368,21 @@
 		static void move_assign_row(column_pointers& dest_columns,
 									size_t dest_index,
 									column_pointers& source_columns,
 									size_t source_index,
 									std::index_sequence<Cols...>) //
 			noexcept(all_nothrow_move_assignable)
 		{
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
 
 			// todo: how to provide a strong-exception guarantee here?
 
-			(column<Cols>::move_assign_at(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+			(column<Cols>::move_assign(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
 		}
 
 	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_move_assignable)
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
 		static void move_assign_row(column_pointers& dest_columns,
@@ -3569,17 +4403,19 @@
 		static void move_assign_rows(column_pointers& dest_columns,
 									 size_t dest_start,
 									 column_pointers& source_columns,
 									 size_t source_start,
 									 size_t count) //
 			noexcept(all_nothrow_copy_assignable)
 		{
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+
 			if constexpr (all_trivially_copyable)
 			{
-				trivially_copy_rows(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest_columns, dest_start, source_columns, source_start, count);
 			}
 			else
 			{
 				if (&dest_columns == &source_columns && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
 						move_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
@@ -3600,19 +4436,21 @@
 		static void copy_assign_row(column_pointers& dest_columns,
 									size_t dest_index,
 									const const_column_pointers& source_columns,
 									size_t source_index,
 									std::index_sequence<Cols...>) //
 			noexcept(all_nothrow_copy_assignable)
 		{
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_index != source_index);
 
 			// todo: how to provide a strong-exception guarantee here?
 
-			(column<Cols>::copy_assign_at(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
+			(column<Cols>::copy_assign(dest_columns[Cols], dest_index, source_columns[Cols], source_index), ...);
 		}
 
 	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_copy_assignable)
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
 		static void copy_assign_row(column_pointers& dest_columns,
@@ -3633,17 +4471,19 @@
 		static void copy_assign_rows(column_pointers& dest_columns,
 									 size_t dest_start,
 									 const const_column_pointers& source_columns,
 									 size_t source_start,
 									 size_t count) //
 			noexcept(all_nothrow_copy_assignable)
 		{
+			SOAGEN_ASSUME(&dest_columns != &source_columns || dest_start != source_start);
+
 			if constexpr (all_trivially_copyable)
 			{
-				trivially_copy_rows(dest_columns, dest_start, source_columns, source_start, count);
+				memmove(dest_columns, dest_start, source_columns, source_start, count);
 			}
 			else
 			{
 				if (&dest_columns == &source_columns && dest_start > source_start)
 				{
 					for (size_t i = count; i-- > 0u;)
 						copy_assign_row(dest_columns, dest_start + i, source_columns, source_start + i);
@@ -3664,90 +4504,236 @@
 		static void swap_rows(column_pointers& lhs_columns,
 							  size_t lhs_index,
 							  column_pointers& rhs_columns,
 							  size_t rhs_index,
 							  std::index_sequence<Cols...>) //
 			noexcept(all_nothrow_swappable)
 		{
-			static_assert(sizeof...(Cols) == column_count);
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
 
-			(column<Cols>::swap_at(lhs_columns[Cols], lhs_index, rhs_columns[Cols], rhs_index), ...);
+			(column<Cols>::swap(lhs_columns[Cols], lhs_index, rhs_columns[Cols], rhs_index), ...);
 		}
 
 	  public:
 		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_swappable)
 		SOAGEN_ALWAYS_INLINE
 		SOAGEN_CPP20_CONSTEXPR
 		static void swap_rows(column_pointers& lhs_columns,
 							  size_t lhs_index,
 							  column_pointers& rhs_columns,
 							  size_t rhs_index) //
 			noexcept(all_nothrow_swappable)
 		{
 			swap_rows(lhs_columns, lhs_index, rhs_columns, rhs_index, std::make_index_sequence<column_count>{});
 		}
+
+		//--- equality -------------------------------------------------------------------------------------------------
+
+	  private:
+		template <typename... Args, size_t... Cols>
+		SOAGEN_NODISCARD
+		constexpr static bool equal(const const_column_pointers& lhs_columns,
+									size_t lhs_start_index,
+									const const_column_pointers& rhs_columns,
+									size_t rhs_start_index,
+									size_t count,
+									std::index_sequence<Cols...>) //
+			noexcept(all_nothrow_equality_comparable)
+		{
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+
+			// note that the equality-comparison is done column-major for speed (cache-locality) because
+			// equality-comparison does not need to know anything about the order of the columns,
+			// just that they are all equal (there is no lexicographic constraint)
+
+			return (column<Cols>::equal(lhs_columns[Cols], lhs_start_index, rhs_columns[Cols], rhs_start_index, count)
+					&& ...);
+		}
+
+	  public:
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_equality_comparable)
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		constexpr static bool equal(const const_column_pointers& lhs_columns,
+									size_t lhs_start,
+									const const_column_pointers& rhs_columns,
+									size_t rhs_start,
+									size_t count) //
+			noexcept(all_nothrow_equality_comparable)
+		{
+			return equal(lhs_columns,
+						 lhs_start,
+						 rhs_columns,
+						 rhs_start,
+						 count,
+						 std::make_index_sequence<column_count>{});
+		}
+
+		//--- compare --------------------------------------------------------------------------------------------------
+
+	  private:
+		template <typename... Args, size_t... Cols>
+		SOAGEN_NODISCARD
+		constexpr static int compare(const const_column_pointers& lhs_columns,
+									 size_t lhs_start_index,
+									 const const_column_pointers& rhs_columns,
+									 size_t rhs_start_index,
+									 size_t count,
+									 std::index_sequence<Cols...>) //
+			noexcept(all_nothrow_less_than_comparable)
+		{
+			static_assert(std::is_same_v<std::index_sequence<Cols...>, std::make_index_sequence<column_count>>);
+
+			for (size_t i = 0; i < count; i++)
+			{
+				if ((false || ...
+					 || column<Cols>::less_than(lhs_columns[Cols],
+												lhs_start_index + i,
+												rhs_columns[Cols],
+												rhs_start_index + i)))
+					return -1;
+
+				if ((false || ...
+					 || column<Cols>::less_than(rhs_columns[Cols],
+												rhs_start_index + i,
+												lhs_columns[Cols],
+												lhs_start_index + i)))
+					return 1;
+			}
+
+			return 0;
+		}
+
+	  public:
+		SOAGEN_HIDDEN_CONSTRAINT(sfinae, auto sfinae = all_less_than_comparable)
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		constexpr static int compare(const const_column_pointers& lhs_columns,
+									 size_t lhs_start,
+									 const const_column_pointers& rhs_columns,
+									 size_t rhs_start,
+									 size_t count) //
+			noexcept(all_nothrow_less_than_comparable)
+		{
+			return compare(lhs_columns,
+						   lhs_start,
+						   rhs_columns,
+						   rhs_start,
+						   count,
+						   std::make_index_sequence<column_count>{});
+		}
 	};
 }
 
 namespace soagen
 {
 	template <typename... Columns>
-	struct table_traits : public detail::table_traits_base<detail::to_base_traits<Columns>...>
+	struct SOAGEN_EMPTY_BASES table_traits : public detail::table_traits_base<detail::to_base_traits<Columns>...>
 	{
 		static constexpr size_t column_count = sizeof...(Columns);
 		static_assert(column_count, "tables must have at least one column");
 		static_assert((... && is_column_traits<Columns>), "columns must be instances of soagen::column_traits");
 
 		static constexpr size_t aligned_stride = lcm(size_t{ 1 }, Columns::aligned_stride...);
 
 		// columns
 		// (note that these hide the base class typedefs - this is intentional)
 
 		template <size_t Index>
 		using column = type_at_index<Index, Columns...>;
 
-		template <size_t Index>
-		using column_type = typename column<Index>::value_type;
-
-		template <size_t Index>
-		using column_storage_type = typename column<Index>::storage_type;
-
-		template <typename IntegralConstant>
-		using column_from_ic = type_at_index<IntegralConstant::value, Columns...>;
-
-		template <typename IntegralConstant>
-		using column_type_from_ic = typename column_from_ic<IntegralConstant>::value_type;
-
-		template <typename IntegralConstant>
-		using column_storage_type_from_ic = typename column_from_ic<IntegralConstant>::storage_type;
+		template <typename IndexConstant>
+		using column_from_ic = type_at_index<IndexConstant::value, Columns...>;
 
 		static constexpr size_t column_alignments[column_count] = { Columns::alignment... };
 
 		static constexpr size_t largest_alignment = max(size_t{ 1 }, Columns::alignment...);
-	};
 
-	template <typename>
-	inline constexpr bool is_table_traits = false;
+		static constexpr bool rvalue_type_list_is_distinct = POXY_IMPLEMENTATION_DETAIL(
+			!(std::is_same_v<typename Columns::param_type, typename Columns::rvalue_type> && ...));
 
+		template <typename BackingTable, typename... Args>
+		static constexpr bool emplace_back_is_nothrow =
+			noexcept(std::declval<BackingTable>().emplace_back(std::declval<Args>()...));
+
+		template <typename BackingTable>
+		static constexpr bool push_back_is_nothrow =
+			emplace_back_is_nothrow<BackingTable, typename Columns::param_forward_type...>;
+
+		template <typename BackingTable>
+		static constexpr bool rvalue_push_back_is_nothrow =
+			emplace_back_is_nothrow<BackingTable, typename Columns::rvalue_forward_type...>;
+
+		template <typename BackingTable, typename Row>
+		static constexpr bool row_push_back_is_nothrow = emplace_back_is_nothrow<BackingTable, Row>;
+
+		template <typename BackingTable, typename... Args>
+		static constexpr bool emplace_is_nothrow =
+			noexcept(std::declval<BackingTable>().emplace(typename remove_cvref<BackingTable>::size_type{},
+														  std::declval<Args>()...));
+
+		template <typename BackingTable>
+		static constexpr bool insert_is_nothrow =
+			emplace_is_nothrow<BackingTable, typename Columns::param_forward_type...>;
+
+		template <typename BackingTable>
+		static constexpr bool rvalue_insert_is_nothrow =
+			emplace_is_nothrow<BackingTable, typename Columns::rvalue_forward_type...>;
+
+		template <typename BackingTable, typename Row>
+		static constexpr bool row_insert_is_nothrow = emplace_is_nothrow<BackingTable, Row>;
+
+		template <typename Func, bool Const = false>
+		static constexpr bool for_each_column_ptr_invocable = POXY_IMPLEMENTATION_DETAIL( //
+			(is_invocable_with_optarg<Func,
+									  std::conditional_t<Const,
+														 std::add_const_t<typename Columns::value_type>,
+														 typename Columns::value_type>*,
+									  size_t>
+			 && ...));
+
+		template <typename Func, bool Const = false>
+		static constexpr bool for_each_column_ptr_nothrow_invocable = POXY_IMPLEMENTATION_DETAIL( //
+			(is_nothrow_invocable_with_optarg<Func,
+											  std::conditional_t<Const,
+																 std::add_const_t<typename Columns::value_type>,
+																 typename Columns::value_type>*,
+											  size_t>
+			 && ...));
+	};
+
+	template <typename T>
+	inline constexpr bool is_table_traits = POXY_IMPLEMENTATION_DETAIL(false);
 	template <typename... Columns>
 	inline constexpr bool is_table_traits<table_traits<Columns...>> = true;
-
 	template <typename... Columns>
 	inline constexpr bool is_table_traits<detail::table_traits_base<Columns...>> = true;
+	template <typename T>
+	inline constexpr bool is_table_traits<const T> = is_table_traits<T>;
+	template <typename T>
+	inline constexpr bool is_table_traits<volatile T> = is_table_traits<T>;
+	template <typename T>
+	inline constexpr bool is_table_traits<const volatile T> = is_table_traits<T>;
 }
 
 namespace soagen::detail
 {
 	template <typename... Columns>
 	struct to_base_traits_<table_traits<Columns...>>
 	{
 		using type = table_traits_base<to_base_traits<Columns>...>;
 
 		static_assert(std::is_base_of_v<type, table_traits<Columns...>>);
 	};
+
+	template <typename... Columns>
+	struct table_traits_type_<table_traits<Columns...>>
+	{
+		using type = table_traits<Columns...>;
+	};
 }
 
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
@@ -3791,24 +4777,40 @@
 #if SOAGEN_CLANG >= 16
 	#pragma clang diagnostic ignored "-Wunsafe-buffer-usage"
 #endif
 
 namespace soagen::detail
 {
 	SOAGEN_CONSTRAINED_TEMPLATE(is_unsigned<T>, typename T)
-	SOAGEN_PURE_GETTER
+	[[nodiscard]]
 	constexpr bool add_without_overflowing(T lhs, T rhs, T& result) noexcept
 	{
 		if (lhs > static_cast<T>(-1) - rhs)
 			return false;
 
 		result = lhs + rhs;
 		return true;
 	};
 
+	// trait for determining the _actual_ alignment of a table column, taking the allocator and
+	// table-allocation semantics into account (since the full allocation for a table always has
+	// alignment == table_traits::largest_alignment).
+	//
+	// note that this has absolutely nothing to do with the aligned_stride; that is still calculated
+	// according to the user's specified alignment requirements. this trait is _only_ used
+	// to help the compiler via assume_aligned.
+	template <typename Traits, typename Allocator, size_t ColumnIndex>
+	inline constexpr size_t actual_column_alignment = Traits::template column<ColumnIndex>::alignment;
+
+	template <typename Traits, typename Allocator>
+	inline constexpr size_t actual_column_alignment<Traits, Allocator, 0> =
+		max(Traits::template column<0>::alignment,
+			allocator_traits<Allocator>::min_alignment,
+			Traits::largest_alignment);
+
 	//------------------------------------------------------------------------------------------------------------------
 	// generic allocation class for tracking the column pointers and the actual size in bytes
 	//------------------------------------------------------------------------------------------------------------------
 
 	template <size_t ColumnCount>
 	struct table_allocation
 	{
@@ -3832,18 +4834,17 @@
 	template <size_t ColumnCount, typename Allocator>
 	class table_base
 	{
 		static_assert(ColumnCount, "tables must have at least one column");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
 	  public:
-		using size_type		   = size_t;
-		using difference_type  = ptrdiff_t;
-		using allocator_type   = Allocator;
-		using allocator_traits = soagen::allocator_traits<allocator_type>;
+		using size_type		  = size_t;
+		using difference_type = ptrdiff_t;
+		using allocator_type  = Allocator;
 
 	  protected:
 		using allocation = table_allocation<ColumnCount>;
 
 		allocation alloc_ = {};
 		size_t count_	  = {};
 		compressed_pair<size_t, Allocator> capacity_;
@@ -3888,26 +4889,14 @@
 			// element destructors are run in a more specialized child class
 
 			if (alloc_)
 				deallocate(alloc_);
 		}
 
 		SOAGEN_PURE_INLINE_GETTER
-		constexpr std::byte* data() noexcept
-		{
-			return alloc_.columns[0];
-		}
-
-		SOAGEN_PURE_INLINE_GETTER
-		constexpr const std::byte* data() const noexcept
-		{
-			return alloc_.columns[0];
-		}
-
-		SOAGEN_PURE_INLINE_GETTER
 		constexpr size_t size() const noexcept
 		{
 			return count_;
 		}
 
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr bool empty() const noexcept
@@ -3917,16 +4906,23 @@
 
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr size_t capacity() const noexcept
 		{
 			return capacity_.first();
 		}
 
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr size_t allocation_size() const noexcept
+		{
+			return alloc_.size_in_bytes;
+		}
+
 		SOAGEN_INLINE_GETTER
-		constexpr Allocator get_allocator() const noexcept
+		SOAGEN_CPP20_CONSTEXPR
+		Allocator get_allocator() const noexcept
 		{
 			return capacity_.second();
 		}
 
 	  protected:
 		SOAGEN_INLINE_GETTER
 		constexpr Allocator& allocator() noexcept
@@ -3937,30 +4933,31 @@
 		SOAGEN_INLINE_GETTER
 		constexpr const Allocator& allocator() const noexcept
 		{
 			return capacity_.second();
 		}
 
 		static constexpr bool allocate_is_nothrow =
-			noexcept(allocator_traits::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}));
+			noexcept(allocator_traits<Allocator>::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}));
 
 		// guard against allocators with incorrect pointer typedefs where possible
 		using allocator_pointer_type = std::remove_reference_t<
-			decltype(allocator_traits::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}))>;
+			decltype(allocator_traits<Allocator>::allocate(std::declval<Allocator&>(), size_t{}, std::align_val_t{}))>;
 
-		[[nodiscard]]
+		SOAGEN_NODISCARD
 		constexpr allocation allocate(size_t n_bytes, size_t alignment) noexcept(allocate_is_nothrow)
 		{
 			SOAGEN_ASSUME(n_bytes);
-			SOAGEN_ASSUME(has_single_bit(alignment));
+			SOAGEN_ASSUME((static_cast<size_t>(alignment) & (static_cast<size_t>(alignment) - 1u)) == 0u);
 
-			const auto ptr = soagen::assume_aligned<allocator_traits::min_alignment>(
-				allocator_traits::allocate(allocator(),
-										   n_bytes,
-										   std::align_val_t{ max(alignment, allocator_traits::min_alignment) }));
+			const auto ptr = soagen::assume_aligned<allocator_traits<Allocator>::min_alignment>(
+				allocator_traits<Allocator>::allocate(
+					allocator(),
+					n_bytes,
+					std::align_val_t{ max(alignment, allocator_traits<Allocator>::min_alignment) }));
 			SOAGEN_ASSUME(ptr != nullptr);
 			std::memset(ptr, 0, n_bytes);
 
 			if constexpr (std::is_same_v<allocator_pointer_type, std::byte*>)
 				return { { ptr }, n_bytes };
 			else
 				return { { reinterpret_cast<std::byte*>(ptr) }, n_bytes };
@@ -3968,454 +4965,473 @@
 
 		constexpr void deallocate(const allocation& al) noexcept
 		{
 			SOAGEN_ASSUME(al.columns[0]);
 			SOAGEN_ASSUME(al.size_in_bytes);
 
 			if constexpr (std::is_same_v<allocator_pointer_type, std::byte*>)
-				allocator_traits::deallocate(allocator(), al.columns[0], al.size_in_bytes);
+				allocator_traits<Allocator>::deallocate(allocator(), al.columns[0], al.size_in_bytes);
 			else
-				allocator_traits::deallocate(allocator(),
-											 reinterpret_cast<allocator_pointer_type>(al.columns[0]),
-											 al.size_in_bytes);
+				allocator_traits<Allocator>::deallocate(allocator(),
+														reinterpret_cast<allocator_pointer_type>(al.columns[0]),
+														al.size_in_bytes);
 		}
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructibility
 	//------------------------------------------------------------------------------------------------------------------
 
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_base
+#undef SOAGEN_BASE_TYPE
+#define SOAGEN_BASE_TYPE SOAGEN_BASE_NAME<ColumnCount, Allocator>
+
 	template <size_t ColumnCount,
 			  typename Allocator,
-			  typename Base = table_base<ColumnCount, Allocator>,
-			  bool			= std::is_default_constructible_v<Allocator>>
+			  bool = std::is_default_constructible_v<Allocator>>
 	class SOAGEN_EMPTY_BASES table_default_construct //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FOUR(table_default_construct);
 
 		SOAGEN_NODISCARD_CTOR
 		constexpr table_default_construct() noexcept //
-			: Base{ Allocator{} }
+			: SOAGEN_BASE_TYPE{ Allocator{} }
 		{
 			static_assert(std::is_nothrow_default_constructible_v<Allocator>,
 						  "allocators must be nothrow default-constructible, or not default-constructible at all");
 		}
 	};
 
-	template <size_t ColumnCount, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_default_construct<ColumnCount, Allocator, Base, false> //
-		: public Base
+	template <size_t ColumnCount, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_default_construct<ColumnCount, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_default_construct);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: move-assignment (un-typed base parts only)
 	//------------------------------------------------------------------------------------------------------------------
 
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_default_construct
+
 	template <size_t ColumnCount,
 			  typename Allocator,
-			  typename Base = table_default_construct<ColumnCount, Allocator>,
-			  bool			= !allocator_traits<Allocator>::propagate_on_container_move_assignment::value
+			  bool = !allocator_traits<Allocator>::propagate_on_container_move_assignment::value
 				  || std::is_move_assignable_v<Allocator>>
 	class SOAGEN_EMPTY_BASES table_move_assignable_base //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
 	  protected:
-		using allocation	   = table_allocation<ColumnCount>;
-		using allocator_traits = allocator_traits<Allocator>;
+		using allocation = table_allocation<ColumnCount>;
 
 		constexpr bool move_from_by_taking_ownership(table_move_assignable_base&& rhs) noexcept
 		{
 			SOAGEN_ASSUME(&rhs != this);
 
 			const auto take_ownership = [&]() noexcept
 			{
-				if (Base::alloc_)
-					Base::deallocate(Base::alloc_);
+				if (base::alloc_)
+					base::deallocate(base::alloc_);
 
-				Base::alloc_			= std::exchange(rhs.alloc_, allocation{});
-				Base::count_			= std::exchange(rhs.count_, size_t{});
-				Base::capacity_.first() = std::exchange(rhs.capacity_.first(), size_t{});
+				base::alloc_			= std::exchange(rhs.alloc_, allocation{});
+				base::count_			= std::exchange(rhs.count_, size_t{});
+				base::capacity_.first() = std::exchange(rhs.capacity_.first(), size_t{});
 
-				if constexpr (allocator_traits::propagate_on_container_move_assignment::value)
+				if constexpr (allocator_traits<Allocator>::propagate_on_container_move_assignment::value)
 				{
 					static_assert(std::is_nothrow_move_assignable_v<Allocator>,
 								  "move-propagated allocators must be nothrow move-assignable");
 
-					Base::allocator() = static_cast<Allocator&&>(rhs.allocator());
+					base::allocator() = static_cast<Allocator&&>(rhs.allocator());
 				}
 			};
 
-			if constexpr (allocator_traits::container_move_assign_always_takes_ownership)
+			if constexpr (allocator_traits<Allocator>::container_move_assign_always_takes_ownership)
 			{
 				take_ownership();
 				return true;
 			}
 			else
 			{
-				if (allocator_traits::equal(Base::allocator(), rhs.allocator()))
+				if (allocator_traits<Allocator>::equal(base::allocator(), rhs.allocator()))
 				{
 					take_ownership();
 					return true;
 				}
 
 				// if they compare non-equal then we need to do elementwise move-assignment,
 				// which can't be implemented at this untyped level - must be implemented as part of a more specialized
 				// child class.
 
 				return false;
 			}
 		}
 
+		template <typename T>
+		constexpr bool move_from_by_taking_ownership(T&& rhs, std::true_type) noexcept
+		{
+			return move_from_by_taking_ownership(static_cast<table_move_assignable_base&&>(rhs));
+		}
+
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		table_move_assignable_base()											 = default;
 		table_move_assignable_base(table_move_assignable_base&&)				 = default;
 		table_move_assignable_base(const table_move_assignable_base&)			 = default;
 		table_move_assignable_base& operator=(const table_move_assignable_base&) = default;
 
 		constexpr table_move_assignable_base& operator=(table_move_assignable_base&& rhs) noexcept
 		{
 			if SOAGEN_LIKELY(&rhs != this)
 				move_from_by_taking_ownership(static_cast<table_move_assignable_base&&>(rhs));
 			return *this;
 		}
 	};
 
-	template <size_t ColumnCount, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_move_assignable_base<ColumnCount, Allocator, Base, false> //
-		: public Base
+	template <size_t ColumnCount, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_move_assignable_base<ColumnCount, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_move_assignable_base);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: swap
 	//------------------------------------------------------------------------------------------------------------------
 
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_move_assignable_base
+
 	template <size_t ColumnCount,
 			  typename Allocator,
-			  typename Base = table_move_assignable_base<ColumnCount, Allocator>,
 			  bool = !allocator_traits<Allocator>::propagate_on_container_swap::value || std::is_swappable_v<Allocator>>
 	class SOAGEN_EMPTY_BASES table_swap //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_swap);
 
 		constexpr void swap(table_swap& other) noexcept
 		{
 			if SOAGEN_UNLIKELY(&other == this)
 				return;
 
-			using allocator_traits = soagen::allocator_traits<Allocator>;
-
-			if constexpr (!allocator_traits::propagate_on_container_swap::value
-						  && !allocator_traits::is_always_equal::value)
+			if constexpr (!allocator_traits<Allocator>::propagate_on_container_swap::value
+						  && !allocator_traits<Allocator>::is_always_equal::value)
 			{
-				SOAGEN_ASSERT(Base::allocator() == other.allocator()
+				SOAGEN_ASSERT(base::allocator() == other.allocator()
 							  && "allocators must compare equal in a non-propagating swap");
 			}
 
 			using std::swap;
-			swap(Base::alloc_, other.alloc_);
-			swap(Base::count_, other.count_);
-			swap(Base::capacity_.first(), other.capacity_.first());
+			swap(base::alloc_, other.alloc_);
+			swap(base::count_, other.count_);
+			swap(base::capacity_.first(), other.capacity_.first());
 
-			if constexpr (allocator_traits::propagate_on_container_swap::value)
+			if constexpr (allocator_traits<Allocator>::propagate_on_container_swap::value)
 			{
 				static_assert(std::is_nothrow_swappable_v<Allocator>,
 							  "swap-propagated allocators must be nothrow-swappable");
 
-				swap(Base::allocator(), other.allocator());
+				swap(base::allocator(), other.allocator());
 			}
 		}
 	};
 
-	template <size_t ColumnCount, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_swap<ColumnCount, Allocator, Base, false> //
-		: public Base
+	template <size_t ColumnCount, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_swap<ColumnCount, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_swap);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: typed base
 	//
-	// note: specializations from here down take the full TableTraits, not just the ColumnCount
+	// note: specializations from here down take the full Traits, not just the ColumnCount
 	//------------------------------------------------------------------------------------------------------------------
 
-	template <typename TableTraits,
-			  typename Allocator,
-			  typename Base = table_swap<TableTraits::column_count, Allocator>>
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_swap
+#undef SOAGEN_BASE_TYPE
+#define SOAGEN_BASE_TYPE SOAGEN_BASE_NAME<Traits::column_count, Allocator>
+
+	template <typename Traits, typename Allocator>
 	class SOAGEN_EMPTY_BASES table_typed_base //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
 	  private:
-		using allocation  = table_allocation<TableTraits::column_count>;
-		using column_ends = size_t[TableTraits::column_count];
+		using allocation  = table_allocation<Traits::column_count>;
+		using column_ends = size_t[Traits::column_count];
+		using base		  = SOAGEN_BASE_TYPE;
 
 		static constexpr void calc_column_ends(column_ends& ends, size_t capacity) noexcept
 		{
 			// pad ends so the next column starts at the right alignment for the storage type
 			size_t prev = {};
-			for (size_t i = 0; i < TableTraits::column_count - 1u; i++)
+			for (size_t i = 0; i < Traits::column_count - 1u; i++)
 			{
-				ends[i] = prev + TableTraits::column_sizes[i] * capacity;
-				ends[i] = (ends[i] + TableTraits::column_alignments[i + 1u] - 1u) //
-						& ~(TableTraits::column_alignments[i + 1u] - 1u);
+				ends[i] = prev + Traits::column_sizes[i] * capacity;
+				ends[i] = (ends[i] + Traits::column_alignments[i + 1u] - 1u) //
+						& ~(Traits::column_alignments[i + 1u] - 1u);
 
-				SOAGEN_ASSUME(ends[i] % TableTraits::column_alignments[i + 1u] == 0u);
+				SOAGEN_ASSUME(ends[i] % Traits::column_alignments[i + 1u] == 0u);
 				prev = ends[i];
 			}
 
 			// last end doesn't need to be aligned (it's just the total buffer size)
-			ends[TableTraits::column_count - 1u] =
-				prev + TableTraits::column_sizes[TableTraits::column_count - 1u] * capacity;
+			ends[Traits::column_count - 1u] = prev + Traits::column_sizes[Traits::column_count - 1u] * capacity;
 		}
 
-		constexpr allocation allocate(const column_ends& ends) noexcept(Base::allocate_is_nothrow)
+		constexpr allocation allocate(const column_ends& ends) noexcept(base::allocate_is_nothrow)
 		{
-			SOAGEN_ASSUME(ends[TableTraits::column_count - 1u]);
+			SOAGEN_ASSUME(ends[Traits::column_count - 1u]);
 
-			auto alloc = Base::allocate(ends[TableTraits::column_count - 1u], TableTraits::largest_alignment);
+			auto alloc = base::allocate(ends[Traits::column_count - 1u], Traits::largest_alignment);
 			SOAGEN_ASSUME(alloc.columns[0]);
-			SOAGEN_ASSUME(alloc.size_in_bytes == ends[TableTraits::column_count - 1u]);
+			SOAGEN_ASSUME(alloc.size_in_bytes == ends[Traits::column_count - 1u]);
 
-			for (size_t i = 1; i < TableTraits::column_count; i++)
+			for (size_t i = 1; i < Traits::column_count; i++)
 			{
 				alloc.columns[i] = alloc.columns[0] + ends[i - 1u];
-				SOAGEN_ASSUME(reinterpret_cast<uintptr_t>(alloc.columns[i]) % TableTraits::column_alignments[i] == 0u);
+				SOAGEN_ASSUME(reinterpret_cast<uintptr_t>(alloc.columns[i]) % Traits::column_alignments[i] == 0u);
 			}
 
 			return alloc;
 		}
 
 		SOAGEN_CPP20_CONSTEXPR
 		void adjust_capacity(size_t new_capacity) noexcept(
-			Base::allocate_is_nothrow
-			&& (TableTraits::all_nothrow_move_constructible
-				|| (TableTraits::all_nothrow_default_constructible && TableTraits::all_nothrow_move_assignable)
-				|| TableTraits::all_nothrow_copy_constructible
-				|| (TableTraits::all_nothrow_default_constructible && TableTraits::all_nothrow_copy_assignable)))
+			base::allocate_is_nothrow
+			&& (Traits::all_nothrow_move_constructible
+				|| (Traits::all_nothrow_default_constructible && Traits::all_nothrow_move_assignable)
+				|| Traits::all_nothrow_copy_constructible
+				|| (Traits::all_nothrow_default_constructible && Traits::all_nothrow_copy_assignable)))
 		{
 			SOAGEN_ASSUME(new_capacity);
-			SOAGEN_ASSUME(new_capacity >= Base::count_);
+			SOAGEN_ASSUME(new_capacity >= base::count_);
 
-			if (new_capacity == Base::capacity())
+			if (new_capacity == base::capacity())
 				return;
 
 			// get new ends
 			column_ends new_ends{};
 			calc_column_ends(new_ends, new_capacity);
 
 			// alloc + move
 			auto new_alloc = allocate(new_ends);
 			SOAGEN_ASSERT(new_alloc);
-			if (Base::count_)
+			if (base::count_)
 			{
-				SOAGEN_ASSERT(Base::alloc_);
+				SOAGEN_ASSERT(base::alloc_);
 
 				// this looks a bit convoluted and is probably worth an explainer:
 				// we really, really, _really_ don't want reserve() and shrink_to_fit() to throw if we can avoid it,
 				// since it potentially leaves the container in a sliced state (i.e. some elements were moved already
 				// when an exception is raised), so we're moving or copying the elements according to the 'most nothrow'
 				// path that still fulfills the brief.
 
-				if constexpr (TableTraits::all_nothrow_move_constructible)
+				if constexpr (Traits::all_nothrow_move_constructible)
 				{
-					TableTraits::move_construct_rows(new_alloc.columns, {}, Base::alloc_.columns, {}, Base::count_);
+					Traits::move_construct_rows(new_alloc.columns, {}, base::alloc_.columns, {}, base::count_);
 				}
-				else if constexpr (TableTraits::all_nothrow_default_constructible
-								   && TableTraits::all_nothrow_move_assignable)
+				else if constexpr (Traits::all_nothrow_default_constructible && Traits::all_nothrow_move_assignable)
 				{
-					TableTraits::default_construct_rows(new_alloc.columns, {}, Base::count_);
-					TableTraits::move_assign_rows(new_alloc.columns, {}, Base::alloc_.columns, {}, Base::count_);
+					Traits::default_construct_rows(new_alloc.columns, {}, base::count_);
+					Traits::move_assign_rows(new_alloc.columns, {}, base::alloc_.columns, {}, base::count_);
 				}
-				else if constexpr (TableTraits::all_nothrow_copy_constructible)
+				else if constexpr (Traits::all_nothrow_copy_constructible)
 				{
-					TableTraits::copy_construct_rows(new_alloc, {}, Base::alloc_.columns, {}, Base::count_);
+					Traits::copy_construct_rows(new_alloc, {}, base::alloc_.columns, {}, base::count_);
 				}
-				else if constexpr (TableTraits::all_nothrow_default_constructible
-								   && TableTraits::all_nothrow_copy_assignable)
+				else if constexpr (Traits::all_nothrow_default_constructible && Traits::all_nothrow_copy_assignable)
 				{
-					TableTraits::default_construct_rows(new_alloc, {}, Base::count_);
-					TableTraits::copy_assign_rows(new_alloc, {}, Base::alloc_.columns, {}, Base::count_);
+					Traits::default_construct_rows(new_alloc, {}, base::count_);
+					Traits::copy_assign_rows(new_alloc, {}, base::alloc_.columns, {}, base::count_);
 				}
 				else
 				{
 					[[maybe_unused]] bool needs_destruct = false;
 					try
 					{
-						if constexpr (TableTraits::all_move_constructible)
+						if constexpr (Traits::all_move_constructible)
 						{
-							TableTraits::move_construct_rows(new_alloc,
-															 {},
-															 Base::alloc_.columns,
-															 {},
-															 Base::count_); // strong
+							Traits::move_construct_rows(new_alloc,
+														{},
+														base::alloc_.columns,
+														{},
+														base::count_); // strong
 						}
-						else if constexpr (TableTraits::all_default_constructible && TableTraits::all_move_assignable)
+						else if constexpr (Traits::all_default_constructible && Traits::all_move_assignable)
 						{
-							TableTraits::default_construct_rows(new_alloc, {}, Base::count_); // strong
+							Traits::default_construct_rows(new_alloc, {}, base::count_); // strong
 							needs_destruct = true;
-							TableTraits::move_assign_rows(new_alloc, {}, Base::alloc_.columns, {}, Base::count_);
+							Traits::move_assign_rows(new_alloc, {}, base::alloc_.columns, {}, base::count_);
 						}
-						else if constexpr (TableTraits::all_copy_constructible)
+						else if constexpr (Traits::all_copy_constructible)
 						{
-							TableTraits::copy_construct_rows(new_alloc,
-															 {},
-															 Base::alloc_.columns,
-															 {},
-															 Base::count_); // strong
+							Traits::copy_construct_rows(new_alloc,
+														{},
+														base::alloc_.columns,
+														{},
+														base::count_); // strong
 						}
-						else if constexpr (TableTraits::all_default_constructible && TableTraits::all_copy_assignable)
+						else if constexpr (Traits::all_default_constructible && Traits::all_copy_assignable)
 						{
-							TableTraits::default_construct_rows(new_alloc, {}, Base::count_); // strong
+							Traits::default_construct_rows(new_alloc, {}, base::count_); // strong
 							needs_destruct = true;
-							TableTraits::copy_assign_rows(new_alloc, {}, Base::alloc_.columns, {}, Base::count_);
+							Traits::copy_assign_rows(new_alloc, {}, base::alloc_.columns, {}, base::count_);
 						}
 					}
 					catch (...)
 					{
 						if (needs_destruct)
-							TableTraits::destruct_rows(new_alloc, {}, Base::count_);
-						Base::deallocate(new_alloc);
+							Traits::destruct_rows(new_alloc, {}, base::count_);
+						base::deallocate(new_alloc);
 						throw;
 					}
 				}
-				TableTraits::destruct_rows(Base::alloc_.columns, {}, Base::count_);
-				Base::deallocate(Base::alloc_);
+				Traits::destruct_rows(base::alloc_.columns, {}, base::count_);
+				base::deallocate(base::alloc_);
 			}
-			Base::alloc_			= new_alloc;
-			Base::capacity_.first() = new_capacity;
+			base::alloc_			= new_alloc;
+			base::capacity_.first() = new_capacity;
 		}
 
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_typed_base);
 
 		~table_typed_base() noexcept
 		{
 			clear();
 		}
 
 		constexpr void clear() noexcept
 		{
-			if constexpr (!TableTraits::all_trivially_destructible)
+			if constexpr (!Traits::all_trivially_destructible)
 			{
-				static_assert(TableTraits::all_nothrow_destructible,
-							  "column storage_types must be nothrow-destructible");
+				static_assert(Traits::all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
-				if (Base::count_)
-					TableTraits::destruct_rows(Base::alloc_.columns, {}, Base::count_);
+				if (base::count_)
+					Traits::destruct_rows(base::alloc_.columns, {}, base::count_);
 			}
-			Base::count_ = {};
+			base::count_ = {};
 		}
 
 		SOAGEN_CPP20_CONSTEXPR
 		void reserve(size_t new_capacity) noexcept(noexcept(this->adjust_capacity(size_t{})))
 		{
 			if (!new_capacity)
 				return;
 
-			if (const size_t rem = new_capacity % TableTraits::aligned_stride; rem > 0u)
+			if constexpr (Traits::aligned_stride > 1)
 			{
-				static_cast<void>(
-					add_without_overflowing(new_capacity, TableTraits::aligned_stride - rem, new_capacity));
+				if (const size_t rem = new_capacity % Traits::aligned_stride; rem > 0u)
+				{
+					static_cast<void>(
+						add_without_overflowing(new_capacity, Traits::aligned_stride - rem, new_capacity));
+				}
 			}
-			if (new_capacity <= Base::capacity())
+			if (new_capacity <= base::capacity())
 				return;
 
 			adjust_capacity(new_capacity);
 		}
 
 		SOAGEN_CPP20_CONSTEXPR
 		void shrink_to_fit() noexcept(noexcept(this->adjust_capacity(size_t{})))
 		{
-			if (!Base::count_)
+			if (!base::count_)
 			{
-				if (Base::alloc_)
+				if (base::alloc_)
 				{
-					Base::deallocate(Base::alloc_);
-					Base::alloc_			= {};
-					Base::capacity_.first() = {};
+					base::deallocate(base::alloc_);
+					base::alloc_			= {};
+					base::capacity_.first() = {};
 				}
 				return;
 			}
 
-			auto new_capacity = Base::count_;
-			if (const size_t rem = new_capacity % TableTraits::aligned_stride; rem > 0u)
+			auto new_capacity = base::count_;
+			if constexpr (Traits::aligned_stride > 1)
 			{
-				static_cast<void>(
-					add_without_overflowing(new_capacity, TableTraits::aligned_stride - rem, new_capacity));
+				if (const size_t rem = new_capacity % Traits::aligned_stride; rem > 0u)
+				{
+					static_cast<void>(
+						add_without_overflowing(new_capacity, Traits::aligned_stride - rem, new_capacity));
+				}
 			}
-			if (new_capacity == Base::capacity())
+			if (new_capacity >= base::capacity())
 				return;
-			SOAGEN_ASSERT(new_capacity < Base::capacity());
-			SOAGEN_ASSERT(new_capacity >= Base::count_);
 
 			adjust_capacity(new_capacity);
 		}
 
 		SOAGEN_CPP20_CONSTEXPR
 		void pop_back(size_t num = 1) noexcept
 		{
-			static_assert(TableTraits::all_nothrow_destructible, "column storage_types must be nothrow-destructible");
+			static_assert(Traits::all_nothrow_destructible, "column storage_types must be nothrow-destructible");
 
-			num = min(Base::count_, num);
-			TableTraits::destruct_rows(Base::alloc_.columns, Base::count_ - num, num);
-			Base::count_ -= num;
+			num = min(base::count_, num);
+			Traits::destruct_rows(base::alloc_.columns, base::count_ - num, num);
+			base::count_ -= num;
 		}
 
 	  public:
 		static constexpr size_t max_capacity = []() -> size_t
 		{
-			if constexpr (TableTraits::column_count == 1)
+			if constexpr (Traits::column_count == 1)
 			{
-				return static_cast<size_t>(-1) / TableTraits::column_sizes[0];
+				return static_cast<size_t>(-1) / Traits::column_sizes[0];
 			}
 			else
 			{
 				// todo: i'm sure there's a smarter way to do this
 
 				constexpr auto capacity_ok = [](size_t cap) noexcept
 				{
 					size_t buf_end = {};
-					for (size_t i = 0u; i < TableTraits::column_count; i++)
+					for (size_t i = 0u; i < Traits::column_count; i++)
 					{
 						if (i)
 						{
-							if (const size_t rem = buf_end % TableTraits::column_alignments[i - 1u]; rem > 0u)
+							if (const size_t rem = buf_end % Traits::column_alignments[i - 1u]; rem > 0u)
 							{
-								if (!add_without_overflowing(buf_end,
-															 TableTraits::column_alignments[i - 1u] - rem,
-															 buf_end))
+								if (!add_without_overflowing(buf_end, Traits::column_alignments[i - 1u] - rem, buf_end))
 									return false;
 							}
 						}
-						if (!add_without_overflowing(buf_end, TableTraits::column_sizes[i] * cap, buf_end))
+						if (!add_without_overflowing(buf_end, Traits::column_sizes[i] * cap, buf_end))
 							return false;
 					}
 					return true;
 				};
 
 				size_t lower  = static_cast<size_t>(-1);
 				size_t higher = lower;
@@ -4447,497 +5463,1335 @@
 		constexpr size_t max_size() const noexcept
 		{
 			return max_capacity;
 		}
 
 	  private:
 		SOAGEN_CPP20_CONSTEXPR
-		void grow_if_necessary(size_t new_elements) noexcept(noexcept(this->reserve(size_t{})))
+		void grow_if_necessary(size_t new_elements)
 		{
-			const auto new_size = Base::size() + new_elements; // todo: throw if this would overflow?
-			if (new_size <= Base::capacity())
+			SOAGEN_ASSUME(new_elements);
+
+			// determine the minimum required allocation size to store the new elements.
+			// if this calculation would overflow or the result would exceed max_capacity then we've
+			// hit system limits and have no choice but to raise std::bad_alloc.
+			auto new_size = base::count_;
+			if SOAGEN_UNLIKELY(!add_without_overflowing(new_size, new_elements, new_size) || new_size > max_capacity)
+				throw std::bad_alloc{};
+
+			// already enough capacity, no work to do.
+			if (new_size <= base::capacity())
 				return;
 
+			// again we need to check system limits, this time when applying the growth factor.
+			// if we overflow or would exceed the max capacity then clamp the result to max_capacity
+			// (the user is right on the edge of hitting system limits and will hit them at the next growth)
 			auto new_cap = new_size;
-			if (!add_without_overflowing(new_cap, new_cap, new_cap)) // new_cap *= 2
+			if SOAGEN_UNLIKELY(!add_without_overflowing(new_cap, new_cap, new_cap) || new_cap > max_capacity)
 				new_cap = max_capacity;
 
 			reserve(new_cap);
 		}
 
 	  public:
-		SOAGEN_CONSTRAINED_TEMPLATE(TableTraits::template row_constructible_from<Args&&...>, typename... Args)
+		SOAGEN_CONSTRAINED_TEMPLATE(Traits::template row_constructible_from<Args&&...>, typename... Args)
 		SOAGEN_CPP20_CONSTEXPR
-		void emplace_back(Args&&... args) noexcept(							//
-			TableTraits::template row_nothrow_constructible_from<Args&&...> //
+		void emplace_back(Args&&... args) noexcept(					   //
+			Traits::template row_nothrow_constructible_from<Args&&...> //
 				&& noexcept(this->grow_if_necessary(size_t{})))
 		{
 			grow_if_necessary(1u);
-			TableTraits::construct_row(Base::alloc_.columns, Base::count_, static_cast<Args&&>(args)...);
-			Base::count_++;
+			Traits::construct_row(base::alloc_.columns, base::count_, static_cast<Args&&>(args)...);
+			base::count_++;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE(Traits::all_move_constructible	   //
+										&& Traits::all_move_assignable //
+											&& Traits::template row_constructible_from<Args&&...>,
+									typename... Args)
+		SOAGEN_CPP20_CONSTEXPR
+		void emplace(size_t position, Args&&... args) noexcept(					  //
+			Traits::all_nothrow_move_constructible								  //
+				&& Traits::all_nothrow_move_assignable							  //
+					&& Traits::template row_nothrow_constructible_from<Args&&...> //
+						&& noexcept(this->grow_if_necessary(size_t{})))
+		{
+			SOAGEN_ASSUME(position <= base::count_);
+
+			// delegating to emplace_back for the end position is ideal
+			// because emplace_back never needs to move+destruct elements (modulo re-allocation)
+			if (position == base::count_)
+			{
+				emplace_back(static_cast<Args&&>(args)...);
+				return;
+			}
+
+			// move construct the last element (since it is new)
+			grow_if_necessary(1u);
+			Traits::move_construct_row(base::alloc_.columns, base::count_, base::alloc_.columns, base::count_ - 1u);
+
+			// move-assign the rest of the elements (they were already alive)
+			if (position + 1u < base::count_)
+			{
+				Traits::move_assign_rows(base::alloc_.columns,
+										 position + 1u,
+										 base::alloc_.columns,
+										 position,
+										 base::count_ - position - 1u);
+			}
+
+			// todo: there might be some inputs that allow us to move-assign instead of destruct+construct
+			Traits::destruct_row(base::alloc_.columns, position);
+			Traits::construct_row(base::alloc_.columns, position, static_cast<Args&&>(args)...);
+
+			base::count_++;
 		}
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: default-constructible column types
 	//------------------------------------------------------------------------------------------------------------------
 
-	template <typename TableTraits, //
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_typed_base
+#undef SOAGEN_BASE_TYPE
+#define SOAGEN_BASE_TYPE SOAGEN_BASE_NAME<Traits, Allocator>
+
+	template <typename Traits, //
 			  typename Allocator,
-			  typename Base = table_typed_base<TableTraits, Allocator>,
-			  bool			= TableTraits::all_default_constructible>
+			  bool = Traits::all_default_constructible>
 	class SOAGEN_EMPTY_BASES table_default_constructible_columns //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_default_constructible_columns);
 
 		SOAGEN_CPP20_CONSTEXPR
-		void resize(size_t num) noexcept(				   //
-			TableTraits::all_nothrow_default_constructible //
-				&& noexcept(this->pop_back(size_t{}))	   //
+		void resize(size_t num) noexcept(			  //
+			Traits::all_nothrow_default_constructible //
+				&& noexcept(this->pop_back(size_t{})) //
 					&& noexcept(this->reserve(size_t{})))
 		{
-			if (Base::size() > num)
+			if (base::size() > num)
 			{
-				Base::pop_back(Base::size() - num);
+				base::pop_back(base::size() - num);
 			}
-			else if (Base::size() < num)
+			else if (base::size() < num)
 			{
-				Base::reserve(num);
-				for (size_t i = Base::size(); i < num; i++)
+				base::reserve(num);
+				for (size_t i = base::size(); i < num; i++)
 				{
-					TableTraits::default_construct_row(Base::alloc_.columns, i);
-					Base::count_++;
+					Traits::default_construct_row(base::alloc_.columns, i);
+					base::count_++;
 				}
 			}
 		}
 	};
 
-	template <typename TableTraits, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_default_constructible_columns<TableTraits, Allocator, Base, false> //
-		: public Base
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_default_constructible_columns<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_default_constructible_columns);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: move-assignment (typed)
 	//------------------------------------------------------------------------------------------------------------------
 
-	template <typename TableTraits, //
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_default_constructible_columns
+
+	template <typename Traits, //
 			  typename Allocator,
-			  typename Base = table_default_constructible_columns<TableTraits, Allocator>,
-			  bool UseBase	= !std::is_move_assignable_v<Base>
+			  bool UseBase = !std::is_move_assignable_v<SOAGEN_BASE_TYPE>
 						  || allocator_traits<Allocator>::container_move_assign_always_takes_ownership,
-			  bool Movable = (TableTraits::all_move_assignable && TableTraits::all_move_constructible)>
+			  bool Movable = (Traits::all_move_assignable && Traits::all_move_constructible)>
 	class SOAGEN_EMPTY_BASES table_move_assign //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
-	  protected:
-		using allocator_traits = allocator_traits<Allocator>;
+	  private:
+		using base = SOAGEN_BASE_TYPE;
 
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		table_move_assign()									   = default;
 		table_move_assign(table_move_assign&&)				   = default;
 		table_move_assign(const table_move_assign& other)	   = default;
 		table_move_assign& operator=(const table_move_assign&) = default;
 
 		// note that this is only specialized when allocator_traits::container_move_assign_always_takes_ownership
 		// is false - if it's true then the untyped base move-assign operator is already complete and no elementwise
 		// moving will ever need to take place
 		static_assert(!UseBase);
 		static_assert(Movable);
 
 		table_move_assign& operator=(table_move_assign&& rhs) noexcept( //
-			TableTraits::all_nothrow_move_assignable					//
-				&& TableTraits::all_nothrow_move_constructible			//
-					&& noexcept(Base::clear())							//
-						&& noexcept(Base::pop_back())					//
-							&& noexcept(Base::reserve(size_t{})))
+			Traits::all_nothrow_move_assignable							//
+				&& Traits::all_nothrow_move_constructible				//
+					&& noexcept(base::clear())							//
+						&& noexcept(base::pop_back())					//
+							&& noexcept(base::reserve(size_t{})))
 		{
 			if SOAGEN_UNLIKELY(&rhs == this)
 				return *this;
 
-			static_assert(!allocator_traits::propagate_on_container_move_assignment::value);
-			static_assert(!allocator_traits::is_always_equal::value);
+			static_assert(!allocator_traits<Allocator>::propagate_on_container_move_assignment::value);
+			static_assert(!allocator_traits<Allocator>::is_always_equal::value);
 
-			if (Base::move_from_by_taking_ownership(static_cast<table_move_assignable_base&&>(rhs)))
+			if (base::move_from_by_taking_ownership(rhs, std::true_type{}))
 				return *this;
 
-			SOAGEN_ASSERT(!allocator_traits::equal(Base::allocator(), rhs.allocator()));
+			SOAGEN_ASSERT(!allocator_traits<Allocator>::equal(base::allocator(), rhs.allocator()));
 
 			if (rhs.empty())
 			{
-				Base::clear();
+				base::clear();
 				return *this;
 			}
 
-			if (rhs.size() < Base::size())
-				Base::pop_back(Base::size() - rhs.size());
+			if (rhs.size() < base::size())
+				base::pop_back(base::size() - rhs.size());
 
-			Base::reserve(rhs.size());
+			base::reserve(rhs.size());
 
-			const auto assigned_end = min(Base::size(), rhs.size());
+			const auto assigned_end = min(base::size(), rhs.size());
 			for (size_t i = 0; i < assigned_end; i++)
-				TableTraits::move_assign_row(Base::alloc_.columns, i, rhs.alloc_.columns, i);
+				Traits::move_assign_row(base::alloc_.columns, i, rhs.alloc_.columns, i);
 
-			const auto constructed_end = max(Base::size(), rhs.size());
+			const auto constructed_end = max(base::size(), rhs.size());
 			for (size_t i = assigned_end; i < constructed_end; i++)
 			{
-				TableTraits::move_construct_row(Base::alloc_.columns, i, rhs.alloc_.columns, i);
-				Base::count_++;
+				Traits::move_construct_row(base::alloc_.columns, i, rhs.alloc_.columns, i);
+				base::count_++;
 			}
 
 			return *this;
 		}
 	};
 
-	template <typename TableTraits, typename Allocator, typename Base, bool Movable>
-	class SOAGEN_EMPTY_BASES table_move_assign<TableTraits, Allocator, Base, /*UseBase*/ true, Movable> //
-		: public Base
+	template <typename Traits, typename Allocator, bool Movable>
+	class SOAGEN_EMPTY_BASES table_move_assign<Traits, Allocator, /*UseBase*/ true, Movable> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_move_assign);
 	};
 
-	template <typename TableTraits, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_move_assign<TableTraits, Allocator, Base, /*UseBase*/ false, /*Movable*/ false> //
-		: public Base
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_move_assign<Traits, Allocator, /*UseBase*/ false, /*Movable*/ false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		table_move_assign()									   = default;
 		table_move_assign(table_move_assign&&)				   = default;
 		table_move_assign(const table_move_assign&)			   = default;
 		table_move_assign& operator=(const table_move_assign&) = default;
 
 		// base operator is insufficient but the elements aren't movable so no choice but to explicitly delete
 		table_move_assign& operator=(table_move_assign&&) = delete;
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: copy-construct
 	//------------------------------------------------------------------------------------------------------------------
 
-	template <typename TableTraits, //
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_move_assign
+
+	template <typename Traits, //
 			  typename Allocator,
-			  typename Base = table_move_assign<TableTraits, Allocator>,
-			  bool			= TableTraits::all_copy_constructible&& std::is_copy_constructible_v<Allocator>>
+			  bool = Traits::all_copy_constructible&& std::is_copy_constructible_v<Allocator>>
 	class SOAGEN_EMPTY_BASES table_copy_construct //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
-	  protected:
-		using allocator_traits = allocator_traits<Allocator>;
+	  private:
+		using base = SOAGEN_BASE_TYPE;
 
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		table_copy_construct()										 = default;
 		table_copy_construct(table_copy_construct&&)				 = default;
 		table_copy_construct& operator=(table_copy_construct&&)		 = default;
 		table_copy_construct& operator=(const table_copy_construct&) = default;
 
-		table_copy_construct(const table_copy_construct& other) noexcept(TableTraits::all_nothrow_copy_constructible //
-																			 && noexcept(Base::reserve(size_t{})))
-			: Base{ allocator_traits::select_on_container_copy_construction(Base::allocator()) }
+		table_copy_construct(const table_copy_construct& other) noexcept(Traits::all_nothrow_copy_constructible //
+																			 && noexcept(base::reserve(size_t{})))
+			: base{ allocator_traits<Allocator>::select_on_container_copy_construction(base::allocator()) }
 		{
 			static_assert(std::is_nothrow_copy_constructible_v<Allocator>,
 						  "allocators must be nothrow copy-constructible");
 
-			Base::reserve(other.size());
-			TableTraits::copy_construct_rows(Base::alloc_.columns, {}, other.alloc_.columns, {}, other.size());
-			Base::count_ = other.size();
+			base::reserve(other.size());
+			Traits::copy_construct_rows(base::alloc_.columns, {}, other.alloc_.columns, {}, other.size());
+			base::count_ = other.size();
 		}
 	};
 
-	template <typename TableTraits, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_copy_construct<TableTraits, Allocator, Base, false> //
-		: public Base
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_copy_construct<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_copy_construct);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: copy-assign
 	//------------------------------------------------------------------------------------------------------------------
 
-	template <typename TableTraits,
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_copy_construct
+
+	template <typename Traits,
 			  typename Allocator,
-			  typename Base = table_copy_construct<TableTraits, Allocator>,
-			  bool			= TableTraits::all_copy_assignable	//
-						 && TableTraits::all_copy_constructible //
+			  bool = Traits::all_copy_assignable		   //
+						 && Traits::all_copy_constructible //
 				  && (!allocator_traits<Allocator>::propagate_on_container_copy_assignment::value
 					  || std::is_copy_assignable_v<Allocator>)>
 	class SOAGEN_EMPTY_BASES table_copy_assign //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
-	  protected:
-		using allocator_traits = allocator_traits<Allocator>;
+	  private:
+		using base = SOAGEN_BASE_TYPE;
 
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		table_copy_assign()								  = default;
 		table_copy_assign(table_copy_assign&&)			  = default;
 		table_copy_assign& operator=(table_copy_assign&&) = default;
 		table_copy_assign(const table_copy_assign&)		  = default;
 
 		constexpr table_copy_assign& operator=(const table_copy_assign& rhs) noexcept( // wtb: noexcept(auto)
-			TableTraits::all_nothrow_copy_assignable								   //
-				&& TableTraits::all_nothrow_copy_constructible						   //
-					&& noexcept(Base::clear())										   //
-						&& noexcept(Base::pop_back())								   //
-							&& noexcept(Base::reserve(size_t{})))
+			Traits::all_nothrow_copy_assignable										   //
+				&& Traits::all_nothrow_copy_constructible							   //
+					&& noexcept(base::clear())										   //
+						&& noexcept(base::pop_back())								   //
+							&& noexcept(base::reserve(size_t{})))
 		{
 			if SOAGEN_UNLIKELY(&rhs == this)
 				return *this;
 
-			if constexpr (allocator_traits::propagate_on_container_copy_assignment::value
-						  || !allocator_traits::is_always_equal::value)
+			if constexpr (allocator_traits<Allocator>::propagate_on_container_copy_assignment::value
+						  || !allocator_traits<Allocator>::is_always_equal::value)
 			{
-				if (!allocator_traits::equal(Base::allocator(), rhs.allocator()))
+				if (!allocator_traits<Allocator>::equal(base::allocator(), rhs.allocator()))
 				{
-					Base::clear();
-					Base::shink_to_fit();
-					SOAGEN_ASSERT(Base::empty());
-					SOAGEN_ASSERT(!Base::alloc_);
+					base::clear();
+					base::shink_to_fit();
+					SOAGEN_ASSERT(base::empty());
+					SOAGEN_ASSERT(!base::alloc_);
 				}
 			}
 
-			if constexpr (allocator_traits::propagate_on_container_copy_assignment::value)
+			if constexpr (allocator_traits<Allocator>::propagate_on_container_copy_assignment::value)
 			{
 				static_assert(std::is_nothrow_copy_assignable_v<Allocator>,
 							  "copy-propagated allocators must be nothrow copy-assignable");
 
-				Base::allocator() = rhs.allocator();
+				base::allocator() = rhs.allocator();
 			}
 
 			if (rhs.empty())
 			{
-				Base::clear();
+				base::clear();
 				return *this;
 			}
 
-			if (rhs.size() < Base::size())
-				Base::pop_back(Base::size() - rhs.size());
+			if (rhs.size() < base::size())
+				base::pop_back(base::size() - rhs.size());
 
-			Base::reserve(rhs.size());
+			base::reserve(rhs.size());
 
-			const auto assigned_end = min(Base::size(), rhs.size());
+			const auto assigned_end = min(base::size(), rhs.size());
 			for (size_t i = 0; i < assigned_end; i++)
-				TableTraits::copy_assign_row(Base::alloc_.columns, i, rhs.alloc_.columns, i);
+				Traits::copy_assign_row(base::alloc_.columns, i, rhs.alloc_.columns, i);
 
-			const auto constructed_end = max(Base::size(), rhs.size());
+			const auto constructed_end = max(base::size(), rhs.size());
 			for (size_t i = assigned_end; i < constructed_end; i++)
 			{
-				TableTraits::copy_construct_row(Base::alloc_.columns, i, rhs.alloc_.columns, i);
-				Base::count_++;
+				Traits::copy_construct_row(base::alloc_.columns, i, rhs.alloc_.columns, i);
+				base::count_++;
 			}
 
 			return *this;
 		}
 	};
 
-	template <typename TableTraits, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_copy_assign<TableTraits, Allocator, Base, false> //
-		: public Base
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_copy_assign<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_copy_assign);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: row erasure
 	//------------------------------------------------------------------------------------------------------------------
 
-	template <typename TableTraits,
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_copy_assign
+
+	template <typename Traits,
 			  typename Allocator,
-			  typename Base = table_copy_assign<TableTraits, Allocator>,
-			  bool			= TableTraits::all_move_assignable>
+			  bool = Traits::all_move_assignable>
 	class SOAGEN_EMPTY_BASES table_row_erasure //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_row_erasure);
 
-		void erase(size_t pos)								  //
-			noexcept(TableTraits::all_nothrow_move_assignable //
-						 && noexcept(Base::pop_back()))
-		{
-			SOAGEN_ASSUME(pos < Base::count_);
+		void erase(size_t pos)							 //
+			noexcept(Traits::all_nothrow_move_assignable //
+						 && noexcept(base::pop_back()))
+		{
+			SOAGEN_ASSUME(pos < base::count_);
+
+			if (pos + 1u < base::count_)
+				Traits::move_assign_rows(base::alloc_.columns,
+										 pos,
+										 base::alloc_.columns,
+										 pos + 1u,
+										 base::count_ - pos - 1u);
 
-			TableTraits::move_assign_rows(Base::alloc_.columns,
-										  pos,
-										  Base::alloc_.columns,
-										  pos + 1u,
-										  Base::count_ - pos - 1u);
-			Base::pop_back();
+			base::pop_back();
 		}
 	};
 
-	template <typename TableTraits, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_row_erasure<TableTraits, Allocator, Base, false> //
-		: public Base
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_row_erasure<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_row_erasure);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
 	// specialization: row erasure (unordered)
 	//------------------------------------------------------------------------------------------------------------------
 
-	template <typename TableTraits,
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_row_erasure
+
+	template <typename Traits,
 			  typename Allocator,
-			  typename Base = table_row_erasure<TableTraits, Allocator>,
-			  bool			= TableTraits::all_swappable>
+			  bool = Traits::all_swappable>
 	class SOAGEN_EMPTY_BASES table_row_erasure_unordered //
-		: public Base
+		: public SOAGEN_BASE_TYPE
 	{
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_row_erasure_unordered);
 
 		soagen::optional<size_t> unordered_erase(size_t pos) //
-			noexcept(TableTraits::all_nothrow_swappable		 //
-						 && noexcept(Base::pop_back()))
+			noexcept(Traits::all_nothrow_swappable			 //
+						 && noexcept(base::pop_back()))
 		{
-			SOAGEN_ASSUME(pos < Base::count_);
+			SOAGEN_ASSUME(pos < base::count_);
 
-			if (pos + 1u == Base::count_)
+			if (pos + 1u == base::count_)
 			{
-				Base::pop_back();
+				base::pop_back();
 				return {};
 			}
 
-			TableTraits::swap_rows(Base::alloc_.columns, pos, Base::alloc_.columns, Base::count_ - 1u);
-			Base::pop_back();
-			return soagen::optional<size_t>{ Base::count_ };
+			Traits::swap_rows(base::alloc_.columns, pos, base::alloc_.columns, base::count_ - 1u);
+			base::pop_back();
+			return soagen::optional<size_t>{ base::count_ };
 		}
 	};
 
-	template <typename TableTraits, typename Allocator, typename Base>
-	class SOAGEN_EMPTY_BASES table_row_erasure_unordered<TableTraits, Allocator, Base, false> //
-		: public Base
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_row_erasure_unordered<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
 	{
 	  public:
-		using Base::Base;
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 
 		SOAGEN_DEFAULT_RULE_OF_FIVE(table_row_erasure_unordered);
 	};
 
 	//------------------------------------------------------------------------------------------------------------------
-	// misc
+	// specialization: EqualityComparable
 	//------------------------------------------------------------------------------------------------------------------
 
-	// trait for determining the _actual_ alignment of a table column, taking the allocator and table-allocation
-	// semantics into account (since the full allocation for a table is always has alignment ==
-	// table_traits::largest_alignment).
-	//
-	// note that this has absolutely nothing to do with the aligned_stride; that is still calculated according to
-	// the user's specified alignment requirements. this trait is _only_ used to help the compiler via assume_aligned.
-	template <typename TableTraits, typename Allocator, size_t ColumnIndex>
-	inline constexpr size_t actual_column_alignment = TableTraits::template column<ColumnIndex>::alignment;
-
-	template <typename TableTraits, typename Allocator>
-	inline constexpr size_t actual_column_alignment<TableTraits, Allocator, 0> =
-		max(TableTraits::template column<0>::alignment,
-			allocator_traits<Allocator>::min_alignment,
-			TableTraits::largest_alignment);
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_row_erasure_unordered
+
+	template <typename Traits,
+			  typename Allocator,
+			  bool = Traits::all_equality_comparable>
+	class SOAGEN_EMPTY_BASES table_equality_compare //
+		: public SOAGEN_BASE_TYPE
+	{
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_equality_compare);
+
+		SOAGEN_NODISCARD
+		friend constexpr bool operator==(const table_equality_compare& lhs,
+										 const table_equality_compare& rhs) //
+			noexcept(Traits::all_nothrow_equality_comparable)
+		{
+			if (&lhs == &rhs || (lhs.empty() && rhs.empty()))
+				return true;
+
+			if (lhs.size() != rhs.size())
+				return false;
+
+			return Traits::equal(lhs.alloc_.columns, {}, rhs.alloc_.columns, {}, lhs.size());
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator!=(const table_equality_compare& lhs,
+										 const table_equality_compare& rhs) //
+			noexcept(Traits::all_nothrow_equality_comparable)
+		{
+			return !(lhs == rhs);
+		}
+	};
+
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_equality_compare<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
+	{
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_equality_compare);
+	};
+
+	//------------------------------------------------------------------------------------------------------------------
+	// specialization: LessThanComparable
+	//------------------------------------------------------------------------------------------------------------------
+
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_equality_compare
+
+	template <typename Traits,
+			  typename Allocator,
+			  bool = Traits::all_less_than_comparable>
+	class SOAGEN_EMPTY_BASES table_less_than_compare //
+		: public SOAGEN_BASE_TYPE
+	{
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_less_than_compare);
+
+		SOAGEN_NODISCARD
+		constexpr int compare(const table_less_than_compare& rhs) const //
+			noexcept(Traits::all_nothrow_equality_comparable)
+		{
+			if (&rhs == this)
+				return 0;
+			if (base::empty())
+				return rhs.empty() ? 0 : -1;
+			if (rhs.empty())
+				return 1;
+
+			const auto comp = Traits::compare(base::alloc_.columns, //
+											  {},
+											  rhs.alloc_.columns,
+											  {},
+											  min(base::size(), rhs.size()));
+
+			return comp != 0 ? comp : (base::size() == rhs.size() ? 0 : (base::size() < rhs.size() ? -1 : 1));
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator<(const table_less_than_compare& lhs,
+										const table_less_than_compare& rhs) //
+			noexcept(Traits::all_nothrow_equality_comparable)
+		{
+			return lhs.compare(rhs) < 0;
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator<=(const table_less_than_compare& lhs,
+										 const table_less_than_compare& rhs) //
+			noexcept(Traits::all_nothrow_equality_comparable)
+		{
+			return lhs.compare(rhs) <= 0;
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator>(const table_less_than_compare& lhs,
+										const table_less_than_compare& rhs) //
+			noexcept(Traits::all_nothrow_equality_comparable)
+		{
+			return lhs.compare(rhs) > 0;
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator>=(const table_less_than_compare& lhs,
+										 const table_less_than_compare& rhs) //
+			noexcept(Traits::all_nothrow_equality_comparable)
+		{
+			return lhs.compare(rhs) >= 0;
+		}
+	};
+
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_less_than_compare<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
+	{
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_less_than_compare);
+	};
+
+	//------------------------------------------------------------------------------------------------------------------
+	// specialization: data()
+	//------------------------------------------------------------------------------------------------------------------
+
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_less_than_compare
+
+	template <typename Traits,
+			  typename Allocator,
+			  bool = Traits::all_trivially_copyable>
+	class SOAGEN_EMPTY_BASES table_data_ptr //
+		: public SOAGEN_BASE_TYPE
+	{
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_data_ptr);
+
+		using table_traits	 = Traits;
+		using allocator_type = Allocator;
+
+		SOAGEN_ALIGNED_COLUMN(0)
+		constexpr std::byte* data() noexcept
+		{
+			return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, 0>>(
+				base::alloc_.columns[0]);
+		}
+
+		SOAGEN_ALIGNED_COLUMN(0)
+		constexpr const std::byte* data() const noexcept
+		{
+			return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, 0>>(
+				base::alloc_.columns[0]);
+		}
+	};
+
+	template <typename Traits, typename Allocator>
+	class SOAGEN_EMPTY_BASES table_data_ptr<Traits, Allocator, false> //
+		: public SOAGEN_BASE_TYPE
+	{
+	  public:
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+
+		SOAGEN_DEFAULT_RULE_OF_FIVE(table_data_ptr);
+	};
 }
 
+#undef SOAGEN_BASE_NAME
+#define SOAGEN_BASE_NAME table_data_ptr
+#undef SOAGEN_BASE_TYPE
+#define SOAGEN_BASE_TYPE detail::SOAGEN_BASE_NAME<Traits, Allocator>
+
 namespace soagen
 {
-	template <typename TableTraits,
-			  typename Allocator = allocator,
-			  typename Base		 = detail::table_row_erasure_unordered<TableTraits, Allocator>>
+	template <typename Traits,
+			  typename Allocator = soagen::allocator>
 	class SOAGEN_EMPTY_BASES table //
-		: public Base
+		SOAGEN_HIDDEN_BASE(public SOAGEN_BASE_TYPE)
 	{
-		static_assert(is_table_traits<TableTraits>, "TableTraits must be an instance of soagen::table_traits");
-		static_assert(!is_cvref<TableTraits>, "table traits may not be cvref-qualified");
+		static_assert(is_table_traits<Traits>, "Traits must be an instance of soagen::table_traits");
+		static_assert(!is_cvref<Traits>, "table traits may not be cvref-qualified");
 		static_assert(!is_cvref<Allocator>, "allocators may not be cvref-qualified");
 
+	  private:
+		using base = SOAGEN_BASE_TYPE;
+
 	  public:
-		using size_type		   = size_t;
-		using difference_type  = ptrdiff_t;
-		using allocator_type   = Allocator;
-		using allocator_traits = allocator_traits<Allocator>;
-		using table_traits	   = TableTraits;
+		using size_type		  = size_t;
+		using difference_type = ptrdiff_t;
 
-		template <size_type I>
-		using column_traits = typename table_traits::template column<I>;
+		using table_traits = Traits;
 
-		template <size_type I>
-		using column_type = typename column_traits<I>::value_type;
+		using allocator_type = Allocator;
 
-		using Base::Base;
+		template <size_type Column>
+		using column_traits = typename table_traits::template column<Column>;
 
-		SOAGEN_DEFAULT_RULE_OF_FIVE(table);
+		template <size_type Column>
+		using column_type = typename column_traits<Column>::value_type;
 
-		template <size_t I>
-		SOAGEN_ALIGNED_COLUMN(I)
-		column_type<I>* column() noexcept
+		static constexpr size_t aligned_stride = Traits::aligned_stride;
+
+		SOAGEN_NODISCARD_CTOR
+		table() = default;
+
+		SOAGEN_NODISCARD_CTOR
+		table(table&&) = default;
+
+		table& operator=(table&&) = default;
+
+		SOAGEN_NODISCARD_CTOR
+		table(const table&) = default;
+
+		table& operator=(const table&) = default;
+
+		~table() = default;
+
+#if !SOAGEN_DOXYGEN
+		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
+#endif
+
+#if SOAGEN_DOXYGEN
+
+		constexpr std::byte* data() noexcept;
+
+		constexpr const std::byte* data() const noexcept;
+
+#endif
+
+		template <size_t Column>
+		SOAGEN_ALIGNED_COLUMN(Column)
+		column_type<Column>* column() noexcept
 		{
-			static_assert(I < table_traits::column_count, "column index out of range");
+			static_assert(Column < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, I>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<I>*>(Base::alloc_.columns[I])));
+			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, Column>>(
+				SOAGEN_LAUNDER(reinterpret_cast<column_type<Column>*>(base::alloc_.columns[Column])));
 		}
 
-		template <size_t I>
-		SOAGEN_ALIGNED_COLUMN(I)
-		std::add_const_t<column_type<I>>* column() const noexcept
+		template <size_t Column>
+		SOAGEN_ALIGNED_COLUMN(Column)
+		std::add_const_t<column_type<Column>>* column() const noexcept
 		{
-			static_assert(I < table_traits::column_count, "column index out of range");
+			static_assert(Column < table_traits::column_count, "column index out of range");
 
-			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, I>>(
-				SOAGEN_LAUNDER(reinterpret_cast<column_type<I>*>(Base::alloc_.columns[I])));
+			return soagen::assume_aligned<detail::actual_column_alignment<table_traits, allocator_type, Column>>(
+				SOAGEN_LAUNDER(reinterpret_cast<column_type<Column>*>(base::alloc_.columns[Column])));
 		}
 	};
 
 	template <typename>
-	inline constexpr bool is_table = false;
-
+	inline constexpr bool is_table = POXY_IMPLEMENTATION_DETAIL(false);
 	template <typename... Args>
 	inline constexpr bool is_table<table<Args...>> = true;
-
-	template <typename... Args>
-	inline constexpr bool is_soa<table<Args...>> = true;
-
-	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Traits, Alloc>>), typename Traits, typename Alloc)
+	template <typename T>
+	inline constexpr bool is_table<const T> = is_table<T>;
+	template <typename T>
+	inline constexpr bool is_table<volatile T> = is_table<T>;
+	template <typename T>
+	inline constexpr bool is_table<const volatile T> = is_table<T>;
+	namespace detail
+	{
+		template <typename... Args>
+		struct table_type_<table<Args...>>
+		{
+			using type = table<Args...>;
+		};
+	}
+	SOAGEN_CONSTRAINED_TEMPLATE((has_swap_member<table<Traits, Allocator>>), typename Traits, typename Allocator)
 	SOAGEN_ALWAYS_INLINE
-	constexpr void swap(table<Traits, Alloc>& lhs, table<Traits, Alloc>& rhs) //
-		noexcept(noexcept(std::declval<table<Traits, Alloc>&>().swap(std::declval<table<Traits, Alloc>&>())))
+	constexpr void swap(table<Traits, Allocator>& lhs, table<Traits, Allocator>& rhs) //
+		noexcept(soagen::has_nothrow_swap_member<table<Traits, Allocator>>)
 	{
 		lhs.swap(rhs);
 	}
 }
 
+#undef SOAGEN_BASE_NAME
+#undef SOAGEN_BASE_TYPE
+
+#if SOAGEN_ALWAYS_OPTIMIZE
+	#if SOAGEN_MSVC
+		#pragma strict_gs_check(pop)
+		#pragma runtime_checks("", restore)
+		#pragma optimize("", on)
+		#pragma inline_recursion(off)
+	#elif SOAGEN_GCC
+		#pragma GCC pop_options
+	#endif
+#endif
+
+#if SOAGEN_MSVC_LIKE
+	#pragma pop_macro("min")
+	#pragma pop_macro("max")
+#endif
+
+SOAGEN_POP_WARNINGS;
+
+//********  mixins.hpp  ************************************************************************************************
+
+namespace soagen::mixins
+{
+	//--- resize() -----------------------------------------------------------------------------------------------------
+
+	template <typename Derived, bool = has_resize_member<table_type<Derived>, typename table_type<Derived>::size_type>>
+	struct SOAGEN_EMPTY_BASES resizable
+	{
+		using table_type = soagen::table_type<Derived>;
+		using size_type	 = typename table_type::size_type;
+
+		SOAGEN_ALWAYS_INLINE
+		SOAGEN_CPP20_CONSTEXPR
+		Derived& resize(size_type new_size) //
+			noexcept(soagen::has_nothrow_resize_member<table_type, size_type>)
+		{
+			static_cast<Derived&>(*this).table().resize(new_size);
+			return static_cast<Derived&>(*this);
+		}
+	};
+
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES resizable<Derived, false>
+	{};
+
+	//--- swap() -------------------------------------------------------------------------------------------------------
+
+	template <typename Derived, bool = has_swap_member<table_type<Derived>>>
+	struct SOAGEN_EMPTY_BASES swappable
+	{
+		using table_type = soagen::table_type<Derived>;
+
+		SOAGEN_ALWAYS_INLINE
+		SOAGEN_CPP20_CONSTEXPR
+		void swap(Derived& other) //
+			noexcept(soagen::has_nothrow_swap_member<table_type>)
+		{
+			return static_cast<Derived&>(*this).table().swap(other.table());
+		}
+	};
+
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES swappable<Derived, false>
+	{};
+
+	//--- equality-comparable-------------------------------------------------------------------------------------------
+
+	template <typename Derived, bool = is_equality_comparable<const table_type<Derived>>>
+	struct SOAGEN_EMPTY_BASES equality_comparable
+	{
+		using table_type = soagen::table_type<Derived>;
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator==(const Derived& lhs, const Derived& rhs) //
+			noexcept(soagen::is_nothrow_equality_comparable<table_type>)
+		{
+			return lhs.table() == rhs.table();
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator!=(const Derived& lhs, const Derived& rhs) //
+			noexcept(soagen::is_nothrow_equality_comparable<table_type>)
+		{
+			return lhs.table() != rhs.table();
+		}
+	};
+
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES equality_comparable<Derived, false>
+	{};
+
+	//--- less-than-comparable-------------------------------------------------------------------------------------------
+
+	template <typename Derived, bool = is_less_than_comparable<const table_type<Derived>>>
+	struct SOAGEN_EMPTY_BASES less_than_comparable
+	{
+		using table_type = soagen::table_type<Derived>;
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator<(const Derived& lhs, const Derived& rhs) //
+			noexcept(soagen::is_nothrow_less_than_comparable<table_type>)
+		{
+			return lhs.table() < rhs.table();
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator<=(const Derived& lhs, const Derived& rhs) //
+			noexcept(soagen::is_nothrow_less_than_comparable<table_type>)
+		{
+			return lhs.table() <= rhs.table();
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator>(const Derived& lhs, const Derived& rhs) //
+			noexcept(soagen::is_nothrow_less_than_comparable<table_type>)
+		{
+			return lhs.table() > rhs.table();
+		}
+
+		SOAGEN_NODISCARD
+		SOAGEN_ALWAYS_INLINE
+		friend constexpr bool operator>=(const Derived& lhs, const Derived& rhs) //
+			noexcept(soagen::is_nothrow_less_than_comparable<table_type>)
+		{
+			return lhs.table() >= rhs.table();
+		}
+	};
+
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES less_than_comparable<Derived, false>
+	{};
+
+	//--- data() -------------------------------------------------------------------------------------------------------
+
+	template <typename Derived, bool = has_data_member<table_type<Derived>>>
+	struct SOAGEN_EMPTY_BASES data_ptr
+	{
+		using table_type	 = soagen::table_type<Derived>;
+		using table_traits	 = soagen::table_traits_type<Derived>;
+		using allocator_type = soagen::allocator_type<Derived>;
+
+		SOAGEN_ALIGNED_COLUMN(0)
+		constexpr std::byte* data() //
+			noexcept(soagen::has_nothrow_data_member<table_type>)
+		{
+			return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, 0>>(
+				static_cast<Derived&>(*this).table().data());
+		}
+	};
+
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES data_ptr<Derived, false>
+	{};
+
+	//--- data() (const) -----------------------------------------------------------------------------------------------
+
+	template <typename Derived, bool = has_data_member<const table_type<Derived>>>
+	struct SOAGEN_EMPTY_BASES const_data_ptr
+	{
+		using table_type	 = soagen::table_type<Derived>;
+		using table_traits	 = soagen::table_traits_type<Derived>;
+		using allocator_type = soagen::allocator_type<Derived>;
+
+		SOAGEN_ALIGNED_COLUMN(0)
+		constexpr const std::byte* data() const //
+			noexcept(soagen::has_nothrow_data_member<const table_type>)
+		{
+			return soagen::assume_aligned<soagen::detail::actual_column_alignment<table_traits, allocator_type, 0>>(
+				static_cast<const Derived&>(*this).table().data());
+		}
+	};
+
+	template <typename Derived>
+	struct SOAGEN_EMPTY_BASES const_data_ptr<Derived, false>
+	{};
+}
+
+//********  iterator.hpp  **********************************************************************************************
+
+SOAGEN_DISABLE_WARNINGS;
+#include <iterator>
+SOAGEN_ENABLE_WARNINGS;
+
+SOAGEN_PUSH_WARNINGS;
+SOAGEN_DISABLE_SPAM_WARNINGS;
+
+#if SOAGEN_MSVC_LIKE
+	#pragma push_macro("min")
+	#pragma push_macro("max")
+	#undef min
+	#undef max
+#endif
+
+#if SOAGEN_ALWAYS_OPTIMIZE
+	#if SOAGEN_MSVC
+		#pragma inline_recursion(on)
+		#pragma optimize("gt", on)
+		#pragma runtime_checks("", off)
+		#pragma strict_gs_check(push, off)
+	#elif SOAGEN_GCC
+		#pragma GCC push_options
+		#pragma GCC optimize("O2")
+	#endif
+#endif
+
+namespace soagen
+{
+	template <typename, size_t...>
+	class iterator;
+
+	namespace detail
+	{
+		// iterator implicit conversions are allowed when:
+		// - changing columns
+		// - losing rvalue (Table&& -> Table&), (const Table&& -> const Table&)
+		// - gaining const (Table& -> const Table&, Table&& -> const Table&&)
+		// - any combination of the three
+
+		template <typename From, typename To>
+		inline constexpr bool iterator_implicit_conversion_ok = false;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table, ColumnsA...>, //
+															  iterator<Table, ColumnsB...>> = true;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
+															  iterator<Table&, ColumnsB...>> = true;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_implicit_conversion_ok<iterator<const Table&&, ColumnsA...>, //
+															  iterator<const Table&, ColumnsB...>> = true;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&, ColumnsA...>, //
+															  iterator<const Table&, ColumnsB...>> = true;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
+															  iterator<const Table&&, ColumnsB...>> = true;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_implicit_conversion_ok<iterator<Table&&, ColumnsA...>, //
+															  iterator<const Table&, ColumnsB...>> = true;
+
+		// iterator explicit conversions are allowed when gaining rvalue and optionally gaining const
+		// (note that we specifically avoid providing anything that would be the moral equivalent of
+		// a const_cast because that armory is filled with very large and powerful footguns)
+
+		template <typename From, typename To>
+		inline constexpr bool iterator_explicit_conversion_ok = false;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_explicit_conversion_ok<iterator<Table&, ColumnsA...>, //
+															  iterator<Table&&, ColumnsB...>> = true;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_explicit_conversion_ok<iterator<const Table&, ColumnsA...>, //
+															  iterator<const Table&&, ColumnsB...>> = true;
+
+		template <typename Table, size_t... ColumnsA, size_t... ColumnsB>
+		inline constexpr bool iterator_explicit_conversion_ok<iterator<Table&, ColumnsA...>, //
+															  iterator<const Table&&, ColumnsB...>> = true;
+
+		template <typename T>
+		struct arrow_proxy
+		{
+			mutable T value;
+
+			SOAGEN_PURE_INLINE_GETTER
+			constexpr T* operator->() const noexcept
+			{
+				return &value;
+			}
+		};
+
+		template <typename Table>
+		struct iterator_storage
+		{
+			std::add_const_t<remove_cvref<Table>>* table;
+			typename remove_cvref<Table>::difference_type offset;
+		};
+	}
+	template <typename Table, size_t... Columns>
+	class iterator SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>)
+	{
+	  public:
+		using table_type = remove_cvref<Table>;
+		static_assert(is_soa<table_type>, "soagen iterators are for use with soagen-generated SoA table types.");
+
+		using table_ref = Table;
+		static_assert(std::is_reference_v<table_ref>,
+					  "Table must be a reference so row members can derive their reference category");
+
+		using size_type = typename table_type::size_type;
+
+		using difference_type = typename table_type::difference_type;
+
+		using row_type = row<Table, Columns...>;
+
+		using value_type = row_type;
+
+		using reference = row_type;
+
+		using iterator_category = std::random_access_iterator_tag;
+
+#if SOAGEN_CPP == 17
+		using pointer = void;
+#endif
+
+	  private:
+		using base		= detail::iterator_storage<remove_cvref<Table>>;
+		using table_ptr = std::add_pointer_t<std::remove_reference_t<Table>>;
+
+		template <typename, size_t...>
+		friend class soagen::iterator;
+
+		SOAGEN_NODISCARD_CTOR
+		constexpr iterator(base b) noexcept //
+			: base{ b }
+		{}
+
+	  public:
+		SOAGEN_NODISCARD_CTOR
+		constexpr iterator() noexcept = default;
+
+		SOAGEN_NODISCARD_CTOR
+		constexpr iterator(table_ref tbl, difference_type pos) noexcept //
+			: base{ &tbl, pos }
+		{}
+
+		friend constexpr iterator& operator++(iterator& it) noexcept // pre
+		{
+			++it.offset;
+			return it;
+		}
+
+		friend constexpr iterator operator++(iterator& it, int) noexcept // post
+		{
+			iterator pre = it;
+			++it.offset;
+			return pre;
+		}
+
+		friend constexpr iterator& operator+=(iterator& it, difference_type n) noexcept
+		{
+			it.offset += n;
+			return it;
+		}
+
+		SOAGEN_PURE_GETTER
+		friend constexpr iterator operator+(const iterator& it, difference_type n) noexcept
+		{
+			auto it2 = it;
+			it2 += n;
+			return it2;
+		}
+
+		friend constexpr iterator& operator--(iterator& it) noexcept // pre
+		{
+			--it.offset;
+			return it;
+		}
+
+		friend constexpr iterator operator--(iterator& it, int) noexcept // post
+		{
+			iterator pre = it;
+			--it.offset;
+			return pre;
+		}
+
+		friend constexpr iterator& operator-=(iterator& it, difference_type n) noexcept
+		{
+			return it += (-n);
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		friend constexpr iterator operator-(const iterator& it, difference_type n) noexcept
+		{
+			return it + (-n);
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_GETTER
+		constexpr difference_type operator-(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset - rhs.offset;
+		}
+
+		SOAGEN_PURE_GETTER
+		constexpr reference operator*() const noexcept
+		{
+			SOAGEN_ASSUME(!!base::table);
+			SOAGEN_ASSUME(base::offset >= 0);
+
+			return static_cast<table_ref>(*const_cast<table_ptr>(base::table))
+				.template row<Columns...>(static_cast<size_type>(base::offset));
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr detail::arrow_proxy<row_type> operator->() const noexcept
+		{
+			return { *(*this) };
+		}
+
+		SOAGEN_PURE_GETTER
+		constexpr reference operator[](difference_type offset) const noexcept
+		{
+			SOAGEN_ASSUME(!!base::table);
+			SOAGEN_ASSUME(base::offset + offset >= 0);
+
+			return static_cast<table_ref>(*const_cast<table_ptr>(base::table))
+				.template row<Columns...>(static_cast<size_type>(base::offset + offset));
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_GETTER
+		constexpr bool operator==(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::table == rhs.table && base::offset == rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		friend constexpr bool operator!=(const iterator& lhs, const iterator<T, Cols...>& rhs) noexcept
+		{
+			return !(lhs == rhs);
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator<(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset < rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator<=(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset <= rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator>(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset > rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>), typename T, size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr bool operator>=(const iterator<T, Cols...>& rhs) const noexcept
+		{
+			return base::offset >= rhs.offset;
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((detail::iterator_implicit_conversion_ok<iterator, iterator<T, Cols...>>
+									 && !detail::iterator_explicit_conversion_ok<iterator, iterator<T, Cols...>>),
+									typename T,
+									size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		constexpr operator iterator<T, Cols...>() const noexcept
+		{
+			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
+		}
+
+		SOAGEN_CONSTRAINED_TEMPLATE((!detail::iterator_implicit_conversion_ok<iterator, iterator<T, Cols...>>
+									 && detail::iterator_explicit_conversion_ok<iterator, iterator<T, Cols...>>),
+									typename T,
+									size_t... Cols)
+		SOAGEN_PURE_INLINE_GETTER
+		explicit constexpr operator iterator<T, Cols...>() const noexcept
+		{
+			return iterator<T, Cols...>{ static_cast<const base&>(*this) };
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		explicit constexpr operator difference_type() const noexcept
+		{
+			return base::offset;
+		}
+
+		SOAGEN_PURE_INLINE_GETTER
+		explicit constexpr operator size_type() const noexcept
+		{
+			SOAGEN_ASSUME(base::offset >= 0);
+
+			return static_cast<size_type>(base::offset);
+		}
+	};
+
+	template <typename Table, size_t... Columns>
+	SOAGEN_PURE_INLINE_GETTER
+	constexpr iterator<Table, Columns...> operator+(typename iterator<Table, Columns...>::difference_type n,
+													const iterator<Table, Columns...>& it) noexcept
+	{
+		return it + n;
+	}
+
+	template <typename T>
+	inline constexpr bool is_iterator = POXY_IMPLEMENTATION_DETAIL(false);
+	template <typename Table, size_t... Columns>
+	inline constexpr bool is_iterator<iterator<Table, Columns...>> = true;
+	template <typename T>
+	inline constexpr bool is_iterator<const T> = is_row<T>;
+	template <typename T>
+	inline constexpr bool is_iterator<volatile T> = is_row<T>;
+	template <typename T>
+	inline constexpr bool is_iterator<const volatile T> = is_row<T>;
+	namespace detail
+	{
+		template <typename Table, size_t... Columns>
+		struct table_type_<iterator<Table, Columns...>>
+		{
+			using type = remove_cvref<Table>;
+		};
+		template <typename Table, size_t... Columns>
+		struct table_traits_type_<iterator<Table, Columns...>>
+		{
+			using type = table_traits_type<remove_cvref<Table>>;
+		};
+
+		template <typename Table, typename IndexSequence>
+		struct iterator_type_;
+		template <typename Table, size_t... Columns>
+		struct iterator_type_<Table, std::index_sequence<Columns...>>
+		{
+			using type = iterator<Table, Columns...>;
+		};
+		template <typename Table>
+		struct iterator_type_<Table, std::index_sequence<>>
+			: iterator_type_<Table, std::make_index_sequence<table_traits_type<remove_cvref<Table>>::column_count>>
+		{};
+	}
+	template <typename Table, size_t... Columns>
+	using iterator_type = POXY_IMPLEMENTATION_DETAIL(
+		typename detail::iterator_type_<coerce_ref<Table>, std::index_sequence<Columns...>>::type);
+}
+
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
 		#pragma inline_recursion(off)
 	#elif SOAGEN_GCC
```

### Comparing `soagen-0.0.1/src/soagen/paths.py` & `soagen-0.1.0/src/soagen/paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,35 +10,51 @@
 
 import tempfile
 from pathlib import Path
 
 PACKAGE = Path(Path(__file__).resolve().parent)
 """The root directory of the package installation."""
 
-HPP = Path(PACKAGE, r'hpp')
-"""The PACKAGE containing soagen's (non-autogenerated) hpp files."""
-
-HPP_TEMPLATES = Path(HPP, r'templates')
-"""The directory containing soagen's .hpp template files"""
-
 SRC = Path(PACKAGE, r'..').resolve()
 """The root directory of repository's package sources."""
 
 REPOSITORY = Path(SRC, r'..').resolve()
 """The root directory of the repository."""
 
 TESTS = Path(REPOSITORY, r'tests')
 """The root directory of the repository's tests."""
 
+HPP = Path(PACKAGE, r'hpp')
+"""The PACKAGE containing soagen's (non-autogenerated) hpp files."""
+
+HPP_TEMPLATES = Path(HPP, r'templates')
+"""The directory containing soagen's .hpp template files"""
+
+HPP_GENERATED = Path(HPP, r'generated')
+"""The directory containing soagen's procedurally-generated .hpp files"""
+
+HPP_SINGLE = Path(HPP, r'single')
+"""The directory containing soagen's pre-processed 'single' soagen.hpp"""
+
+DOCS = Path(REPOSITORY, r'docs')
+"""The root directory of the repository's documentation."""
+
+EXAMPLES = Path(REPOSITORY, r'examples')
+"""The root directory of the repository's examples."""
+
 TEMP = Path(tempfile.gettempdir(), r'soagen')
 """A global temp directory shared by all instances of soagen."""
 
 BUG_REPORT_DIR = (TEMP / r'bug_report').resolve()
 """Directory used for assembling bug reports."""
 
 BUG_REPORT_INPUTS = BUG_REPORT_DIR / r'inputs'
 """Directory used for storing the inputs when assembling bug reports."""
 
 BUG_REPORT_OUTPUTS = BUG_REPORT_DIR / r'outputs'
 """Directory used for storing the outputs when assembling bug reports."""
 
+VERSION_TXT = PACKAGE / r'version.txt'
+"""The version file, version.txt."""
+
+
 MAKE_SINGLE = Path(REPOSITORY, r'..', r'muu', r'tools', r'make_single.py')
```

### Comparing `soagen-0.0.1/src/soagen/utils.py` & `soagen-0.1.0/src/soagen/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,85 +7,93 @@
 """
 Misc utility functions.
 """
 
 import re
 import shutil
 import subprocess
+import textwrap
 from pathlib import Path
 
 from misk import *
 
 from . import paths
 
 
 def to_snake_case(s: str) -> str:
-	s = str(s)
-	s = s.strip()
-	s = re.sub('\s+', '_', s)
-	s = re.sub('__+', '_', s)
-	s = re.sub('([a-z])([A-Z])', lambda m: m[1] + '_' + m[2].lower(), s)
-	s = s.lower()
-	return s
-
+    s = str(s)
+    s = s.strip()
+    s = re.sub('\s+', '_', s)
+    s = re.sub('__+', '_', s)
+    s = re.sub('([a-z])([A-Z])', lambda m: m[1] + '_' + m[2].lower(), s)
+    s = s.lower()
+    return s
 
 
 def to_pascal_case(s: str) -> str:
-	s = to_snake_case(s)
-	s = re.sub('_([a-z])', lambda m: m[1].upper(), s)
-	s = s.strip('_')
-	if len(s):
-		s = s[:1].upper() + s[1:]
-	return s
-
+    s = to_snake_case(s)
+    s = re.sub('_([a-z])', lambda m: m[1].upper(), s)
+    s = s.strip('_')
+    if len(s):
+        s = s[:1].upper() + s[1:]
+    return s
 
 
 def clang_format(s, cwd=None):
-	cwd = Path.cwd() if cwd is None else cwd
-	# respect the user's .clang-format file if one exists, but
-	# fallback to the internal one (so there's always a sane default)
-	style_dir = cwd
-	style_file = None
-	while True:
-		file = Path(style_dir, r'.clang-format')
-		if file.is_file():
-			style_file = file
-			break
-		dir = style_dir.parent
-		if not dir or dir == style_dir or not dir.is_dir():
-			break
-		style_dir = dir
-	if style_file is None:
-		style_file = Path(paths.HPP, r'.clang-format')
-		assert style_file.is_file()
-
-	result = subprocess.run([r'clang-format', rf'--style=file:{style_file}'],
-		capture_output=True,
-		cwd=str(cwd),
-		encoding='utf-8',
-		check=True,
-		input=s)
-	return str(result.stdout)
-
+    cwd = Path.cwd() if cwd is None else cwd
+    # respect the user's .clang-format file if one exists, but
+    # fallback to the internal one (so there's always a sane default)
+    style_dir = cwd
+    style_file = None
+    while True:
+        file = Path(style_dir, r'.clang-format')
+        if file.is_file():
+            style_file = file
+            break
+        dir = style_dir.parent
+        if not dir or dir == style_dir or not dir.is_dir():
+            break
+        style_dir = dir
+    if style_file is None:
+        style_file = Path(paths.HPP, r'.clang-format')
+        assert style_file.is_file()
+
+    result = subprocess.run(
+        [r'clang-format', rf'--style=file:{style_file}'],
+        capture_output=True,
+        cwd=str(cwd),
+        encoding='utf-8',
+        check=True,
+        input=s,
+    )
+    return str(result.stdout)
 
 
 def is_tool(name):
-	return shutil.which(name) is not None
-
+    return shutil.which(name) is not None
 
 
 def repeat_pattern(pattern: str, count: int) -> str:
-	if len(pattern) == 1:
-		return pattern * count
-	text = ''
-	for i in range(0, count):
-		text = text + pattern[i % len(pattern)]
-	return text
-
+    if len(pattern) == 1:
+        return pattern * count
+    text = ''
+    for i in range(0, count):
+        text = text + pattern[i % len(pattern)]
+    return text
 
 
 def make_divider(text: str, text_col=40, pattern='-', line_length=120) -> str:
-	text = "//{}  {}  ".format(repeat_pattern(pattern, text_col - 2), text)
-	if (len(text) < line_length):
-		return text + repeat_pattern(pattern, line_length - len(text))
-	else:
-		return text
+    text = "//{}  {}  ".format(repeat_pattern(pattern, text_col - 2), text)
+    if len(text) < line_length:
+        return text + repeat_pattern(pattern, line_length - len(text))
+    else:
+        return text
+
+
+def reflow_text(text: str, line_length=120, tab_size=4) -> str:
+    text = text.replace('\n\n', '\b')
+    text = text.replace('\n', ' ')
+    text = text.replace('\b', '\n')
+    text = text.split('\n')
+    for i in range(len(text)):
+        text[i] = '\n'.join(textwrap.wrap(text[i], width=int(line_length), tabsize=int(tab_size)))
+    return '\n\n'.join(text)
```

### Comparing `soagen-0.0.1/src/soagen/version.py` & `soagen-0.1.0/src/soagen/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 # This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 # Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 # See https://github.com/marzer/soagen/blob/master/LICENSE.txt for the full license text.
 # SPDX-License-Identifier: MIT
 
 from pathlib import Path
+from . import paths
 
 VERSION = ()
 
-with open(Path(__file__).parent / r'version.txt', encoding='utf-8') as file:
-	VERSION = tuple([int(v.strip()) for v in file.read().strip().split('.')])
-	assert len(VERSION) == 3
+with open(paths.VERSION_TXT, encoding='utf-8') as file:
+    VERSION = tuple([int(v.strip()) for v in file.read().strip().split('.')])
+    assert len(VERSION) == 3
 
 VERSION_STRING = r'.'.join([str(v) for v in VERSION])
 
+__all__ = [r'VERSION', r'VERSION_STRING']
```

### Comparing `soagen-0.0.1/src/soagen.egg-info/SOURCES.txt` & `soagen-0.1.0/src/soagen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 README.md
 pyproject.toml
 src/soagen/version.txt
 src/soagen/__init__.py
 src/soagen/column.py
 src/soagen/config.py
 src/soagen/configurable.py
+src/soagen/cpp.py
 src/soagen/errors.py
 src/soagen/header_file.py
-src/soagen/includes.py
 src/soagen/injectors.py
 src/soagen/log.py
 src/soagen/main.py
-src/soagen/meson.build
 src/soagen/metavars.py
 src/soagen/natvis_file.py
 src/soagen/paths.py
 src/soagen/preprocessor.py
 src/soagen/schemas.py
 src/soagen/struct.py
 src/soagen/type_list.py
@@ -32,19 +31,22 @@
 src/soagen.egg-info/entry_points.txt
 src/soagen.egg-info/requires.txt
 src/soagen.egg-info/top_level.txt
 src/soagen.egg-info/zip-safe
 src/soagen/hpp/.clang-format
 src/soagen/hpp/allocator.hpp
 src/soagen/hpp/column_traits.hpp
-src/soagen/hpp/compressed_pair.hpp
-src/soagen/hpp/core.hpp
-src/soagen/hpp/functions.hpp
 src/soagen/hpp/header_end.hpp
 src/soagen/hpp/header_start.hpp
-src/soagen/hpp/meson.build
+src/soagen/hpp/iterator.hpp
 src/soagen/hpp/meta.hpp
-src/soagen/hpp/preprocessor.hpp
+src/soagen/hpp/mixins.hpp
+src/soagen/hpp/row.hpp
 src/soagen/hpp/soagen.hpp
 src/soagen/hpp/table.hpp
 src/soagen/hpp/table_traits.hpp
-src/soagen/hpp/version.hpp
+src/soagen/hpp/generated/compressed_pair.hpp
+src/soagen/hpp/generated/core.hpp
+src/soagen/hpp/generated/functions.hpp
+src/soagen/hpp/generated/preprocessor.hpp
+src/soagen/hpp/generated/version.hpp
+src/soagen/hpp/single/soagen.hpp
```

