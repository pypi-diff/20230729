# Comparing `tmp/tera_utils-0.0.2.tar.gz` & `tmp/tera_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tera_utils-0.0.2.tar", last modified: Tue Apr  4 08:09:52 2023, max compression
+gzip compressed data, was "tera_utils-0.0.3.tar", last modified: Sat Jul 29 07:21:51 2023, max compression
```

## Comparing `tera_utils-0.0.2.tar` & `tera_utils-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 08:09:52.183242 tera_utils-0.0.2/
--rw-rw-rw-   0        0        0     1069 2023-04-04 06:55:35.000000 tera_utils-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0      508 2023-04-04 08:09:52.183242 tera_utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      604 2023-04-04 06:55:35.000000 tera_utils-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 08:09:52.184246 tera_utils-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-04-04 08:09:42.000000 tera_utils-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:09:52.154245 tera_utils-0.0.2/tera_utils/
--rw-rw-rw-   0        0        0      140 2023-04-04 06:55:35.000000 tera_utils-0.0.2/tera_utils/__init__.py
--rw-rw-rw-   0        0        0     2890 2023-04-04 07:44:28.000000 tera_utils-0.0.2/tera_utils/consol.py
--rw-rw-rw-   0        0        0      340 2023-04-04 06:55:35.000000 tera_utils-0.0.2/tera_utils/date.py
--rw-rw-rw-   0        0        0    12190 2023-04-04 07:43:01.000000 tera_utils-0.0.2/tera_utils/locals.py
--rw-rw-rw-   0        0        0     1637 2023-04-04 06:55:35.000000 tera_utils-0.0.2/tera_utils/search.py
--rw-rw-rw-   0        0        0     2743 2023-04-04 06:55:35.000000 tera_utils-0.0.2/tera_utils/sort.py
--rw-rw-rw-   0        0        0     3024 2023-04-04 07:01:47.000000 tera_utils-0.0.2/tera_utils/terminal.py
-drwxrwxrwx   0        0        0        0 2023-04-04 08:09:52.181246 tera_utils-0.0.2/tera_utils.egg-info/
--rw-rw-rw-   0        0        0      508 2023-04-04 08:09:52.000000 tera_utils-0.0.2/tera_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-04 08:09:52.000000 tera_utils-0.0.2/tera_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 08:09:52.000000 tera_utils-0.0.2/tera_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-04 08:09:52.000000 tera_utils-0.0.2/tera_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 07:21:51.237816 tera_utils-0.0.3/
+-rw-rw-rw-   0        0        0     1069 2023-07-28 18:09:47.000000 tera_utils-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0      508 2023-07-29 07:21:51.228784 tera_utils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2023-07-28 18:09:47.000000 tera_utils-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 07:21:51.237816 tera_utils-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-07-29 07:15:58.000000 tera_utils-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:21:51.221731 tera_utils-0.0.3/tera_utils/
+-rw-rw-rw-   0        0        0      135 2023-07-28 18:50:57.000000 tera_utils-0.0.3/tera_utils/__init__.py
+-rw-rw-rw-   0        0        0     3385 2023-07-28 18:51:06.000000 tera_utils-0.0.3/tera_utils/consol.py
+-rw-rw-rw-   0        0        0      340 2023-07-28 18:09:47.000000 tera_utils-0.0.3/tera_utils/date.py
+-rw-rw-rw-   0        0        0    12190 2023-07-28 18:09:47.000000 tera_utils-0.0.3/tera_utils/locals.py
+-rw-rw-rw-   0        0        0     1637 2023-07-28 18:09:47.000000 tera_utils-0.0.3/tera_utils/search.py
+-rw-rw-rw-   0        0        0     2743 2023-07-28 18:09:47.000000 tera_utils-0.0.3/tera_utils/sort.py
+-rw-rw-rw-   0        0        0     4418 2023-07-29 07:14:54.000000 tera_utils-0.0.3/tera_utils/table.py
+-rw-rw-rw-   0        0        0     3024 2023-07-28 18:09:47.000000 tera_utils-0.0.3/tera_utils/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:21:51.227823 tera_utils-0.0.3/tera_utils.egg-info/
+-rw-rw-rw-   0        0        0      508 2023-07-29 07:21:50.000000 tera_utils-0.0.3/tera_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-07-29 07:21:50.000000 tera_utils-0.0.3/tera_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 07:21:50.000000 tera_utils-0.0.3/tera_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-29 07:21:50.000000 tera_utils-0.0.3/tera_utils.egg-info/top_level.txt
```

### Comparing `tera_utils-0.0.2/LICENSE.md` & `tera_utils-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tera_utils-0.0.2/README.md` & `tera_utils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tera_utils-0.0.2/setup.py` & `tera_utils-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Utils for fun"
 LONG_DESCRIPTION = "A package made for fun and education"
 
 # Setting up
 setup(
     name="tera_utils",
     version=VERSION,
```

### Comparing `tera_utils-0.0.2/tera_utils/consol.py` & `tera_utils-0.0.3/tera_utils/consol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 from .locals import ascii_chars as default_chars
 
 
-class Consol:
+class Ascii_text:
     def __init__(
         self,
         consol_width: int = 18,
         char_height: int = 7,
         char_width: int = 8,
         char_set: dict = default_chars,
     ) -> None:
@@ -15,22 +15,32 @@
         self.char_height = char_height
         self.char_width = char_width
         self.char_set = char_set
 
         # Debug settings
         self.debug_mode = False
 
+    def split_text_into_lines(self, text: str, max_width: int) -> list:
+        """Creates a list with the same amount of elements as lines needed to print text.
+
+        Args:
+            text (str): The text you want to print
+            max_width (int): The amount of characters allowed in one line
+
+        Returns:
+            list: a list with the same amount of elements inside that are needed to print a line without warping.
+        """
+        return list(range(math.ceil(len(text) / self.consol_width)))
+
     def render(self, text: str):
         """Turns 'text' into a consol.print()-able list"""
 
-        new_line_idx = list(range(math.ceil(len(text) / self.consol_width)))
-
         self.lines = []
 
-        for line_idx in new_line_idx:
+        for line_idx in self.split_text_into_lines(text, self.consol_width):
             txt_len = len(text)
             chars_to_print = line_idx * self.consol_width
 
             if "\n" in text:
                 # TODO Handle newline characters in text
                 # ! TEMP CODE
                 start = line_idx * self.consol_width
@@ -90,9 +100,9 @@
 if __name__ == "__main__":
     from terminal import getTerminalSize
 
     tw, th = getTerminalSize()
 
     chars_per_line = tw // 8
 
-    consol = Consol(chars_per_line, 7, 8)
+    consol = Ascii_text(chars_per_line, 7, 8)
     consol.render("Hello World! This is my own text to ASCII renderer, 0123456789")
```

### Comparing `tera_utils-0.0.2/tera_utils/locals.py` & `tera_utils-0.0.3/tera_utils/locals.py`

 * *Files identical despite different names*

### Comparing `tera_utils-0.0.2/tera_utils/search.py` & `tera_utils-0.0.3/tera_utils/search.py`

 * *Files identical despite different names*

### Comparing `tera_utils-0.0.2/tera_utils/sort.py` & `tera_utils-0.0.3/tera_utils/sort.py`

 * *Files identical despite different names*

### Comparing `tera_utils-0.0.2/tera_utils/terminal.py` & `tera_utils-0.0.3/tera_utils/terminal.py`

 * *Files identical despite different names*

