# Comparing `tmp/UIron-0.0.4.tar.gz` & `tmp/UIron-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UIron-0.0.4.tar", last modified: Sat Jul 29 04:05:05 2023, max compression
+gzip compressed data, was "UIron-0.0.5.tar", last modified: Sat Jul 29 04:29:33 2023, max compression
```

## Comparing `UIron-0.0.4.tar` & `UIron-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.849826 UIron-0.0.4/
--rw-rw-rw-   0        0        0     1087 2023-07-27 19:37:41.000000 UIron-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      460 2023-07-29 04:05:05.848830 UIron-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.772818 UIron-0.0.4/UIron/
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.4/UIron/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.4/UIron/__main__.py
--rw-rw-rw-   0        0        0     1600 2023-07-28 05:16:34.000000 UIron-0.0.4/UIron/config.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.844826 UIron-0.0.4/UIron/data/
--rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.4/UIron/data/config.json
--rw-rw-rw-   0        0        0        2 2023-07-28 05:20:04.000000 UIron-0.0.4/UIron/data/new.json
--rw-rw-rw-   0        0        0      121 2023-07-28 05:22:37.000000 UIron-0.0.4/UIron/regex.py
--rw-rw-rw-   0        0        0     9412 2023-07-29 03:48:19.000000 UIron-0.0.4/UIron/ui.py
--rw-rw-rw-   0        0        0     2234 2023-07-29 03:02:18.000000 UIron-0.0.4/UIron/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 04:05:05.830824 UIron-0.0.4/UIron.egg-info/
--rw-rw-rw-   0        0        0      460 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-29 04:05:05.000000 UIron-0.0.4/UIron.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 04:05:05.849826 UIron-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-07-29 04:05:04.000000 UIron-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:29:33.867541 UIron-0.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 19:37:41.000000 UIron-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      460 2023-07-29 04:29:33.866536 UIron-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 04:29:33.825138 UIron-0.0.5/UIron/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.5/UIron/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.5/UIron/__main__.py
+-rw-rw-rw-   0        0        0     1600 2023-07-28 05:16:34.000000 UIron-0.0.5/UIron/config.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:29:33.862547 UIron-0.0.5/UIron/data/
+-rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.5/UIron/data/config.json
+-rw-rw-rw-   0        0        0        2 2023-07-28 05:20:04.000000 UIron-0.0.5/UIron/data/new.json
+-rw-rw-rw-   0        0        0      121 2023-07-28 05:22:37.000000 UIron-0.0.5/UIron/regex.py
+-rw-rw-rw-   0        0        0     9414 2023-07-29 04:28:55.000000 UIron-0.0.5/UIron/ui.py
+-rw-rw-rw-   0        0        0     2234 2023-07-29 03:02:18.000000 UIron-0.0.5/UIron/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:29:33.857536 UIron-0.0.5/UIron.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-07-29 04:29:33.000000 UIron-0.0.5/UIron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-29 04:29:33.000000 UIron-0.0.5/UIron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:29:33.000000 UIron-0.0.5/UIron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 04:29:33.000000 UIron-0.0.5/UIron.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-29 04:29:33.000000 UIron-0.0.5/UIron.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:29:33.868537 UIron-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-07-29 04:29:32.000000 UIron-0.0.5/setup.py
```

### Comparing `UIron-0.0.4/LICENSE` & `UIron-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `UIron-0.0.4/UIron/config.py` & `UIron-0.0.5/UIron/config.py`

 * *Files identical despite different names*

### Comparing `UIron-0.0.4/UIron/ui.py` & `UIron-0.0.5/UIron/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,24 +36,24 @@
         super().__init__(master, **kwargs)
 
         # PROPERTIES
         self.base_string = 'Ready to continue...'
         self.text = ttk.StringVar()
         self.text_label = ttk.Label(self, textvariable=self.text)
         self.text_label.pack(anchor='w', padx=10)
-        self.raise_notification = raise_notification
+        self._raise_notification = raise_notification
         self.reset()
     
     def raise_notification(self, text: str, type_: str) -> None:
         """Raises a notificacion, is a template"""
         style = 'danger' if type_ == 'error' else type_
         self.config(bootstyle=style)
         self.text_label.config(bootstyle=f'{style}-inverse')
         self.text.set(text)
-        if not self.raise_notification: return self.reset()
+        if not self._raise_notification: return self.reset()
         notification = getattr(Messagebox, f'show_{type_}')
         notification(text, title=type_.title(), parent=self.master)
         self.reset()
 
     def warning(self, text: str) -> None:
         """Changes the bar and raises a warning notification"""
         self.raise_notification(text, 'warning')
```

### Comparing `UIron-0.0.4/UIron/utils.py` & `UIron-0.0.5/UIron/utils.py`

 * *Files identical despite different names*

### Comparing `UIron-0.0.4/setup.py` & `UIron-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Package for User Interface"
 LONG_DESCRIPTION = "Package for User Interface"
 
 setup(
     name="UIron",
     version=VERSION,
     author="Armando Chaparro",
```

