# Comparing `tmp/dash_component_editor-0.0.6.tar.gz` & `tmp/dash_component_editor-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_component_editor-0.0.6.tar", last modified: Thu Apr 20 06:12:13 2023, max compression
+gzip compressed data, was "dash_component_editor-0.0.7.tar", last modified: Fri Jul 28 23:35:50 2023, max compression
```

## Comparing `dash_component_editor-0.0.6.tar` & `dash_component_editor-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-20 06:12:13.365538 dash_component_editor-0.0.6/
--rw-r--r--   0 zhuowen    (501) staff       (20)     2401 2023-03-27 16:49:46.000000 dash_component_editor-0.0.6/LICENSE.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)     3521 2023-04-20 06:12:13.365323 dash_component_editor-0.0.6/PKG-INFO
--rw-r--r--   0 zhuowen    (501) staff       (20)     2889 2023-04-20 06:09:34.000000 dash_component_editor-0.0.6/README.md
--rw-r--r--   0 zhuowen    (501) staff       (20)       38 2023-04-20 06:12:13.365647 dash_component_editor-0.0.6/setup.cfg
--rwxr--r--   0 zhuowen    (501) staff       (20)     1613 2023-04-20 06:08:59.000000 dash_component_editor-0.0.6/setup.py
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-20 06:12:13.363876 dash_component_editor-0.0.6/src/
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-20 06:12:13.365029 dash_component_editor-0.0.6/src/dash_component_editor.egg-info/
--rw-r--r--   0 zhuowen    (501) staff       (20)     3521 2023-04-20 06:12:13.000000 dash_component_editor-0.0.6/src/dash_component_editor.egg-info/PKG-INFO
--rw-r--r--   0 zhuowen    (501) staff       (20)      303 2023-04-20 06:12:13.000000 dash_component_editor-0.0.6/src/dash_component_editor.egg-info/SOURCES.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)        1 2023-04-20 06:12:13.000000 dash_component_editor-0.0.6/src/dash_component_editor.egg-info/dependency_links.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)       61 2023-04-20 06:12:13.000000 dash_component_editor-0.0.6/src/dash_component_editor.egg-info/requires.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)       22 2023-04-20 06:12:13.000000 dash_component_editor-0.0.6/src/dash_component_editor.egg-info/top_level.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)    15045 2023-04-09 00:35:55.000000 dash_component_editor-0.0.6/src/dash_component_editor.py
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-07-28 23:35:50.364082 dash_component_editor-0.0.7/
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2401 2023-03-27 16:49:46.000000 dash_component_editor-0.0.7/LICENSE.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)     3521 2023-07-28 23:35:50.363925 dash_component_editor-0.0.7/PKG-INFO
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2889 2023-04-20 06:09:34.000000 dash_component_editor-0.0.7/README.md
+-rw-r--r--   0 zhuowen    (501) staff       (20)       38 2023-07-28 23:35:50.364137 dash_component_editor-0.0.7/setup.cfg
+-rwxr--r--   0 zhuowen    (501) staff       (20)     1613 2023-07-28 23:35:24.000000 dash_component_editor-0.0.7/setup.py
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-07-28 23:35:50.363020 dash_component_editor-0.0.7/src/
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-07-28 23:35:50.363711 dash_component_editor-0.0.7/src/dash_component_editor.egg-info/
+-rw-r--r--   0 zhuowen    (501) staff       (20)     3521 2023-07-28 23:35:50.000000 dash_component_editor-0.0.7/src/dash_component_editor.egg-info/PKG-INFO
+-rw-r--r--   0 zhuowen    (501) staff       (20)      303 2023-07-28 23:35:50.000000 dash_component_editor-0.0.7/src/dash_component_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)        1 2023-07-28 23:35:50.000000 dash_component_editor-0.0.7/src/dash_component_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)       61 2023-07-28 23:35:50.000000 dash_component_editor-0.0.7/src/dash_component_editor.egg-info/requires.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)       22 2023-07-28 23:35:50.000000 dash_component_editor-0.0.7/src/dash_component_editor.egg-info/top_level.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)    14997 2023-07-28 23:29:11.000000 dash_component_editor-0.0.7/src/dash_component_editor.py
```

### Comparing `dash_component_editor-0.0.6/LICENSE.txt` & `dash_component_editor-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash_component_editor-0.0.6/PKG-INFO` & `dash_component_editor-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_component_editor
-Version: 0.0.6
+Version: 0.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Zhuowen (Kevin) Zhao, Ronald Pandolfi
 Author-email: zwenzhao11@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/mlexchange/mlex_dash_component_editor.git
 Platform: UNKNOWN
```

### Comparing `dash_component_editor-0.0.6/README.md` & `dash_component_editor-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dash_component_editor-0.0.6/setup.py` & `dash_component_editor-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dash_component_editor",                     # This is the name of the package
-    version="0.0.6",                        # The release version
+    version="0.0.7",                        # The release version
     author="Zhuowen (Kevin) Zhao, Ronald Pandolfi",                     # Full name of the author
     author_email='zwenzhao11@gmail.com',
     description="",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     license_files = ('LICENSE.txt',),                                     # Information to filter the project on PyPi website
```

### Comparing `dash_component_editor-0.0.6/src/dash_component_editor.egg-info/PKG-INFO` & `dash_component_editor-0.0.7/src/dash_component_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-component-editor
-Version: 0.0.6
+Version: 0.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Zhuowen (Kevin) Zhao, Ronald Pandolfi
 Author-email: zwenzhao11@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/mlexchange/mlex_dash_component_editor.git
 Platform: UNKNOWN
```

### Comparing `dash_component_editor-0.0.6/src/dash_component_editor.py` & `dash_component_editor-0.0.7/src/dash_component_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,20 +311,20 @@
     def __init__(self, _id, parameters, **kwargs):
         self._parameters = parameters
 
         super(ParameterEditor, self).__init__(id=_id, children=[], className='kwarg-editor', **kwargs)
         self.children = self.build_children()
 
     def init_callbacks(self, app):
-        app.callback(Output(self.id, 'n_submit', allow_duplicate=True), 
+        app.callback(Output(self.id, 'n_submit'), 
                      Input({**self.id,
                             'name': ALL},
                             'value'), 
                      State(self.id, 'n_submit'), 
-                     prevent_initial_call=True)
+                    )
                      
         for child in self.children:
             if hasattr(child,"init_callbacks"):
                 child.init_callbacks(app)  
 
     @property
     def values(self):
```

