# Comparing `tmp/pyimagejgui-0.0.6.tar.gz` & `tmp/pyimagejgui-0.0.7.tar.gz`

## Comparing `pyimagejgui-0.0.6.tar` & `pyimagejgui-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/init.bat
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/init.sh
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/angle.svg
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/circle.svg
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/clear.svg
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/elliptical.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/file.svg
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/freehand.svg
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/hand.svg
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/line.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/magnifier.svg
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/polygon.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/rectangle.svg
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/rotate.svg
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/icon/save.svg
--rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/style/main.qss
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/style/qssloader.py
--rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/AngleRoi.py
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/CircleRoi.py
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/EllipseRoi.py
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/LineRoi.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/RectangleRoi.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/constant.py
--rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/gui.py
--rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/ui/imageView.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/src/pyImageJGui/utils/function.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/LICENSE
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/README.md
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyimagejgui-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/init.bat
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/init.sh
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/angle.svg
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/circle.svg
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/clear.svg
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/elliptical.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/file.svg
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/freehand.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/hand.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/line.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/magnifier.svg
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/polygon.svg
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/rectangle.svg
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/rotate.svg
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/icon/save.svg
+-rwxr-xr-x   0        0        0     4254 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/style/main.qss
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/style/qssloader.py
+-rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/AngleRoi.py
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/CircleRoi.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/EllipseRoi.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/LineRoi.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/RectangleRoi.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/constant.py
+-rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/gui.py
+-rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/ui/imageView.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/src/pyImageJGui/utils/function.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/LICENSE
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/README.md
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyimagejgui-0.0.7/PKG-INFO
```

### Comparing `pyimagejgui-0.0.6/main.py` & `pyimagejgui-0.0.7/main.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/.github/workflows/python-publish.yml` & `pyimagejgui-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/icon/file.svg` & `pyimagejgui-0.0.7/src/pyImageJGui/icon/file.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/icon/freehand.svg` & `pyimagejgui-0.0.7/src/pyImageJGui/icon/freehand.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/icon/magnifier.svg` & `pyimagejgui-0.0.7/src/pyImageJGui/icon/magnifier.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/icon/polygon.svg` & `pyimagejgui-0.0.7/src/pyImageJGui/icon/polygon.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/icon/save.svg` & `pyimagejgui-0.0.7/src/pyImageJGui/icon/save.svg`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/style/main.qss` & `pyimagejgui-0.0.7/src/pyImageJGui/style/main.qss`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/ui/AngleRoi.py` & `pyimagejgui-0.0.7/src/pyImageJGui/ui/AngleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/ui/CircleRoi.py` & `pyimagejgui-0.0.7/src/pyImageJGui/ui/CircleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/ui/EllipseRoi.py` & `pyimagejgui-0.0.7/src/pyImageJGui/ui/EllipseRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/ui/LineRoi.py` & `pyimagejgui-0.0.7/src/pyImageJGui/ui/LineRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/ui/RectangleRoi.py` & `pyimagejgui-0.0.7/src/pyImageJGui/ui/RectangleRoi.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/ui/gui.py` & `pyimagejgui-0.0.7/src/pyImageJGui/ui/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,22 +144,20 @@
         dialog.setWindowTitle("ROI Datas")
         dialog.setMinimumSize(QSize(900, 100))
         layout = QVBoxLayout(dialog)
         roi = self.figure.roi
         roi_table = QTableWidget()
         header = roi_table.horizontalHeader()
         header.setSectionResizeMode(QHeaderView.ResizeMode.Stretch)
-        # roi_table.insertRow(roi_table.rowCount())
+        roi_table.insertRow(roi_table.rowCount())
         layout.addWidget(roi_table)
         if isinstance(roi, RectangleRoi):
             roi_table.setColumnCount(7)
             roi_table.setHorizontalHeaderLabels(["Mean", "Min", "Max", "x", "y", "Width", "Height"])
 
-            roi_table.insertRow(roi_table.rowCount())
-
             rect = roi.rect().toRect()
 
             pix_roi = self.figure.pixmap_item.pixmap().copy(rect)
             arr = QPixmapToArray(pix_roi)
 
             Mean = round(np.mean(arr), 3)
             Max = np.max(arr)
@@ -178,16 +176,14 @@
             roi_table.setItem(roi_table.rowCount() - 1, 5, QTableWidgetItem(str(width)))
             roi_table.setItem(roi_table.rowCount() - 1, 6, QTableWidgetItem(str(height)))
 
         if isinstance(roi, CircleRoi):
             roi_table.setColumnCount(6)
             roi_table.setHorizontalHeaderLabels(["Mean", "Min", "Max", "cx", "cy", "Radius"])
 
-            roi_table.insertRow(roi_table.rowCount())
-
             rect = roi.rect().toRect()
 
             pix_roi = self.figure.pixmap_item.pixmap().copy(rect)
             arr = QPixmapToArray(pix_roi)
 
             mask = np.zeros_like(arr)
             h, w = arr.shape[:2]
@@ -212,16 +208,14 @@
             roi_table.setItem(roi_table.rowCount() - 1, 4, QTableWidgetItem(str(cy)))
             roi_table.setItem(roi_table.rowCount() - 1, 5, QTableWidgetItem(str(raduis)))
 
         if isinstance(roi, EllipseRoi):
             roi_table.setColumnCount(8)
             roi_table.setHorizontalHeaderLabels(["Mean", "Min", "Max", "Cx", "Cy", "Major", "Minor", "Ovality"])
 
-            roi_table.insertRow(roi_table.rowCount())
-
             cx = int(roi.rect().center().x())
             cy = int(roi.rect().center().y())
             major = int(roi.rect().width())
             minor = int(roi.rect().height())
             axis = [major, minor]
             ovality = round(abs(1 - min(axis) / max(axis)), 4)
 
@@ -251,30 +245,27 @@
             roi_table.setItem(roi_table.rowCount() - 1, 6, QTableWidgetItem(str(minor)))
             roi_table.setItem(roi_table.rowCount() - 1, 7, QTableWidgetItem(str(ovality)))
 
         if isinstance(roi, LineRoi):
             roi_table.setColumnCount(2)
             roi_table.setHorizontalHeaderLabels(["Length", "Angle"])
 
-            roi_table.insertRow(roi_table.rowCount())
-
             angle = roi.line().angle()
             if angle > 180:
                 angle = angle - 360
 
             angle = round(angle, 3)
 
             length = round(roi.line().length(), 3)
             roi_table.setItem(roi_table.rowCount() - 1, 0, QTableWidgetItem(str(length)))
             roi_table.setItem(roi_table.rowCount() - 1, 1, QTableWidgetItem(str(angle)))
 
         if isinstance(roi, AngleRoi):
             roi_table.setColumnCount(1)
             roi_table.setHorizontalHeaderLabels(["Angle"])
-            roi_table.insertRow(roi_table.rowCount())
 
             p1 = roi.p1.rect().center()
             p2 = roi.p2.rect().center()
             p3 = roi.p3.rect().center()
 
             x1 = p2.x() - p1.x()
             y1 = p2.y() - p1.y()
@@ -305,72 +296,57 @@
         angle = QLineEdit()
         rotate_btn = QPushButton("Rotate")
         layout.addWidget(angle_label)
         layout.addWidget(angle)
         layout.addWidget(rotate_btn)
 
         def rotate():
+            self.clear_button.click()
             ang = float(angle.text())
             transform.rotate(ang)
             rotated_pixmap = self.figure.pixmap_item.pixmap().transformed(transform)
             self.figure.setPixmap(rotated_pixmap)
+            dialog.close()
 
         rotate_btn.clicked.connect(rotate)
 
         dialog.show()
 
     def save_btn_click(self):
         dialog = QDialog(self)
         dialog.setWindowModality(Qt.WindowModality.ApplicationModal)
-        dialog.setMinimumSize(QSize(300, 100))
+        dialog.setMinimumSize(QSize(200, 100))
         layout = QVBoxLayout(dialog)
         allOrRoi = QComboBox()
         allOrRoi.addItems(["ROI", "ALL"])
-        file_path = QLineEdit()
         save_path_btn = QPushButton("Select storage path")
-        save_btn = QPushButton("Save")
         layout.addWidget(allOrRoi)
-        layout.addWidget(file_path)
         layout.addWidget(save_path_btn)
-        layout.addWidget(save_btn)
 
         def save_path_btn_click():
             filePath, _ = QFileDialog.getSaveFileName(
                 self,  # 父窗口对象
                 "Select storage path",  # 标题
                 self.last_open_dir  # 起始目录
             )
             self.last_open_dir = os.path.dirname(filePath)
             if filePath:
-                file_path.setText(filePath)
-                if allOrRoi.currentText() == "ALL":
-                    save_pixmap(filePath, self.figure.pixmap_item.pixmap())
-                else:
-                    if isinstance(self.figure.roi, RectangleRoi):
-                        pix = self.figure.pixmap_item.pixmap().copy(self.figure.roi.rect().toRect())
-                        save_pixmap(filePath, pix)
-                    else:
-                        show_message_box("请先选择ROI区域！")
-
-        def save_btn_click():
-            filePath = file_path.text()
-            if filePath:
                 if allOrRoi.currentText() == "ALL":
                     save_pixmap(filePath, self.figure.pixmap_item.pixmap())
                 else:
                     if isinstance(self.figure.roi, RectangleRoi):
                         pix = self.figure.pixmap_item.pixmap().copy(self.figure.roi.rect().toRect())
                         save_pixmap(filePath, pix)
                     else:
                         show_message_box("Please select the ROI area first!")
                         return
+                dialog.close()
                 show_message_box("Save Successful!")
 
         save_path_btn.clicked.connect(save_path_btn_click)
-        save_btn.clicked.connect(save_btn_click)
 
         dialog.show()
 
 
 class Button(QPushButton):
     def __init__(self, icon: QIcon, string: str, roi: ROI):
         QPushButton.__init__(self, icon, string)
```

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/ui/imageView.py` & `pyimagejgui-0.0.7/src/pyImageJGui/ui/imageView.py`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/src/pyImageJGui/utils/function.py` & `pyimagejgui-0.0.7/src/pyImageJGui/utils/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 
 def imread(file_path, dtype=np.uint8):
     img = cv.imdecode(np.fromfile(file_path, dtype=dtype), 0)
     return img
 
 
 def imwrite(save_path, img, format='bmp'):
-    cv.imencode(format, img)[1].tofile(save_path)
+    cv.imencode('.' + format, img)[1].tofile(save_path)
 
 
 def save_pixmap(save_path, pixmap: QPixmap, format='bmp'):
-    pixmap.save(save_path, format)
+    arr = QPixmapToArray(pixmap)
+    imwrite(save_path, arr, format)
 
 
 def show_message_box(text):
     msg_box = QMessageBox()
     msg_box.setIcon(QMessageBox.Icon.Information)
     msg_box.setText(text)
     msg_box.setStandardButtons(QMessageBox.StandardButton.Ok)
```

### Comparing `pyimagejgui-0.0.6/LICENSE` & `pyimagejgui-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagejgui-0.0.6/pyproject.toml` & `pyimagejgui-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyImageJGui"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python for ImageJ GUI"
 authors = [{name = "sdb", email = "sdb20200101@gmail.com"}]
 readme = "README.md"
 keywords = ["imagej", "GUI", "PySide6"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `pyimagejgui-0.0.6/PKG-INFO` & `pyimagejgui-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyImageJGui
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python for ImageJ GUI
 Project-URL: homepage, https://github.com/aghb123/pyImageJGui
 Author-email: sdb <sdb20200101@gmail.com>
 License-File: LICENSE
 Keywords: GUI,PySide6,imagej
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

