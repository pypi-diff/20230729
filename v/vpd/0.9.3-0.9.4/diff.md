# Comparing `tmp/vpd-0.9.3.tar.gz` & `tmp/vpd-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpd-0.9.3.tar", last modified: Sun Aug  7 19:40:19 2022, max compression
+gzip compressed data, was "vpd-0.9.4.tar", last modified: Wed Mar  1 17:28:08 2023, max compression
```

## Comparing `vpd-0.9.3.tar` & `vpd-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-07 19:40:19.208802 vpd-0.9.3/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1813 2020-10-16 01:19:33.000000 vpd-0.9.3/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      928 2022-08-07 19:40:19.204802 vpd-0.9.3/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      276 2020-10-12 01:40:45.000000 vpd-0.9.3/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2022-08-07 19:40:19.210815 vpd-0.9.3/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      960 2022-08-07 19:33:13.000000 vpd-0.9.3/setup.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-07 19:40:19.007961 vpd-0.9.3/vpd/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      293 2020-10-16 01:24:06.000000 vpd-0.9.3/vpd/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3438 2020-10-12 01:52:02.000000 vpd-0.9.3/vpd/arguments.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4201 2022-08-07 19:30:38.000000 vpd-0.9.3/vpd/cid.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      659 2022-08-07 19:32:10.000000 vpd-0.9.3/vpd/cmp.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3528 2022-08-07 19:34:12.000000 vpd-0.9.3/vpd/iterable.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14336 2020-10-12 01:52:20.000000 vpd-0.9.3/vpd/yaml_dict.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-07 19:40:19.169559 vpd-0.9.3/vpd.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      928 2022-08-07 19:40:16.000000 vpd-0.9.3/vpd.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      248 2022-08-07 19:40:18.000000 vpd-0.9.3/vpd.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-07 19:40:16.000000 vpd-0.9.3/vpd.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       11 2022-08-07 19:40:16.000000 vpd-0.9.3/vpd.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2022-08-07 19:40:16.000000 vpd-0.9.3/vpd.egg-info/top_level.txt
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-01 17:28:08.148789 vpd-0.9.4/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1813 2020-10-16 01:19:33.000000 vpd-0.9.4/LICENSE
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-01 17:28:08.136795 vpd-0.9.4/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      276 2020-10-12 01:40:45.000000 vpd-0.9.4/README.md
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-01 17:28:08.152789 vpd-0.9.4/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      960 2023-03-01 17:27:05.000000 vpd-0.9.4/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-01 17:28:07.664790 vpd-0.9.4/vpd/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      293 2020-10-16 01:24:06.000000 vpd-0.9.4/vpd/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3438 2020-10-12 01:52:02.000000 vpd-0.9.4/vpd/arguments.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4201 2022-08-07 19:30:38.000000 vpd-0.9.4/vpd/cid.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      659 2022-08-07 19:32:10.000000 vpd-0.9.4/vpd/cmp.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3528 2022-08-07 19:34:12.000000 vpd-0.9.4/vpd/iterable.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14315 2023-03-01 17:26:39.000000 vpd-0.9.4/vpd/yaml_dict.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-01 17:28:08.047792 vpd-0.9.4/vpd.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      928 2023-03-01 17:28:05.000000 vpd-0.9.4/vpd.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      248 2023-03-01 17:28:06.000000 vpd-0.9.4/vpd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-01 17:28:05.000000 vpd-0.9.4/vpd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       11 2023-03-01 17:28:05.000000 vpd-0.9.4/vpd.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2023-03-01 17:28:05.000000 vpd-0.9.4/vpd.egg-info/top_level.txt
```

### Comparing `vpd-0.9.3/LICENSE` & `vpd-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vpd-0.9.3/PKG-INFO` & `vpd-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpd
-Version: 0.9.3
+Version: 0.9.4
 Summary: VirtualPathDictChains. Hierarchical, Addressable Dicts, potentially using YaML
 Home-page: https://github.com/dbotwinick/python-vpd
 Author: Drew Botwinick
 Author-email: foss@drewbotwinick.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vpd-0.9.3/setup.py` & `vpd-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     readme_txt = f.read()
 
 setuptools.setup(
     name="vpd",
-    version="0.9.3",
+    version="0.9.4",
     author="Drew Botwinick",
     author_email="foss@drewbotwinick.com",
     description="VirtualPathDictChains. Hierarchical, Addressable Dicts, potentially using YaML",
     long_description=readme_txt,
     long_description_content_type="text/markdown",
     url="https://github.com/dbotwinick/python-vpd",
     packages=setuptools.find_packages(),
```

### Comparing `vpd-0.9.3/vpd/arguments.py` & `vpd-0.9.4/vpd/arguments.py`

 * *Files identical despite different names*

### Comparing `vpd-0.9.3/vpd/cid.py` & `vpd-0.9.4/vpd/cid.py`

 * *Files identical despite different names*

### Comparing `vpd-0.9.3/vpd/cmp.py` & `vpd-0.9.4/vpd/cmp.py`

 * *Files identical despite different names*

### Comparing `vpd-0.9.3/vpd/iterable.py` & `vpd-0.9.4/vpd/iterable.py`

 * *Files identical despite different names*

### Comparing `vpd-0.9.3/vpd/yaml_dict.py` & `vpd-0.9.4/vpd/yaml_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # author: Drew Botwinick, Botwinick Innovations
 # license: 3-clause BSD
-import collections
 from os import path as osp
 
 import yaml
 from six import iteritems, string_types
 
 from .arguments import arg_substitute
 
+try:
+    from collections import Mapping
+except ImportError:
+    from collections.abc import Mapping
+
 
 def read_yaml(path, origin=None, return_path=False, windows_pseudo_links=True):
     """
     extended function to read yaml files and potentially augment the source path relative to another path and/or return the path
     :param path:
     :param origin:
     :param return_path: whether to return the path
@@ -54,15 +58,15 @@
     :return: merged dictionary
     """
     skip_none_values = kwargs.get('skip_none_values', True)
     add_lists = kwargs.get('add_lists', False)
 
     result = dict()
     for include in data_dicts:
-        if not isinstance(include, collections.Mapping):  # skip non-dictionary inputs (intended for filtering Nones etc.)
+        if not isinstance(include, Mapping):  # skip non-dictionary inputs (intended for filtering Nones etc.)
             continue
         # result.update({k: v for (k, v) in include.iteritems() if v is not None or not skip_none_values})
         for k, v in iteritems(include):
             if v is not None or not skip_none_values:
                 # if we're adding lists and we've already got a list and the next thing is another one, then add
                 if add_lists and k in result and isinstance(result[k], list) and isinstance(v, list):
                     result[k] += v
@@ -75,15 +79,15 @@
     """
     sneaky component for grabbing "sub-dict" data with builtin support for external yaml sources and including external files
 
     :param sub_dict:
     :param cwd:
     :return:
     """
-    if not isinstance(sub_dict, collections.Mapping):
+    if not isinstance(sub_dict, Mapping):
         return None
 
     data = dict(sub_dict)  # operate on a shallow copy
 
     if 'source' in data:  # then use external data
         data = get_data(*read_yaml(data['source'], cwd, return_path=True))
     elif 'include' in data:  # merge external data
@@ -107,15 +111,15 @@
     :rtype: VirtualPathDictChain
     """
     vpd = None
     for mapping in reversed(mappings):
         if isinstance(mapping, VirtualPathDictChain):
             for sub_map in reversed(_unchain_vpd(mapping)):
                 vpd = VirtualPathDictChain(sub_map, vpd)
-        elif isinstance(mapping, collections.Mapping):
+        elif isinstance(mapping, Mapping):
             vpd = VirtualPathDictChain(mapping, vpd)
         elif mapping is not None:
             raise ValueError('all arguments must either be Mappings or VirtualPathDictChains')
     return vpd
 
 
 def _unchain_vpd(vpd):
@@ -214,17 +218,17 @@
         :param iter_key: iterable with key parts
         :param from_default: whether to load value from default or 'custom' settings. custom always cascades to default
         """
         if not from_default:
             r = self._data
             if r:
                 for arg in iter_key:
-                    if isinstance(r, collections.Mapping) and arg in r:
+                    if isinstance(r, Mapping) and arg in r:
                         r = r[arg]
-                    elif isinstance(r, collections.Mapping) and arg not in r:  # and not from_default:
+                    elif isinstance(r, Mapping) and arg not in r:  # and not from_default:
                         return self._fallback._get(iter_key) if self._fallback else None
                     else:
                         return None
                 return r
         return self._fallback._get(iter_key) if self._fallback else None
 
     def put(self, key, value):
@@ -245,15 +249,15 @@
     def _put(self, iter_key, value):
         if self._data is None:
             self._data = dict()
         r = self._data
         l = len(iter_key)
         for i in range(l):
             arg = iter_key[i]
-            if i < l - 1 and isinstance(r, collections.Mapping) and arg not in r:  # not at end and missing arg, create missing dict
+            if i < l - 1 and isinstance(r, Mapping) and arg not in r:  # not at end and missing arg, create missing dict
                 r[arg] = dict()
             elif i == l - 1:
                 r[arg] = value
                 break  # this shouldn't be necessary...
             r = r[arg]
         return value
 
@@ -270,15 +274,15 @@
 
     :param vpd:
     :return:
     """
     if vpd and isinstance(vpd, VirtualPathDictChain):
         # noinspection PyProtectedMember
         return vpd._data
-    elif isinstance(vpd, collections.Mapping):
+    elif isinstance(vpd, Mapping):
         return vpd
     return None
 
 
 class Settings(VirtualPathDictChain):
     settings_file = None
 
@@ -292,15 +296,15 @@
         file, env, hard-coded, or nothing)
         """
         self._dsf = default_settings_fn
         self.data_home = data_home
         self.file_name = file_name
         self.settings_file = osp.join(self.data_home, self.file_name)
         _current_dsf = self._dsf()
-        fallback = VirtualPathDictChain(_current_dsf, None) if isinstance(_current_dsf, collections.Mapping) else None
+        fallback = VirtualPathDictChain(_current_dsf, None) if isinstance(_current_dsf, Mapping) else None
         super(Settings, self).__init__(self._load(), fallback)
         self.refresh()
 
     # # TODO: evaluate performance implications with or without ttl cache (thread sync vs get look-ups)
     # @ttl_cache(ttl=120)  # TODO: make TTL cache configurable to support unit tests that can check functionality without long waits
     def get(self, key, from_default=False, do_substitute=False):
         return super(Settings, self).get(key, from_default, do_substitute)
@@ -332,10 +336,10 @@
     def refresh(self):
         """
         discard any changes in memory and refresh configuration to on-disk state
         """
         self.settings_file = osp.join(self.data_home, self.file_name)
         self._data = self._load()
         _current_dsf = self._dsf()
-        self._fallback = VirtualPathDictChain(_current_dsf, None) if isinstance(_current_dsf, collections.Mapping) else None
+        self._fallback = VirtualPathDictChain(_current_dsf, None) if isinstance(_current_dsf, Mapping) else None
         # TODO: reset TTL cache for get(...)
         return self
```

### Comparing `vpd-0.9.3/vpd.egg-info/PKG-INFO` & `vpd-0.9.4/vpd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpd
-Version: 0.9.3
+Version: 0.9.4
 Summary: VirtualPathDictChains. Hierarchical, Addressable Dicts, potentially using YaML
 Home-page: https://github.com/dbotwinick/python-vpd
 Author: Drew Botwinick
 Author-email: foss@drewbotwinick.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

