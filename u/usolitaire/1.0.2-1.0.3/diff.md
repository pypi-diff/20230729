# Comparing `tmp/usolitaire-1.0.2.tar.gz` & `tmp/usolitaire-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usolitaire-1.0.2.tar", last modified: Thu Jul 27 22:14:42 2023, max compression
+gzip compressed data, was "usolitaire-1.0.3.tar", last modified: Fri Jul 28 23:30:10 2023, max compression
```

## Comparing `usolitaire-1.0.2.tar` & `usolitaire-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 22:14:42.177679 usolitaire-1.0.2/
--rw-rw-r--   0 elias     (1000) elias     (1000)     1074 2023-07-23 16:38:34.000000 usolitaire-1.0.2/LICENSE
--rw-rw-r--   0 elias     (1000) elias     (1000)      105 2023-07-27 12:52:48.000000 usolitaire-1.0.2/MANIFEST.in
--rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 22:14:42.177679 usolitaire-1.0.2/PKG-INFO
--rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-27 12:36:19.000000 usolitaire-1.0.2/README.rst
--rw-rw-r--   0 elias     (1000) elias     (1000)       29 2023-07-27 12:14:41.000000 usolitaire-1.0.2/pyproject.toml
--rw-rw-r--   0 elias     (1000) elias     (1000)      404 2023-07-27 22:14:42.177679 usolitaire-1.0.2/setup.cfg
--rw-rw-r--   0 elias     (1000) elias     (1000)     1282 2023-07-27 22:14:26.000000 usolitaire-1.0.2/setup.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 22:14:42.177679 usolitaire-1.0.2/usolitaire/
--rw-rw-r--   0 elias     (1000) elias     (1000)      119 2023-07-27 22:14:26.000000 usolitaire-1.0.2/usolitaire/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)    12099 2023-07-27 21:58:54.000000 usolitaire-1.0.2/usolitaire/app.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2052 2023-07-27 21:42:22.000000 usolitaire-1.0.2/usolitaire/card_render.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     8662 2023-07-27 12:15:26.000000 usolitaire-1.0.2/usolitaire/game.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      775 2023-07-27 21:42:22.000000 usolitaire-1.0.2/usolitaire/textual_app.css
--rw-rw-r--   0 elias     (1000) elias     (1000)     7543 2023-07-27 16:37:59.000000 usolitaire-1.0.2/usolitaire/textual_ui.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 22:14:42.177679 usolitaire-1.0.2/usolitaire.egg-info/
--rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 22:14:42.000000 usolitaire-1.0.2/usolitaire.egg-info/PKG-INFO
--rw-rw-r--   0 elias     (1000) elias     (1000)      441 2023-07-27 22:14:42.000000 usolitaire-1.0.2/usolitaire.egg-info/SOURCES.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 22:14:42.000000 usolitaire-1.0.2/usolitaire.egg-info/dependency_links.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       51 2023-07-27 22:14:42.000000 usolitaire-1.0.2/usolitaire.egg-info/entry_points.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 22:14:42.000000 usolitaire-1.0.2/usolitaire.egg-info/not-zip-safe
--rw-rw-r--   0 elias     (1000) elias     (1000)        8 2023-07-27 22:14:42.000000 usolitaire-1.0.2/usolitaire.egg-info/requires.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-07-27 22:14:42.000000 usolitaire-1.0.2/usolitaire.egg-info/top_level.txt
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-28 23:30:10.981937 usolitaire-1.0.3/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1074 2023-07-23 16:38:34.000000 usolitaire-1.0.3/LICENSE
+-rw-rw-r--   0 elias     (1000) elias     (1000)      105 2023-07-27 12:52:48.000000 usolitaire-1.0.3/MANIFEST.in
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-28 23:30:10.981937 usolitaire-1.0.3/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-27 12:36:19.000000 usolitaire-1.0.3/README.rst
+-rw-rw-r--   0 elias     (1000) elias     (1000)       29 2023-07-27 12:14:41.000000 usolitaire-1.0.3/pyproject.toml
+-rw-rw-r--   0 elias     (1000) elias     (1000)      404 2023-07-28 23:30:10.981937 usolitaire-1.0.3/setup.cfg
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1282 2023-07-28 23:29:58.000000 usolitaire-1.0.3/setup.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-28 23:30:10.981937 usolitaire-1.0.3/usolitaire/
+-rw-rw-r--   0 elias     (1000) elias     (1000)      119 2023-07-28 23:29:58.000000 usolitaire-1.0.3/usolitaire/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)    12204 2023-07-28 23:28:02.000000 usolitaire-1.0.3/usolitaire/app.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2052 2023-07-27 21:42:22.000000 usolitaire-1.0.3/usolitaire/card_render.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     8662 2023-07-27 12:15:26.000000 usolitaire-1.0.3/usolitaire/game.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      775 2023-07-27 21:42:22.000000 usolitaire-1.0.3/usolitaire/textual_app.css
+-rw-rw-r--   0 elias     (1000) elias     (1000)     7543 2023-07-27 16:37:59.000000 usolitaire-1.0.3/usolitaire/textual_ui.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-28 23:30:10.981937 usolitaire-1.0.3/usolitaire.egg-info/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)      441 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/SOURCES.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/dependency_links.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       51 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/entry_points.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/not-zip-safe
+-rw-rw-r--   0 elias     (1000) elias     (1000)        8 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/requires.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/top_level.txt
```

### Comparing `usolitaire-1.0.2/LICENSE` & `usolitaire-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.2/PKG-INFO` & `usolitaire-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usolitaire
-Version: 1.0.2
+Version: 1.0.3
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
 Keywords: usolitaire
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `usolitaire-1.0.2/README.rst` & `usolitaire-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.2/setup.py` & `usolitaire-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 requirements = [
     "textual",
 ]
 
 setup(
     name="usolitaire",
-    version="1.0.2",
+    version="1.0.3",
     description="Solitaire in your terminal",
     long_description=readme,
     author="Elias Dorneles",
     author_email="eliasdorneles@gmail.com",
     url="https://github.com/eliasdorneles/usolitaire",
     entry_points={
         "console_scripts": {
```

### Comparing `usolitaire-1.0.2/usolitaire/app.py` & `usolitaire-1.0.3/usolitaire/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,16 @@
                 self.refresh_foundations()
                 self.selected_card = None
                 self.highlight_selected_cards()
                 self._update_focus()
                 self.check_if_won()
         else:
             if not event.card.face_up:
+                if not self.game.tableau[event.pile_index][-1] == event.card:
+                    return
                 event.card.face_up = True
                 self.current_focus = FocusPosition(FocusRow.BOTTOM, event.pile_index)
                 self.refresh_tableau(event.pile_index)
                 self._update_focus()
                 return
 
             target_card = SelectedCardPosition(
```

### Comparing `usolitaire-1.0.2/usolitaire/card_render.py` & `usolitaire-1.0.3/usolitaire/card_render.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.2/usolitaire/game.py` & `usolitaire-1.0.3/usolitaire/game.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.2/usolitaire/textual_app.css` & `usolitaire-1.0.3/usolitaire/textual_app.css`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.2/usolitaire/textual_ui.py` & `usolitaire-1.0.3/usolitaire/textual_ui.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.2/usolitaire.egg-info/PKG-INFO` & `usolitaire-1.0.3/usolitaire.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usolitaire
-Version: 1.0.2
+Version: 1.0.3
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
 Keywords: usolitaire
 Classifier: Development Status :: 2 - Pre-Alpha
```

