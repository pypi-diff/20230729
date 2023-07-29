# Comparing `tmp/qtdraw-1.1.3.tar.gz` & `tmp/qtdraw-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdraw-1.1.3.tar", last modified: Fri Jun  2 12:21:43 2023, max compression
+gzip compressed data, was "qtdraw-1.1.4.tar", last modified: Sat Jul 29 13:53:24 2023, max compression
```

## Comparing `qtdraw-1.1.3.tar` & `qtdraw-1.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-02 12:21:43.646964 qtdraw-1.1.3/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.3/LICENSE
--rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.3/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2447 2023-06-02 12:21:43.647057 qtdraw-1.1.3/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     2067 2023-05-26 12:13:57.000000 qtdraw-1.1.3/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-02 12:21:43.640911 qtdraw-1.1.3/qtdraw/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2023-05-29 09:26:27.000000 qtdraw-1.1.3/qtdraw/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-02 12:21:43.645975 qtdraw-1.1.3/qtdraw/core/
--rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/core/basic_object.py
--rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/color_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/core/color_palette.py
--rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/default_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/core/dialog_about.py
--rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/dialog_preference.py
--rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/core/editable_widget.py
--rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/group_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/group_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/group_tab.py
--rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/group_view.py
--rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/core/line_edit.py
--rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/core/pixmap_converter.py
--rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/qt_logging.py
--rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/qtdraw.png
--rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/qtdraw.ui
--rw-r--r--   0 hiro       (501) staff       (20)    17478 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/table_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/tree_item.py
--rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.3/qtdraw/core/tree_item_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     7499 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/core/util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/core/validator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-02 12:21:43.646627 qtdraw-1.1.3/qtdraw/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)    46964 2023-05-15 12:36:33.000000 qtdraw-1.1.3/qtdraw/multipie/dialog_group.py
--rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.3/qtdraw/multipie/dialog_group_info.py
--rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/multipie/setting.py
--rw-------   0 hiro       (501) staff       (20)    92079 2023-05-20 07:09:31.000000 qtdraw-1.1.3/qtdraw/qt_draw.py
--rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.3/qtdraw/qt_draw_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-02 12:21:43.646801 qtdraw-1.1.3/qtdraw/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.3/qtdraw/scripts/qtdraw.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-02 12:21:43.641746 qtdraw-1.1.3/qtdraw.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2447 2023-06-02 12:21:43.000000 qtdraw-1.1.3/qtdraw.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1002 2023-06-02 12:21:43.000000 qtdraw-1.1.3/qtdraw.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-06-02 12:21:43.000000 qtdraw-1.1.3/qtdraw.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       53 2023-06-02 12:21:43.000000 qtdraw-1.1.3/qtdraw.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)      102 2023-06-02 12:21:43.000000 qtdraw-1.1.3/qtdraw.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        7 2023-06-02 12:21:43.000000 qtdraw-1.1.3/qtdraw.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      726 2023-06-02 12:21:43.647450 qtdraw-1.1.3/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.3/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.769204 qtdraw-1.1.4/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.4/LICENSE
+-rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.4/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2464 2023-07-29 13:53:24.769289 qtdraw-1.1.4/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     2084 2023-07-29 13:47:38.000000 qtdraw-1.1.4/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.762182 qtdraw-1.1.4/qtdraw/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-29 10:18:46.000000 qtdraw-1.1.4/qtdraw/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.767976 qtdraw-1.1.4/qtdraw/core/
+-rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/basic_object.py
+-rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/color_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/color_palette.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/default_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/dialog_about.py
+-rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/dialog_preference.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/editable_widget.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_tab.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_view.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/line_edit.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/pixmap_converter.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/qt_logging.py
+-rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/qtdraw.png
+-rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/qtdraw.ui
+-rw-r--r--   0 hiro       (501) staff       (20)    17478 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/table_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/tree_item.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.4/qtdraw/core/tree_item_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.4/qtdraw/core/util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/validator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.768862 qtdraw-1.1.4/qtdraw/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.4/qtdraw/multipie/dialog_group.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.4/qtdraw/multipie/dialog_group_info.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/multipie/setting.py
+-rw-------   0 hiro       (501) staff       (20)    92079 2023-05-20 07:09:31.000000 qtdraw-1.1.4/qtdraw/qt_draw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/qt_draw_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.769035 qtdraw-1.1.4/qtdraw/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.4/qtdraw/scripts/qtdraw.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.763172 qtdraw-1.1.4/qtdraw.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2464 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1002 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      102 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      726 2023-07-29 13:53:24.769758 qtdraw-1.1.4/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.4/setup.py
```

### Comparing `qtdraw-1.1.3/LICENSE` & `qtdraw-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/PKG-INFO` & `qtdraw-1.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: qtdraw
-Version: 1.1.3
-Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
-Home-page: https://github.com/CMT-MU/QtDraw
-Author: Hiroaki Kusunose
-Author-email: hiroaki.kusunose@gmail.com
-License: MIT
-Keywords: pyvista,qtpy5
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # QtDraw
 
 3D drawing tool for molecules and crystals based on [PyVista](https://docs.pyvista.org/) and [Qt](https://www.riverbankcomputing.com/static/Docs/PyQt5/#).
 Drawings are associated with crystallographic symmetry operations provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Installation
 
@@ -63,8 +49,9 @@
 
 ## Requirements
 - This library requires [TeXLive](https://www.tug.org/texlive/) environment.
 - Symmetry operation supports are provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Documentation
 
-Refer to the [documentation](https://cmt-mu.github.io/QtDraw/) for detailed installation and usage details.
+Refer to the [documentation](https://cmt-mu.github.io/QtDraw/) for installation and usage.
+See also, [Manual](./manual.pdf).
```

### Comparing `qtdraw-1.1.3/qtdraw/core/basic_object.py` & `qtdraw-1.1.4/qtdraw/core/basic_object.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/color_dialog.py` & `qtdraw-1.1.4/qtdraw/core/color_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/color_palette.py` & `qtdraw-1.1.4/qtdraw/core/color_palette.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/default_panel.ui` & `qtdraw-1.1.4/qtdraw/core/default_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/dialog_about.py` & `qtdraw-1.1.4/qtdraw/core/dialog_about.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/dialog_preference.py` & `qtdraw-1.1.4/qtdraw/core/dialog_preference.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/editable_widget.py` & `qtdraw-1.1.4/qtdraw/core/editable_widget.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/group_model.py` & `qtdraw-1.1.4/qtdraw/core/group_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/group_panel.ui` & `qtdraw-1.1.4/qtdraw/core/group_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/group_tab.py` & `qtdraw-1.1.4/qtdraw/core/group_tab.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/group_view.py` & `qtdraw-1.1.4/qtdraw/core/group_view.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/line_edit.py` & `qtdraw-1.1.4/qtdraw/core/line_edit.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/pixmap_converter.py` & `qtdraw-1.1.4/qtdraw/core/pixmap_converter.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/qt_logging.py` & `qtdraw-1.1.4/qtdraw/core/qt_logging.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/qtdraw.png` & `qtdraw-1.1.4/qtdraw/core/qtdraw.png`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/qtdraw.ui` & `qtdraw-1.1.4/qtdraw/core/qtdraw.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/setting.py` & `qtdraw-1.1.4/qtdraw/core/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/table_dialog.py` & `qtdraw-1.1.4/qtdraw/core/table_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/tree_item.py` & `qtdraw-1.1.4/qtdraw/core/tree_item.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/tree_item_model.py` & `qtdraw-1.1.4/qtdraw/core/tree_item_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/core/util.py` & `qtdraw-1.1.4/qtdraw/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import vtk
-from pyvista._vtk import vtkParametricSpline
+from vtk import vtkParametricSpline
 import pyvista as pv
 from pyvista.utilities import surface_from_para
 from qtpy.QtWidgets import QApplication, QStyleFactory
 from gcoreutils.nsarray import NSArray
 from gcoreutils.latex_util import latex_setting
 from qtdraw.core.setting import rcParams
 from qtdraw.core.color_palette import custom_colormap, all_colors
```

### Comparing `qtdraw-1.1.3/qtdraw/core/validator.py` & `qtdraw-1.1.4/qtdraw/core/validator.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/multipie/dialog_group.py` & `qtdraw-1.1.4/qtdraw/multipie/dialog_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -682,14 +682,20 @@
         orbital_proj_rank = QComboBox(self)
         orbital_proj_rank.setFocusPolicy(Qt.NoFocus)
         orbital_proj_rank.addItems(map(str, range(12)))
         orbital_proj_rank.setCurrentIndex(0)
         orbital_proj_draw_button = QPushButton("draw", self)
         orbital_proj_draw_button.setFocusPolicy(Qt.NoFocus)
 
+        hopping_proj_label = QLabel(
+            "HOPPING (imag)\ne.g., [0,0,0];[1/2,1/2,0] (bond)",
+            self,
+        )
+        hopping_proj_pos = QLineEdit("[0, 0, 0]; [1/2, 1/2, 0]", self)
+
         tab2_v_spacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         tab2_grid = QGridLayout(self.tab2)
 
         tab2_grid.addWidget(site_proj_label, 0, 0, 1, 9)
         tab2_grid.addWidget(site_proj_pos, 1, 0, 1, 7)
         tab2_grid.addWidget(site_proj_label1, 2, 0, 1, 1)
@@ -715,15 +721,18 @@
         tab2_grid.addWidget(orbital_proj_type, 10, 7, 1, 1)
         tab2_grid.addWidget(orbital_proj_rank, 10, 8, 1, 1)
         tab2_grid.addWidget(orbital_proj_label1, 11, 0, 1, 1)
         tab2_grid.addWidget(orbital_proj_type1, 11, 1, 1, 1)
         tab2_grid.addWidget(orbital_proj_irrep1, 11, 2, 1, 6)
         tab2_grid.addWidget(orbital_proj_draw_button, 11, 8, 1, 1)
 
-        tab2_grid.addItem(tab2_v_spacer, 12, 1, 1, 1)
+        tab2_grid.addWidget(hopping_proj_label, 12, 0, 1, 9)
+        tab2_grid.addWidget(hopping_proj_pos, 13, 0, 1, 9)
+
+        tab2_grid.addItem(tab2_v_spacer, 14, 1, 1, 1)
 
         show_lbl = rcParams["show_label"]
 
         # --- plot site_cluster SAMB ---
         def gen_site_cluster():
             combined_info = self._create_combined(site_proj_pos.text(), 0, "Q")
             if combined_info is None:
@@ -927,18 +936,35 @@
             self.tab2_vector_proj_c_samb, self.tab2_vector_proj_site, self.tab2_vector_proj_z_samb = combined_info
 
             select_z_samb_vector()
 
         def select_z_samb_vector():
             self.tab2_vector_proj_comb_select = self.tab2_vector_proj_z_samb[vector_proj_type1.currentText()]
             vector_proj_irrep1.clear()
-            comb = [self._combined_format(i) for i in self.tab2_vector_proj_comb_select]
+            comb = [i[0] for i in self.tab2_vector_proj_comb_select]
             vector_proj_irrep1.addItems(comb)
             vector_proj_irrep1.setCurrentIndex(0)
 
+        def plot_vector_object(site, obj, rep, pname, label, color):
+            if self.n_pset == 1:
+                for s, c in zip(site, obj):
+                    if c != 0:
+                        c = str(c.subs(rep).T[:])
+                        c = NSArray(c)
+                        d = c.norm()
+                        self._qtdraw.plot_vector(s, c, length=d, color=color, name=pname, label=label, show_lbl=show_lbl)
+            else:
+                for p in self._group.symmetry_operation.plus_set:
+                    for s, c in zip(site, obj):
+                        if c != 0:
+                            c = str(c.subs(rep).T[:])
+                            c = NSArray(c)
+                            d = c.norm()
+                            self._qtdraw.plot_vector(s + p, c, length=d, color=color, name=pname, label=label, show_lbl=show_lbl)
+
         def plot_z_samb_vector():
             irrep = vector_proj_irrep1.currentIndex()
             try:
                 eq = self.tab2_vector_proj_comb_select[irrep][1]
             except (IndexError, AttributeError):
                 return
             cluster_obj = NSArray(str([0] * len(self.tab2_vector_proj_site)))
@@ -953,29 +979,16 @@
                 cluster_obj *= -sp.I
 
             rep = {v[0]: sp.Matrix([1, 0, 0]), v[1]: sp.Matrix([0, 1, 0]), v[2]: sp.Matrix([0, 0, 1])}
             color = rcParams["vector_color_" + vector_proj_type.currentText()]
             self._qtdraw._close_dialog()
             lbl = vector_proj_irrep1.currentText().replace("(", "[").replace(")", "]")
             pname = "Z_" + self._qtdraw._get_name("vector")
-            if self.n_pset == 1:
-                for s, c in zip(self.tab2_vector_proj_site, cluster_obj):
-                    if c != 0:
-                        c = str(c.subs(rep).T[:])
-                        c = NSArray(c)
-                        d = c.norm()
-                        self._qtdraw.plot_vector(s, c, length=d, color=color, name=pname, label=lbl, show_lbl=show_lbl)
-            else:
-                for p in self._group.symmetry_operation.plus_set:
-                    for s, c in zip(self.tab2_vector_proj_site, cluster_obj):
-                        if c != 0:
-                            c = str(c.subs(rep).T[:])
-                            c = NSArray(c)
-                            d = c.norm()
-                            self._qtdraw.plot_vector(s + p, c, length=d, color=color, name=pname, label=lbl, show_lbl=show_lbl)
+
+            plot_vector_object(self.tab2_vector_proj_site, cluster_obj, rep, pname, lbl, color)
 
             self._qtdraw._plot_all_object()
 
         vector_proj_pos.returnPressed.connect(gen_z_samb_vector)
         vector_proj_type1.currentIndexChanged.connect(select_z_samb_vector)
         vector_proj_draw_button.clicked.connect(plot_z_samb_vector)
 
@@ -990,77 +1003,115 @@
             self.tab2_orbital_proj_c_samb, self.tab2_orbital_proj_site, self.tab2_orbital_proj_z_samb = combined_info
 
             select_z_samb_orbital()
 
         def select_z_samb_orbital():
             self.tab2_orbital_proj_comb_select = self.tab2_orbital_proj_z_samb[orbital_proj_type1.currentText()]
             orbital_proj_irrep1.clear()
-            comb = [self._combined_format(i) for i in self.tab2_orbital_proj_comb_select]
+            comb = [i[0] for i in self.tab2_orbital_proj_comb_select]
             orbital_proj_irrep1.addItems(comb)
             orbital_proj_irrep1.setCurrentIndex(0)
 
-        def plot_z_samb_orbital():
-            irrep = orbital_proj_irrep1.currentIndex()
-            try:
-                eq = self.tab2_orbital_proj_comb_select[irrep][1]
-            except (IndexError, AttributeError):
-                return
-            cluster_obj = NSArray(str([0] * len(self.tab2_orbital_proj_site)))
-            for i in eq:
-                coeff, tag_h, tag_c = i
-                harm = self._pgroup.harmonics[tag_h].expression()
-                cluster = self.tab2_orbital_proj_c_samb[tag_c]
-                cluster_obj += coeff * harm * cluster
-            if self._different_time_reversal(orbital_proj_type.currentText(), orbital_proj_type1.currentText()):
-                cluster_obj *= -sp.I
-
-            self._qtdraw._close_dialog()
-            color = rcParams["orbital_color_" + orbital_proj_type.currentText()]
-            lbl = orbital_proj_irrep1.currentText().replace("(", "[").replace(")", "]")
-            pname = "Z_" + self._qtdraw._get_name("orbital")
+        def plot_orbital_object(site, obj, pname, label, color):
             if self.n_pset == 1:
-                for s, orb in zip(self.tab2_orbital_proj_site, cluster_obj):
+                for s, orb in zip(site, obj):
                     self._qtdraw.plot_orbital(
                         s,
                         orb,
                         size=0.6,
                         scale=False,
                         color=color,
                         name=pname,
-                        label=lbl,
+                        label=label,
                         show_lbl=show_lbl,
                     )
             else:
                 for p in self._group.symmetry_operation.plus_set:
-                    for s, orb in zip(self.tab2_orbital_proj_site, cluster_obj):
+                    for s, orb in zip(site, obj):
                         self._qtdraw.plot_orbital(
                             s + p,
                             orb,
                             size=0.6,
                             scale=False,
                             color=color,
                             name=pname,
-                            label=lbl,
+                            label=label,
                             show_lbl=show_lbl,
                         )
+
+        def plot_z_samb_orbital():
+            irrep = orbital_proj_irrep1.currentIndex()
+            try:
+                eq = self.tab2_orbital_proj_comb_select[irrep][1]
+            except (IndexError, AttributeError):
+                return
+            cluster_obj = NSArray(str([0] * len(self.tab2_orbital_proj_site)))
+            for i in eq:
+                coeff, tag_h, tag_c = i
+                harm = self._pgroup.harmonics[tag_h].expression()
+                cluster = self.tab2_orbital_proj_c_samb[tag_c]
+                cluster_obj += coeff * harm * cluster
+            if self._different_time_reversal(orbital_proj_type.currentText(), orbital_proj_type1.currentText()):
+                cluster_obj *= -sp.I
+
+            self._qtdraw._close_dialog()
+            color = rcParams["orbital_color_" + orbital_proj_type.currentText()]
+            lbl = orbital_proj_irrep1.currentText().replace("(", "[").replace(")", "]")
+            pname = "Z_" + self._qtdraw._get_name("orbital")
+
+            plot_orbital_object(self.tab2_orbital_proj_site, cluster_obj, pname, lbl, color)
+
             self._qtdraw._plot_all_object()
 
         orbital_proj_pos.returnPressed.connect(gen_z_samb_orbital)
         orbital_proj_type1.currentIndexChanged.connect(select_z_samb_orbital)
         orbital_proj_draw_button.clicked.connect(plot_z_samb_orbital)
 
+        # --- plot hopping ---
+        def plot_z_samb_hopping():
+            combined_info = self._create_combined(hopping_proj_pos.text(), 1, "T")
+            if combined_info is None:
+                return
+
+            c_samb, site, z_samb = combined_info
+
+            try:
+                eq = z_samb["Q"][0][1]
+            except (IndexError, AttributeError):
+                return
+            cluster_obj = NSArray(str([0] * len(site)))
+            v = NSArray.vector3d()
+
+            for coeff, tag_h, tag_c in eq:
+                harm = self._pgroup.harmonics[tag_h].expression(v=v)
+                cluster = c_samb[tag_c]
+                cluster_obj += coeff * harm * cluster
+
+            cluster_obj *= -sp.I
+
+            rep = {v[0]: sp.Matrix([1, 0, 0]), v[1]: sp.Matrix([0, 1, 0]), v[2]: sp.Matrix([0, 0, 1])}
+            color = rcParams["vector_color_T"]
+            self._qtdraw._close_dialog()
+            lbl = "t_imag"
+            pname = "Z_" + self._qtdraw._get_name("vector")
+
+            plot_vector_object(site, cluster_obj, rep, pname, lbl, color)
+
+            self._qtdraw._plot_all_object()
+
+        hopping_proj_pos.returnPressed.connect(plot_z_samb_hopping)
+
     # ==================================================
     def _different_time_reversal(self, t1, t2):
         tp = {"Q": "E", "G": "E", "T": "M", "M": "M"}
         return tp[t1] != tp[t2]
 
     # ==================================================
     def _combined_format(self, tag_list):
-        z_tag = tag_list[0]
-        _, x_tag, y_tag = tag_list[1][0]
+        z_tag, x_tag, y_tag = tag_list
         t1 = (",".join(str(x_tag).split(",")[:-1]) + ")").replace("h", "a")
         t2 = ",".join(str(y_tag).split(",")[:-1]) + ")"
         tag = f"{z_tag} = {t1} x {t2}"
         return tag
 
     # ==================================================
     def _create_combined(self, site_bond, harm_rank, harm_head, ret_bond=False):
@@ -1084,13 +1135,13 @@
         x_tag = self._pgroup.harmonics.key_list().select(rank=int(harm_rank), head=t_rev[harm_head])
         if harm_head in ["T", "M"]:
             x_tag = [tag.reverse_t_type() for tag in x_tag]
         y_tag = list(c_samb.keys())
         z_samb_all = self._group.z_samb(x_tag, y_tag)
         z_samb = {"Q": [], "G": [], "T": [], "M": []}
         for tag, c in z_samb_all.items():
-            tag = tag[0]
-            z_samb[tag.head].append((tag, c))
+            tag_str = self._combined_format(tag)
+            z_samb[tag[0].head].append((tag_str, c))
         for k in z_samb.keys():
             z_samb[k] = list(sorted(z_samb[k], key=lambda i: i[0]))
 
         return c_samb, site, z_samb
```

### Comparing `qtdraw-1.1.3/qtdraw/multipie/dialog_group_info.py` & `qtdraw-1.1.4/qtdraw/multipie/dialog_group_info.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/multipie/setting.py` & `qtdraw-1.1.4/qtdraw/multipie/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/qt_draw.py` & `qtdraw-1.1.4/qtdraw/qt_draw.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw/qt_draw_base.py` & `qtdraw-1.1.4/qtdraw/qt_draw_base.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/qtdraw.egg-info/PKG-INFO` & `qtdraw-1.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.3
+Version: 1.1.4
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
@@ -63,8 +63,9 @@
 
 ## Requirements
 - This library requires [TeXLive](https://www.tug.org/texlive/) environment.
 - Symmetry operation supports are provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Documentation
 
-Refer to the [documentation](https://cmt-mu.github.io/QtDraw/) for detailed installation and usage details.
+Refer to the [documentation](https://cmt-mu.github.io/QtDraw/) for installation and usage.
+See also, [Manual](./manual.pdf).
```

### Comparing `qtdraw-1.1.3/qtdraw.egg-info/SOURCES.txt` & `qtdraw-1.1.4/qtdraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.3/setup.cfg` & `qtdraw-1.1.4/setup.cfg`

 * *Files identical despite different names*

