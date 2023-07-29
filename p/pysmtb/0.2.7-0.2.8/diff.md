# Comparing `tmp/pysmtb-0.2.7.tar.gz` & `tmp/pysmtb-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmtb-0.2.7.tar", last modified: Tue Feb 28 09:22:58 2023, max compression
+gzip compressed data, was "pysmtb-0.2.8.tar", last modified: Sat Jul 29 21:43:13 2023, max compression
```

## Comparing `pysmtb-0.2.7.tar` & `pysmtb-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 spl       (1000) spl       (1000)        0 2023-02-28 09:22:58.614045 pysmtb-0.2.7/
--rw-rw-r--   0 spl       (1000) spl       (1000)     1075 2022-11-06 08:35:52.000000 pysmtb-0.2.7/LICENSE
--rw-rw-r--   0 spl       (1000) spl       (1000)    12581 2023-02-28 09:22:58.614045 pysmtb-0.2.7/PKG-INFO
--rw-rw-r--   0 spl       (1000) spl       (1000)    11981 2022-11-06 08:35:52.000000 pysmtb-0.2.7/README.md
-drwxrwxr-x   0 spl       (1000) spl       (1000)        0 2023-02-28 09:22:58.614045 pysmtb-0.2.7/pysmtb/
--rw-rw-r--   0 spl       (1000) spl       (1000)      139 2022-11-06 08:35:52.000000 pysmtb-0.2.7/pysmtb/__init__.py
--rw-rw-r--   0 spl       (1000) spl       (1000)     4720 2022-11-06 08:35:52.000000 pysmtb-0.2.7/pysmtb/btf.py
--rw-rw-r--   0 spl       (1000) spl       (1000)     3363 2022-11-06 08:35:52.000000 pysmtb-0.2.7/pysmtb/geometry.py
--rw-rw-r--   0 spl       (1000) spl       (1000)    31448 2023-02-28 09:22:40.000000 pysmtb-0.2.7/pysmtb/image.py
--rw-rw-r--   0 spl       (1000) spl       (1000)    64956 2023-02-27 00:23:44.000000 pysmtb-0.2.7/pysmtb/iv.py
--rw-rw-r--   0 spl       (1000) spl       (1000)     8045 2022-11-06 08:35:52.000000 pysmtb-0.2.7/pysmtb/plotting.py
--rw-rw-r--   0 spl       (1000) spl       (1000)    37384 2022-11-06 08:35:52.000000 pysmtb-0.2.7/pysmtb/rendering.py
--rw-rw-r--   0 spl       (1000) spl       (1000)    15979 2022-11-06 08:35:52.000000 pysmtb-0.2.7/pysmtb/utils.py
-drwxrwxr-x   0 spl       (1000) spl       (1000)        0 2023-02-28 09:22:58.614045 pysmtb-0.2.7/pysmtb.egg-info/
--rw-rw-r--   0 spl       (1000) spl       (1000)    12581 2023-02-28 09:22:58.000000 pysmtb-0.2.7/pysmtb.egg-info/PKG-INFO
--rw-rw-r--   0 spl       (1000) spl       (1000)      344 2023-02-28 09:22:58.000000 pysmtb-0.2.7/pysmtb.egg-info/SOURCES.txt
--rw-rw-r--   0 spl       (1000) spl       (1000)        1 2023-02-28 09:22:58.000000 pysmtb-0.2.7/pysmtb.egg-info/dependency_links.txt
--rw-rw-r--   0 spl       (1000) spl       (1000)       41 2023-02-28 09:22:58.000000 pysmtb-0.2.7/pysmtb.egg-info/entry_points.txt
--rw-rw-r--   0 spl       (1000) spl       (1000)      132 2023-02-28 09:22:58.000000 pysmtb-0.2.7/pysmtb.egg-info/requires.txt
--rw-rw-r--   0 spl       (1000) spl       (1000)        7 2023-02-28 09:22:58.000000 pysmtb-0.2.7/pysmtb.egg-info/top_level.txt
--rw-rw-r--   0 spl       (1000) spl       (1000)       38 2023-02-28 09:22:58.614045 pysmtb-0.2.7/setup.cfg
--rw-rw-r--   0 spl       (1000) spl       (1000)     1125 2023-02-28 09:22:55.000000 pysmtb-0.2.7/setup.py
+drwxrwxr-x   0 spl       (1000) spl       (1000)        0 2023-07-29 21:43:13.531624 pysmtb-0.2.8/
+-rw-rw-r--   0 spl       (1000) spl       (1000)     1075 2022-11-06 08:35:52.000000 pysmtb-0.2.8/LICENSE
+-rw-rw-r--   0 spl       (1000) spl       (1000)    12581 2023-07-29 21:43:13.531624 pysmtb-0.2.8/PKG-INFO
+-rw-rw-r--   0 spl       (1000) spl       (1000)    11981 2022-11-06 08:35:52.000000 pysmtb-0.2.8/README.md
+drwxrwxr-x   0 spl       (1000) spl       (1000)        0 2023-07-29 21:43:13.531624 pysmtb-0.2.8/pysmtb/
+-rw-rw-r--   0 spl       (1000) spl       (1000)      139 2022-11-06 08:35:52.000000 pysmtb-0.2.8/pysmtb/__init__.py
+-rw-rw-r--   0 spl       (1000) spl       (1000)     4720 2022-11-06 08:35:52.000000 pysmtb-0.2.8/pysmtb/btf.py
+-rw-rw-r--   0 spl       (1000) spl       (1000)     3363 2022-11-06 08:35:52.000000 pysmtb-0.2.8/pysmtb/geometry.py
+-rw-rw-r--   0 spl       (1000) spl       (1000)    31448 2023-02-28 09:22:40.000000 pysmtb-0.2.8/pysmtb/image.py
+-rw-rw-r--   0 spl       (1000) spl       (1000)    64956 2023-07-29 21:43:01.000000 pysmtb-0.2.8/pysmtb/iv.py
+-rw-rw-r--   0 spl       (1000) spl       (1000)     8045 2022-11-06 08:35:52.000000 pysmtb-0.2.8/pysmtb/plotting.py
+-rw-rw-r--   0 spl       (1000) spl       (1000)    37384 2022-11-06 08:35:52.000000 pysmtb-0.2.8/pysmtb/rendering.py
+-rw-rw-r--   0 spl       (1000) spl       (1000)    16143 2023-07-29 21:43:01.000000 pysmtb-0.2.8/pysmtb/utils.py
+drwxrwxr-x   0 spl       (1000) spl       (1000)        0 2023-07-29 21:43:13.531624 pysmtb-0.2.8/pysmtb.egg-info/
+-rw-rw-r--   0 spl       (1000) spl       (1000)    12581 2023-07-29 21:43:13.000000 pysmtb-0.2.8/pysmtb.egg-info/PKG-INFO
+-rw-rw-r--   0 spl       (1000) spl       (1000)      344 2023-07-29 21:43:13.000000 pysmtb-0.2.8/pysmtb.egg-info/SOURCES.txt
+-rw-rw-r--   0 spl       (1000) spl       (1000)        1 2023-07-29 21:43:13.000000 pysmtb-0.2.8/pysmtb.egg-info/dependency_links.txt
+-rw-rw-r--   0 spl       (1000) spl       (1000)       41 2023-07-29 21:43:13.000000 pysmtb-0.2.8/pysmtb.egg-info/entry_points.txt
+-rw-rw-r--   0 spl       (1000) spl       (1000)      132 2023-07-29 21:43:13.000000 pysmtb-0.2.8/pysmtb.egg-info/requires.txt
+-rw-rw-r--   0 spl       (1000) spl       (1000)        7 2023-07-29 21:43:13.000000 pysmtb-0.2.8/pysmtb.egg-info/top_level.txt
+-rw-rw-r--   0 spl       (1000) spl       (1000)       38 2023-07-29 21:43:13.531624 pysmtb-0.2.8/setup.cfg
+-rw-rw-r--   0 spl       (1000) spl       (1000)     1125 2023-07-29 21:43:01.000000 pysmtb-0.2.8/setup.py
```

### Comparing `pysmtb-0.2.7/LICENSE` & `pysmtb-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmtb-0.2.7/PKG-INFO` & `pysmtb-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmtb
-Version: 0.2.7
+Version: 0.2.8
 Summary: python toolbox of (mostly) image-related helper / visualization functions
 Home-page: https://github.com/smerzbach/pysmtb
 Author: Sebastian Merzbach
 Author-email: smerzbach@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysmtb-0.2.7/README.md` & `pysmtb-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pysmtb-0.2.7/pysmtb/btf.py` & `pysmtb-0.2.8/pysmtb/btf.py`

 * *Files identical despite different names*

### Comparing `pysmtb-0.2.7/pysmtb/geometry.py` & `pysmtb-0.2.8/pysmtb/geometry.py`

 * *Files identical despite different names*

### Comparing `pysmtb-0.2.7/pysmtb/image.py` & `pysmtb-0.2.8/pysmtb/image.py`

 * *Files identical despite different names*

### Comparing `pysmtb-0.2.7/pysmtb/iv.py` & `pysmtb-0.2.8/pysmtb/iv.py`

 * *Files 0% similar despite different names*

```diff
@@ -910,15 +910,15 @@
         return [self.get_img(ind, tonemap=tonemap, decorate=decorate) for ind in range(len(self.images))]
 
     def decorate(self, im, i=None, label=''):
         """add annotation to an image"""
         if i is None:
             i = self.imind
         if self.annotate:
-            from pysmtb.utils import annotate_image
+            from pysmtb.image import annotate_image
             if self.annotate_numbers:
                 label += str(i) + ' '
             if self.labels is not None:
                 label += self.labels[i]
             if im.shape[2] == 3:
                 im = annotate_image(im, label, font_size=self.font_size, font_color=self.font_color)
             else:
```

### Comparing `pysmtb-0.2.7/pysmtb/plotting.py` & `pysmtb-0.2.8/pysmtb/plotting.py`

 * *Files identical despite different names*

### Comparing `pysmtb-0.2.7/pysmtb/rendering.py` & `pysmtb-0.2.8/pysmtb/rendering.py`

 * *Files identical despite different names*

### Comparing `pysmtb-0.2.7/pysmtb/utils.py` & `pysmtb-0.2.8/pysmtb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,10 +415,14 @@
         self[key] = val
 
     def __repr__(self):
         if not len(self):
             return ""
         width = max([len(str(k)) for k in self])
         items = '{:' + str(width + 2) + 's} {}'
-        items = [items.format(str(key) + ':', self[key]) for key in sorted(self.keys())]
+        try:
+            items = [items.format(str(key) + ':', self[key]) for key in sorted(self.keys())]
+        except TypeError:
+            # keys are not sortable
+            items = [items.format(str(key) + ':', self[key]) for key in self.keys()]
         items = '\n'.join(items)
         return items
```

### Comparing `pysmtb-0.2.7/pysmtb.egg-info/PKG-INFO` & `pysmtb-0.2.8/pysmtb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmtb
-Version: 0.2.7
+Version: 0.2.8
 Summary: python toolbox of (mostly) image-related helper / visualization functions
 Home-page: https://github.com/smerzbach/pysmtb
 Author: Sebastian Merzbach
 Author-email: smerzbach@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pysmtb-0.2.7/setup.py` & `pysmtb-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pysmtb",
-    version="0.2.7",
+    version="0.2.8",
     author="Sebastian Merzbach",
     author_email="smerzbach@gmail.com",
     description="python toolbox of (mostly) image-related helper / visualization functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/smerzbach/pysmtb",
     packages=setuptools.find_packages(),
```

