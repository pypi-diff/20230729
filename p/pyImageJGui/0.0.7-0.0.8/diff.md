# Comparing `tmp/pyimagejgui-0.0.7.tar.gz` & `tmp/pyimagejgui-0.0.8.tar.gz`

## Comparing `pyimagejgui-0.0.7.tar` & `pyimagejgui-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/init.bat
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/init.sh
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/requirements.txt
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/angle.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/circle.svg
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/clear.svg
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/elliptical.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/file.svg
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/freehand.svg
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/hand.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/line.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/magnifier.svg
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/polygon.svg
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/rectangle.svg
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/rotate.svg
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/save.svg
--rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/style/main.qss
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/style/qssloader.py
--rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/AngleRoi.py
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/CircleRoi.py
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/EllipseRoi.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/LineRoi.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/RectangleRoi.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/constant.py
--rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/gui.py
--rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/imageView.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/utils/function.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/LICENSE
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/README.md
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/init.bat
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/init.sh
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/requirements.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/angle.svg
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/circle.svg
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/clear.svg
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/elliptical.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/file.svg
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/freehand.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/hand.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/line.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/magnifier.svg
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/polygon.svg
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/rectangle.svg
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/rotate.svg
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/icon/save.svg
+-rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/style/main.qss
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/style/qssloader.py
+-rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/AngleRoi.py
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/CircleRoi.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/EllipseRoi.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/LineRoi.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/RectangleRoi.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/constant.py
+-rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/gui.py
+-rw-r--r--   0        0        0    15058 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/ui/imageView.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/src/pyImageJGui/utils/function.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/LICENSE
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/README.md
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyimagejgui-0.0.8/PKG-INFO
```

### Comparing `pyimagejgui-0.0.7/main.py` & `pyimagejgui-0.0.8/main.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/.github/workflows/python-publish.yml` & `pyimagejgui-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/angle.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/angle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/clear.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/clear.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/elliptical.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/elliptical.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/file.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/file.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/freehand.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/freehand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/hand.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/hand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/magnifier.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/magnifier.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/polygon.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/polygon.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/rectangle.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/rectangle.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/rotate.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/rotate.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/icon/save.svg` & `pyimagejgui-0.0.8/src/pyImageJGui/icon/save.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/style/main.qss` & `pyimagejgui-0.0.8/src/pyImageJGui/style/main.qss`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/ui/AngleRoi.py` & `pyimagejgui-0.0.8/src/pyImageJGui/ui/AngleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/ui/CircleRoi.py` & `pyimagejgui-0.0.8/src/pyImageJGui/ui/CircleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/ui/EllipseRoi.py` & `pyimagejgui-0.0.8/src/pyImageJGui/ui/EllipseRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/ui/LineRoi.py` & `pyimagejgui-0.0.8/src/pyImageJGui/ui/LineRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/ui/RectangleRoi.py` & `pyimagejgui-0.0.8/src/pyImageJGui/ui/RectangleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/ui/gui.py` & `pyimagejgui-0.0.8/src/pyImageJGui/ui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,20 +127,15 @@
         elif sender.roi == ROI.Angle:
             self.figure.setDragMode(QGraphicsView.DragMode.NoDrag)
             self.figure.mouseMoveEvent = self.figure.mouseMoveAngleEvent
             self.figure.mousePressEvent = self.figure.mousePressAngleEvent
             self.figure.mouseReleaseEvent = self.figure.mouseReleaseAngleEvent
 
     def clear_btn_click(self):
-        for item in self.figure.scene.items():
-            if isinstance(item, QGraphicsPixmapItem):
-                continue
-            self.figure.scene.removeItem(item)
-
-        self.figure.roi = None
+        self.figure.clear()
 
     def measure_btn_click(self):
         dialog = QDialog(self)
         dialog.setWindowModality(Qt.WindowModality.ApplicationModal)
         dialog.setWindowTitle("ROI Datas")
         dialog.setMinimumSize(QSize(900, 100))
         layout = QVBoxLayout(dialog)
```

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/ui/imageView.py` & `pyimagejgui-0.0.8/src/pyImageJGui/ui/imageView.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,34 +55,50 @@
         self.handle_index = None
         self.mouseMoveEvent = self.mouseMoveEventNoRoi
         self.setFocusPolicy(Qt.FocusPolicy.StrongFocus)
         self.initScale = None
         self.points = []
         self.pressed_keys = []
 
+    def clear(self):
+        self.roi = None
+        self.roi_select_status = None
+        self.handle_move_status = None
+        self.roi_move_status = None
+        self.start_pos = None
+        self.init_point = None
+        self.handle_index = None
+        self.points = []
+        self.pressed_keys = []
+        for item in self.scene.items():
+            if not isinstance(item, QGraphicsPixmapItem):
+                self.scene.removeItem(item)
+
     def setImage(self, image):
         # 设置图像
         self.image = image
         pixmap = QPixmap.fromImage(self.image)
         self.pixmap_item.setPixmap(pixmap)
         self.scene.setSceneRect(pixmap.rect())
         self.fitInView(self.scene.sceneRect(), Qt.AspectRatioMode.KeepAspectRatio)
         self.initScale = self.transform().m11()
+        self.clear()
 
     def setImageNoQImage(self, img):
         height, width = img.shape
         img1 = QImage(img, width, height, width, QImage.Format.Format_Grayscale8)
         self.setImage(img1)
 
     def setPixmap(self, pix: QPixmap):
         self.image = pix.toImage()
         self.pixmap_item.setPixmap(pix)
         self.scene.setSceneRect(pix.rect())
         self.fitInView(self.scene.sceneRect(), Qt.AspectRatioMode.KeepAspectRatio)
         self.initScale = self.transform().m11()
+        self.clear()
 
     def wheelEvent(self, event):
         # 实现缩放
         if self.image is None:
             return
         mouse_point = self.mapToScene(event.position().toPoint())
         width = self.viewport().width()
```

### Comparing `pyimagejgui-0.0.7/src/pyImageJGui/utils/function.py` & `pyimagejgui-0.0.8/src/pyImageJGui/utils/function.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/LICENSE` & `pyimagejgui-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.7/pyproject.toml` & `pyimagejgui-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyImageJGui"
-version = "0.0.7"
+version = "0.0.8"
 description = "Python for ImageJ GUI"
 authors = [{name = "sdb", email = "sdb20200101@gmail.com"}]
 readme = "README.md"
 keywords = ["imagej", "GUI", "PySide6"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `pyimagejgui-0.0.7/PKG-INFO` & `pyimagejgui-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyImageJGui
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python for ImageJ GUI
 Project-URL: homepage, https://github.com/aghb123/pyImageJGui
 Author-email: sdb <sdb20200101@gmail.com>
 License-File: LICENSE
 Keywords: GUI,PySide6,imagej
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

