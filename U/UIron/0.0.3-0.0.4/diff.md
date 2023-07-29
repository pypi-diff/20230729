# Comparing `tmp/UIron-0.0.3.tar.gz` & `tmp/UIron-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UIron-0.0.3.tar", last modified: Thu Jul 27 16:58:54 2023, max compression
+gzip compressed data, was "UIron-0.0.4.tar", last modified: Sat Jul 29 04:05:05 2023, max compression
```

## Comparing `UIron-0.0.3.tar` & `UIron-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.892322 UIron-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-07-27 02:09:14.000000 UIron-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      460 2023-07-27 16:58:54.892322 UIron-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.856345 UIron-0.0.3/UIron/
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.3/UIron/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.3/UIron/__main__.py
--rw-rw-rw-   0        0        0     1269 2023-07-27 16:14:37.000000 UIron-0.0.3/UIron/config.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.892322 UIron-0.0.3/UIron/data/
--rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.3/UIron/data/config.json
--rw-rw-rw-   0        0        0     1897 2023-07-27 16:50:20.000000 UIron-0.0.3/UIron/gui.py
--rw-rw-rw-   0        0        0      958 2023-07-27 16:49:06.000000 UIron-0.0.3/UIron/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.882187 UIron-0.0.3/UIron.egg-info/
--rw-rw-rw-   0        0        0      460 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 16:58:54.892322 UIron-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-07-27 16:58:53.000000 UIron-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.849826 UIron-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 19:37:41.000000 UIron-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      460 2023-07-29 04:05:05.848830 UIron-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.772818 UIron-0.0.4/UIron/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.4/UIron/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.4/UIron/__main__.py
+-rw-rw-rw-   0        0        0     1600 2023-07-28 05:16:34.000000 UIron-0.0.4/UIron/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.844826 UIron-0.0.4/UIron/data/
+-rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.4/UIron/data/config.json
+-rw-rw-rw-   0        0        0        2 2023-07-28 05:20:04.000000 UIron-0.0.4/UIron/data/new.json
+-rw-rw-rw-   0        0        0      121 2023-07-28 05:22:37.000000 UIron-0.0.4/UIron/regex.py
+-rw-rw-rw-   0        0        0     9412 2023-07-29 03:48:19.000000 UIron-0.0.4/UIron/ui.py
+-rw-rw-rw-   0        0        0     2234 2023-07-29 03:02:18.000000 UIron-0.0.4/UIron/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.830824 UIron-0.0.4/UIron.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:05:05.849826 UIron-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-07-29 04:05:04.000000 UIron-0.0.4/setup.py
```

### Comparing `UIron-0.0.3/LICENSE` & `UIron-0.0.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Copyright (c) <year> <copyright holders>
+"""Copyright (c) <2023> <Armando Chaparro>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `UIron-0.0.3/UIron/config.py` & `UIron-0.0.4/UIron/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,41 @@
 from UIron.utils import prettify
 
 class ConfigError(Exception):
     ...
 
 
 class Config:
-    def __init__(self, config_path: str, auto_save: bool=True, indent: int=4):
+    def __init__(
+            self, config_path: str, auto_save: bool=True, indent: int=4,
+            create_new: bool=True
+    ):
         
         # PROPERTIES
         self.indent = indent
         self.path = config_path
-        self.config = self.load()
+        self.config = self.load(create_new)
         self.auto_save = auto_save
     
-    def load(self) -> None:
+    def load(self, create_new: bool=True) -> None:
         """Loads the configutation from json to dictionary"""
         try:
             with open(self.path, 'r') as f: config = json.load(f)
         except json.decoder.JSONDecodeError:
             raise ConfigError('Invalid json content. Please verify file...')
+        except FileNotFoundError:
+            if create_new: return self.new()
+            raise ConfigError('No such file or directory')
         return config
     
+    def new(self):
+        self.config = dict()
+        self.save()
+        return self.config
+
     def save(self) -> None:
         """Saves the configuration based on dictionary"""
         with open(self.path, 'w') as f:
             json.dump(self.config, f, indent=self.indent)
     
     def __getitem__(self, key: str) -> object:
         if not key in self.config: raise ConfigError(f'Attribute "{key}" does not exist.')
```

### Comparing `UIron-0.0.3/setup.py` & `UIron-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Package for User Interface"
 LONG_DESCRIPTION = "Package for User Interface"
 
 setup(
     name="UIron",
     version=VERSION,
     author="Armando Chaparro",
```

