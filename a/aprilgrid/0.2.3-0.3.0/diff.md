# Comparing `tmp/aprilgrid-0.2.3.tar.gz` & `tmp/aprilgrid-0.3.0.tar.gz`

## Comparing `aprilgrid-0.2.3.tar` & `aprilgrid-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/__about__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/__init__.py
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/common.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/detection.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/detector.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/qtp.py
--rw-r--r--   0        0        0    14678 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/tag_codes.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/src/aprilgrid/tag_family.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/LICENSE
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/README.md
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 aprilgrid-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/src/aprilgrid/__about__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/src/aprilgrid/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/src/aprilgrid/common.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/src/aprilgrid/detection.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/src/aprilgrid/detector.py
+-rw-r--r--   0        0        0    14678 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/src/aprilgrid/tag_codes.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/src/aprilgrid/tag_family.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/README.md
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 aprilgrid-0.3.0/PKG-INFO
```

### Comparing `aprilgrid-0.2.3/src/aprilgrid/tag_codes.py` & `aprilgrid-0.3.0/src/aprilgrid/tag_codes.py`

 * *Files identical despite different names*

### Comparing `aprilgrid-0.2.3/src/aprilgrid/tag_family.py` & `aprilgrid-0.3.0/src/aprilgrid/tag_family.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from dataclasses import dataclass
 import numpy as np
 from typing import List
 from .tag_codes import APRILTAG_CODE_DICT
 from .detection import Detection
 import cv2
 
+
 @dataclass
 class TagFamily:
     marker_edge: int
     border_bit: int
     min_distance: int
     _hamming_thres: int = 3
     debug_level: int = 0
 
     def __post_init__(self):
         self.name = f"t{self.marker_edge**2}h{self.min_distance}"
         if self.name not in APRILTAG_CODE_DICT:
-            raise ValueError(f"{self.name} is not in {APRILTAG_CODE_DICT.keys()}")
+            raise ValueError(
+                f"{self.name} is not in {APRILTAG_CODE_DICT.keys()}")
         self.tag_bit_list = np.array([np.array([bool(int(i)) for i in np.binary_repr(
             tag, 36)]) for tag in APRILTAG_CODE_DICT[self.name]])
-        
+
         self.marker_edge_bit = 2 * self.border_bit + self.marker_edge  # tagFamily.d 10
         edge_position = self.marker_edge_bit - 0.5
         self.tag_corners = np.expand_dims(np.array(
             [[-0.5, -0.5], [edge_position, -0.5], [edge_position, edge_position], [-0.5, edge_position]], np.float32), 1)
 
     def decode(self, detect_code: np.ndarray, quad, detections: List[Detection]):
         code_mat = detect_code.copy()
         for r in range(4):
-            scores = np.count_nonzero(code_mat.flatten() != self.tag_bit_list, axis=1)
+            scores = np.count_nonzero(
+                code_mat.flatten() != self.tag_bit_list, axis=1)
             best_score_idx = np.argmin(scores)
             best_score = scores[best_score_idx]
             if best_score < self._hamming_thres:
                 # print(f"best tag: {best_score_idx}, hamming: {best_score}")
                 new_quad = np.flip(np.roll(quad, -r, axis=0), axis=0)
                 detections.append(Detection(best_score_idx, new_quad))
                 if self.debug_level > 0:
@@ -65,12 +68,18 @@
             avg_brightness = np.average(tag_img)
             # TODO add some filter
             detect_code = np.where(tag_img[self.border_bit:-self.border_bit,
                                    self.border_bit: -self.border_bit] > avg_brightness+20, True, False)
             self.decode(detect_code, quad, detections)
         return detections
 
+
 TAG_FAMILY_DICT = {
-    "t36h11": TagFamily(6, 2, 11)
+    "t36h11": TagFamily(6, 2, 11, 3),
+    "t36h11b1": TagFamily(6, 1, 11, 3),
+    "t25h9": TagFamily(5, 2, 9, 2),
+    "t25h9b1": TagFamily(5, 1, 9, 2),
+    "t25h7": TagFamily(5, 2, 7, 2),
+    "t25h7b1": TagFamily(5, 1, 7, 2),
+    "t16h5": TagFamily(4, 2, 5, 1),
+    "t16h5b1": TagFamily(4, 1, 5, 1),
 }
-
-
```

### Comparing `aprilgrid-0.2.3/.gitignore` & `aprilgrid-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aprilgrid-0.2.3/LICENSE` & `aprilgrid-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aprilgrid-0.2.3/pyproject.toml` & `aprilgrid-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 requires = ["hatchling", "hatch-regex-commit"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aprilgrid"
 description = 'Pure python version of aprilgrid.'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "BSD-3-Clause"
 keywords = []
 authors = [
   { name = "Powei Lin", email = "poweilin1994@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -47,15 +46,15 @@
   "pytest-cov",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=test_package --cov=tests"
 no-cov = "cov --no-cov"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "aprilgrid/__about__.py",
 ]
```

