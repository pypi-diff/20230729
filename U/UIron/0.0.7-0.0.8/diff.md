# Comparing `tmp/UIron-0.0.7.tar.gz` & `tmp/UIron-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UIron-0.0.7.tar", last modified: Sat Jul 29 04:36:32 2023, max compression
+gzip compressed data, was "UIron-0.0.8.tar", last modified: Sat Jul 29 04:44:34 2023, max compression
```

## Comparing `UIron-0.0.7.tar` & `UIron-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 04:36:32.886108 UIron-0.0.7/
--rw-rw-rw-   0        0        0     1087 2023-07-27 19:37:41.000000 UIron-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      460 2023-07-29 04:36:32.884108 UIron-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 04:36:32.839104 UIron-0.0.7/UIron/
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.7/UIron/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.7/UIron/__main__.py
--rw-rw-rw-   0        0        0     1600 2023-07-28 05:16:34.000000 UIron-0.0.7/UIron/config.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:36:32.881111 UIron-0.0.7/UIron/data/
--rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.7/UIron/data/config.json
--rw-rw-rw-   0        0        0        2 2023-07-28 05:20:04.000000 UIron-0.0.7/UIron/data/new.json
--rw-rw-rw-   0        0        0      121 2023-07-28 05:22:37.000000 UIron-0.0.7/UIron/regex.py
--rw-rw-rw-   0        0        0     9525 2023-07-29 04:36:02.000000 UIron-0.0.7/UIron/ui.py
--rw-rw-rw-   0        0        0     2234 2023-07-29 03:02:18.000000 UIron-0.0.7/UIron/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:36:32.872107 UIron-0.0.7/UIron.egg-info/
--rw-rw-rw-   0        0        0      460 2023-07-29 04:36:32.000000 UIron-0.0.7/UIron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-29 04:36:32.000000 UIron-0.0.7/UIron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 04:36:32.000000 UIron-0.0.7/UIron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-29 04:36:32.000000 UIron-0.0.7/UIron.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-29 04:36:32.000000 UIron-0.0.7/UIron.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 04:36:32.886108 UIron-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-07-29 04:36:31.000000 UIron-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.846202 UIron-0.0.8/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 19:37:41.000000 UIron-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      460 2023-07-29 04:44:34.844202 UIron-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.800320 UIron-0.0.8/UIron/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.8/UIron/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.8/UIron/__main__.py
+-rw-rw-rw-   0        0        0     1600 2023-07-28 05:16:34.000000 UIron-0.0.8/UIron/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.838204 UIron-0.0.8/UIron/data/
+-rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.8/UIron/data/config.json
+-rw-rw-rw-   0        0        0        2 2023-07-28 05:20:04.000000 UIron-0.0.8/UIron/data/new.json
+-rw-rw-rw-   0        0        0      121 2023-07-28 05:22:37.000000 UIron-0.0.8/UIron/regex.py
+-rw-rw-rw-   0        0        0     9537 2023-07-29 04:44:01.000000 UIron-0.0.8/UIron/ui.py
+-rw-rw-rw-   0        0        0     2234 2023-07-29 03:02:18.000000 UIron-0.0.8/UIron/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:44:34.831203 UIron-0.0.8/UIron.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-29 04:44:34.000000 UIron-0.0.8/UIron.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:44:34.846202 UIron-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-07-29 04:44:33.000000 UIron-0.0.8/setup.py
```

### Comparing `UIron-0.0.7/LICENSE` & `UIron-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `UIron-0.0.7/UIron/config.py` & `UIron-0.0.8/UIron/config.py`

 * *Files identical despite different names*

### Comparing `UIron-0.0.7/UIron/ui.py` & `UIron-0.0.8/UIron/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,17 +180,17 @@
 
     def set(self, value: str) -> None:
         self.entry.delete(0, 'end')
         self.entry.insert(0, value)
 
 
 class Image(ttk.Label):
-    def __init__(self, master: ttk.Frame|ttk.Window, path: str, **kwargs):
+    def __init__(self, master: ttk.Frame|ttk.Window, path: str='', **kwargs):
         super().__init__(master, **kwargs)
-        self.config(image=path)
+        if path: self.config(image=path)
     
     def set_image(self, image) -> None:
         self._image = image
         self.width, self.height = self._image.size
         self.image = ImageTk.PhotoImage(self._image)
         super().config(image=self.image)
```

### Comparing `UIron-0.0.7/UIron/utils.py` & `UIron-0.0.8/UIron/utils.py`

 * *Files identical despite different names*

### Comparing `UIron-0.0.7/setup.py` & `UIron-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 DESCRIPTION = "Package for User Interface"
 LONG_DESCRIPTION = "Package for User Interface"
 
 setup(
     name="UIron",
     version=VERSION,
     author="Armando Chaparro",
```

