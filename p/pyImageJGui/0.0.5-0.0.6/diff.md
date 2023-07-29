# Comparing `tmp/pyimagejgui-0.0.5.tar.gz` & `tmp/pyimagejgui-0.0.6.tar.gz`

## Comparing `pyimagejgui-0.0.5.tar` & `pyimagejgui-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/init.bat
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/init.sh
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/angle.svg
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/circle.svg
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/clear.svg
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/elliptical.svg
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/file.svg
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/freehand.svg
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/hand.svg
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/line.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/magnifier.svg
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/polygon.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/rectangle.svg
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/icon/rotate.svg
--rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/style/main.qss
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/style/qssloader.py
--rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/AngleRoi.py
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/CircleRoi.py
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/EllipseRoi.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/LineRoi.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/RectangleRoi.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/constant.py
--rw-r--r--   0        0        0    14275 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/imageView.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/src/pyImageJGui/ui/main_ui.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/README.md
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyimagejgui-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/init.bat
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/init.sh
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/angle.svg
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/circle.svg
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/clear.svg
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/elliptical.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/file.svg
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/freehand.svg
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/hand.svg
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/line.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/magnifier.svg
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/polygon.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/rectangle.svg
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/rotate.svg
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/save.svg
+-rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/style/main.qss
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/style/qssloader.py
+-rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/AngleRoi.py
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/CircleRoi.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/EllipseRoi.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/LineRoi.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/RectangleRoi.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/constant.py
+-rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/gui.py
+-rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/imageView.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/utils/function.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/LICENSE
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/README.md
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/PKG-INFO
```

### Comparing `pyimagejgui-0.0.5/main.py` & `pyimagejgui-0.0.6/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @File: main.py
 @Software : PyCharm
 """
 import multiprocessing
 import sys
 
 multiprocessing.freeze_support()
+from src.pyImageJGui.ui.gui import *
 from qt_material import apply_stylesheet
 from src.pyImageJGui.style.qssloader import style
 
 if __name__ == "__main__":
     app = QApplication([])
     window = QMainWindow()
     window.setMinimumSize(QSize(1200, 800))
```

### Comparing `pyimagejgui-0.0.5/.github/workflows/python-publish.yml` & `pyimagejgui-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/angle.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/angle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/circle.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/circle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/clear.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/clear.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/elliptical.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/elliptical.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/freehand.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/freehand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/hand.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/hand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/magnifier.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/magnifier.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/polygon.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/polygon.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/icon/rotate.svg` & `pyimagejgui-0.0.6/src/pyImageJGui/icon/rotate.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/style/main.qss` & `pyimagejgui-0.0.6/src/pyImageJGui/style/main.qss`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/ui/AngleRoi.py` & `pyimagejgui-0.0.6/src/pyImageJGui/ui/AngleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/ui/CircleRoi.py` & `pyimagejgui-0.0.6/src/pyImageJGui/ui/CircleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/ui/EllipseRoi.py` & `pyimagejgui-0.0.6/src/pyImageJGui/ui/EllipseRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/ui/LineRoi.py` & `pyimagejgui-0.0.6/src/pyImageJGui/ui/LineRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/ui/RectangleRoi.py` & `pyimagejgui-0.0.6/src/pyImageJGui/ui/RectangleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/src/pyImageJGui/ui/imageView.py` & `pyimagejgui-0.0.6/src/pyImageJGui/ui/imageView.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,21 @@
         self.initScale = self.transform().m11()
 
     def setImageNoQImage(self, img):
         height, width = img.shape
         img1 = QImage(img, width, height, width, QImage.Format.Format_Grayscale8)
         self.setImage(img1)
 
+    def setPixmap(self, pix: QPixmap):
+        self.image = pix.toImage()
+        self.pixmap_item.setPixmap(pix)
+        self.scene.setSceneRect(pix.rect())
+        self.fitInView(self.scene.sceneRect(), Qt.AspectRatioMode.KeepAspectRatio)
+        self.initScale = self.transform().m11()
+
     def wheelEvent(self, event):
         # 实现缩放
         if self.image is None:
             return
         mouse_point = self.mapToScene(event.position().toPoint())
         width = self.viewport().width()
         height = self.viewport().height()
```

### Comparing `pyimagejgui-0.0.5/LICENSE` & `pyimagejgui-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.5/pyproject.toml` & `pyimagejgui-0.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyImageJGui"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python for ImageJ GUI"
 authors = [{name = "sdb", email = "sdb20200101@gmail.com"}]
 readme = "README.md"
 keywords = ["imagej", "GUI", "PySide6"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -31,11 +31,12 @@
 ]
 
 requires-python = ">=3.8"
 dependencies = [
     "PySide6",
     "shapely",
     "opencv-python",
+    "numpy",
 ]
 
 [project.urls]
 homepage = "https://github.com/aghb123/pyImageJGui"
```

### Comparing `pyimagejgui-0.0.5/PKG-INFO` & `pyimagejgui-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyImageJGui
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python for ImageJ GUI
 Project-URL: homepage, https://github.com/aghb123/pyImageJGui
 Author-email: sdb <sdb20200101@gmail.com>
 License-File: LICENSE
 Keywords: GUI,PySide6,imagej
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,13 +21,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
+Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pyside6
 Requires-Dist: shapely
 Description-Content-Type: text/markdown
 
-# pyImageJGui
+# pyImageJGui
+
+This repository uses PySide6 to implement ImageJ's GUI functionality.
+
+Launch main.py to display image and select various types of ROI.
```

