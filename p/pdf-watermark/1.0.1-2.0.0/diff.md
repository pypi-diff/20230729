# Comparing `tmp/pdf-watermark-1.0.1.tar.gz` & `tmp/pdf-watermark-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-watermark-1.0.1.tar", last modified: Wed Jun 28 14:41:40 2023, max compression
+gzip compressed data, was "pdf-watermark-2.0.0.tar", last modified: Sat Jul 29 19:31:14 2023, max compression
```

## Comparing `pdf-watermark-1.0.1.tar` & `pdf-watermark-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-06-28 14:41:40.898532 pdf-watermark-1.0.1/
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     1079 2023-06-26 20:37:07.000000 pdf-watermark-1.0.1/LICENSE
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       15 2023-06-26 20:38:11.000000 pdf-watermark-1.0.1/MANIFEST.in
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     4475 2023-06-28 14:41:40.898532 pdf-watermark-1.0.1/PKG-INFO
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     4033 2023-06-28 14:33:16.000000 pdf-watermark-1.0.1/README.md
-drwxr-xr-x   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-06-28 14:41:40.888532 pdf-watermark-1.0.1/app/
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-06-26 20:34:49.000000 pdf-watermark-1.0.1/app/__init__.py
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     4294 2023-06-28 13:39:29.000000 pdf-watermark-1.0.1/app/objects.py
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     4706 2023-06-28 13:34:45.000000 pdf-watermark-1.0.1/app/utils.py
-drwxr-xr-x   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-06-28 14:41:40.898532 pdf-watermark-1.0.1/pdf_watermark.egg-info/
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     4475 2023-06-28 14:41:40.000000 pdf-watermark-1.0.1/pdf_watermark.egg-info/PKG-INFO
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)      319 2023-06-28 14:41:40.000000 pdf-watermark-1.0.1/pdf_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)        1 2023-06-28 14:41:40.000000 pdf-watermark-1.0.1/pdf_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       44 2023-06-28 14:41:40.000000 pdf-watermark-1.0.1/pdf_watermark.egg-info/entry_points.txt
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       70 2023-06-28 14:41:40.000000 pdf-watermark-1.0.1/pdf_watermark.egg-info/requires.txt
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       14 2023-06-28 14:41:40.000000 pdf-watermark-1.0.1/pdf_watermark.egg-info/top_level.txt
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       38 2023-06-28 14:41:40.898532 pdf-watermark-1.0.1/setup.cfg
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)      930 2023-06-28 14:36:50.000000 pdf-watermark-1.0.1/setup.py
--rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     2658 2023-06-28 13:40:57.000000 pdf-watermark-1.0.1/watermark.py
+drwxr-xr-x   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-07-29 19:31:14.877283 pdf-watermark-2.0.0/
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     1079 2023-07-29 19:23:05.000000 pdf-watermark-2.0.0/LICENSE
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       15 2023-07-29 19:23:05.000000 pdf-watermark-2.0.0/MANIFEST.in
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     7336 2023-07-29 19:31:14.877283 pdf-watermark-2.0.0/PKG-INFO
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     6894 2023-07-29 19:26:36.000000 pdf-watermark-2.0.0/README.md
+drwxr-xr-x   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-07-29 19:31:14.877283 pdf-watermark-2.0.0/app/
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-07-29 19:23:05.000000 pdf-watermark-2.0.0/app/__init__.py
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     6030 2023-07-29 19:23:06.000000 pdf-watermark-2.0.0/app/draw.py
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     1421 2023-07-29 19:23:06.000000 pdf-watermark-2.0.0/app/handler.py
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     4127 2023-07-29 19:23:06.000000 pdf-watermark-2.0.0/app/options.py
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     1404 2023-07-29 19:23:06.000000 pdf-watermark-2.0.0/app/utils.py
+drwxr-xr-x   0 bastienlcn  (1000) bastienlcn  (1000)        0 2023-07-29 19:31:14.877283 pdf-watermark-2.0.0/pdf_watermark.egg-info/
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     7336 2023-07-29 19:31:14.000000 pdf-watermark-2.0.0/pdf_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)      346 2023-07-29 19:31:14.000000 pdf-watermark-2.0.0/pdf_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)        1 2023-07-29 19:31:14.000000 pdf-watermark-2.0.0/pdf_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       44 2023-07-29 19:31:14.000000 pdf-watermark-2.0.0/pdf_watermark.egg-info/entry_points.txt
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       70 2023-07-29 19:31:14.000000 pdf-watermark-2.0.0/pdf_watermark.egg-info/requires.txt
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       14 2023-07-29 19:31:14.000000 pdf-watermark-2.0.0/pdf_watermark.egg-info/top_level.txt
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)       38 2023-07-29 19:31:14.877283 pdf-watermark-2.0.0/setup.cfg
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)      930 2023-07-29 19:31:13.000000 pdf-watermark-2.0.0/setup.py
+-rw-r--r--   0 bastienlcn  (1000) bastienlcn  (1000)     4999 2023-07-29 19:23:06.000000 pdf-watermark-2.0.0/watermark.py
```

### Comparing `pdf-watermark-1.0.1/LICENSE` & `pdf-watermark-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf-watermark-1.0.1/PKG-INFO` & `pdf-watermark-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-watermark
-Version: 1.0.1
+Version: 2.0.0
 Summary: A python CLI tool to add watermarks to a PDF
 Home-page: https://github.com/bastienlc/pdf-watermark
 Author: Bastien Le Chenadec
 Author-email: bastien.lechenadec@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
@@ -16,28 +16,36 @@
 
 A python CLI tool to add watermarks to a PDF. Support for bulk processing of multiple PDF files, with nice saving options.
 
 ## Description
 
 There are multiple similar tools out there but I couldn't find one that really suited my needs. This project also serves as an excuse to play with building and distributing a python CLI tool.
 
-With this tool you can add a watermark to a PDF file. The watermark can either be a text string that you provide, or an image (PNG being the recommanded format). The watermark is repeated multiple times on each page.
+With this tool you can add a watermark to a PDF file. The watermark can either be a text string that you provide, or an image (PNG being the recommanded format).
 
-Below this is an example of a PDF before using this tool, after using this tool with a text watermark, and after using this tool with an image watermark.
+This tool provides two commands.
+* **insert**: The watermark is placed once on each page at a specific position.
+* **grid**: The watermark is repeated multiple times on each page in a grid pattern.
+
+Below is an example of a PDF before using this tool, after using this tool with the *grid* command and a text watermark, and after using this tool with the *grid* command and an image watermark.
 
 <p align="middle">
   <img src="https://raw.githubusercontent.com/bastienlc/pdf-watermark/master/images/before.png" width="29%" />
   <img src="https://raw.githubusercontent.com/bastienlc/pdf-watermark/master/images/text.png" width="29%" />
   <img src="https://raw.githubusercontent.com/bastienlc/pdf-watermark/master/images/image.png" width="29%" />
 </p>
 
-You can control the opacity of the watermark and its inclination. You can also control the number of repetitions along the horizontal and vertical directions, as well as wether to leave a margin around the page or not.
+You can control the opacity of the watermark and its inclination.
 
 There are also specific options for text and image watermarks. For text watermarks, you can control the color, font and font size. For image watermarks, you can add a scale factor (by default, the image is scaled to fit nicely in the rectangles created by the horizontal and vertical repetitions).
 
+With the *grid* command, you can control the number of repetitions along the horizontal and vertical directions, as well as wether to leave a margin around the page or not.
+
+With the *insert* command, you can control the x and y coordinates at which the watermark is inserted, as well as the horizontal alignment relative to x (left, center or right).
+
 ## Getting Started
 
 ### Dependencies
 
 * This project was built with python 3.11. However it should also run just fine with older versions.
 * See `requirements.txt` for the list of dependencies.
 
@@ -48,34 +56,91 @@
 ```
 pip install pdf-watermark
 ```
 
 ### Usage
 
 ```
-Usage: watermark [OPTIONS] FILE WATERMARK
+Usage: watermark [OPTIONS] COMMAND [ARGS]...
+
+  Add a watermark to one or more PDF files.
+
+  The watermark can be repeated in a grid pattern using the grid command, or
+  inserted at a specific position using the insert command.
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  grid    Add a watermark in a grid pattern.
+  insert  Add a watermark at a specific position.
+```
+
+**insert** command:
+```
+Usage: watermark insert [OPTIONS] FILE WATERMARK
+
+  Add a watermark at a specific position.
 
   Add a WATERMARK to one or more PDF files referenced by FILE. WATERMARK can
   be either a string or a path to an image file. FILE can be a single file or
   a directory, in which case all PDF files in the directory will be
   watermarked.
 
 Options:
+  -y, --y FLOAT                   Position of the watermark with respect to
+                                  the vertical direction. Must be between 0
+                                  and 1.
+  -x, --x FLOAT                   Position of the watermark with respect to
+                                  the horizontal direction. Must be between 0
+                                  and 1.
+  -ha, --horizontal-alignment TEXT
+                                  Alignment of the watermark with respect to
+                                  the horizontal direction. Can be one of
+                                  'left', 'right' and 'center'.
   -s, --save TEXT                 File or folder to save results to. By
                                   default, the input files are overwritten.
   -o, --opacity FLOAT             Watermark opacity between 0 (invisible) and
                                   1 (no transparency).
   -a, --angle FLOAT               Watermark inclination in degrees.
+  -tc, --text-color TEXT          Text color in hexadecimal format, e.g.
+                                  #000000.
+  -tf, --text-font TEXT           Text font to use. Supported fonts are those
+                                  supported by reportlab.
+  -ts, --text-size INTEGER        Text font size.
+  -is, --image-scale FLOAT        Scale factor for the image. Note that before
+                                  this factor is applied, the image is already
+                                  scaled down to fit in the boxes.
+  --help                          Show this message and exit.
+```
+
+**grid** command:
+```
+Usage: watermark grid [OPTIONS] FILE WATERMARK
+
+  Add a watermark in a grid pattern.
+
+  Add a WATERMARK to one or more PDF files referenced by FILE. WATERMARK can
+  be either a string or a path to an image file. FILE can be a single file or
+  a directory, in which case all PDF files in the directory will be
+  watermarked.
+
+Options:
   -h, --horizontal-boxes INTEGER  Number of repetitions of the watermark along
                                   the horizontal direction.
   -v, --vertical-boxes INTEGER    Number of repetitions of the watermark along
                                   the vertical direction.
   -m, --margin BOOLEAN            Wether to leave a margin around the page or
                                   not. When False (default), the watermark
                                   will be cut on the PDF edges.
+  -s, --save TEXT                 File or folder to save results to. By
+                                  default, the input files are overwritten.
+  -o, --opacity FLOAT             Watermark opacity between 0 (invisible) and
+                                  1 (no transparency).
+  -a, --angle FLOAT               Watermark inclination in degrees.
   -tc, --text-color TEXT          Text color in hexadecimal format, e.g.
                                   #000000.
   -tf, --text-font TEXT           Text font to use. Supported fonts are those
                                   supported by reportlab.
   -ts, --text-size INTEGER        Text font size.
   -is, --image-scale FLOAT        Scale factor for the image. Note that before
                                   this factor is applied, the image is already
@@ -90,14 +155,17 @@
 ## Version History
 
 * 1.0.0
     * Add text watermark support.
     * Add image watermark support.
     * Add CLI.
     * Add complex directories support.
+* 2.0.0
+    * Move tool to subcommand **grid**.
+    * Add **insert** command.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf-watermark-1.0.1/app/objects.py` & `pdf-watermark-2.0.0/app/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import Union
+from enum import Enum
+from typing import List, Union
 from reportlab.lib.colors import HexColor
 import os
 from reportlab.lib.utils import ImageReader
 
 
 class DrawingOptions:
     def __init__(
         self,
         watermark: str,
         opacity,
         angle: float,
-        horizontal_boxes: int,
-        vertical_boxes: int,
-        margin: bool,
         text_color: str,
         text_font: str,
         text_size: int,
         image_scale: float,
     ) -> None:
         self.image = None
         self.text = None
@@ -27,28 +25,25 @@
         ) and os.path.isfile(potential_image_path):
             self.image = ImageReader(watermark)
         else:
             self.text = watermark
 
         self.opacity = opacity
         self.angle = angle
-        self.horizontal_boxes = horizontal_boxes
-        self.vertical_boxes = vertical_boxes
-        self.margin = margin
         self.text_color = HexColor(text_color)
         self.text_font = text_font
         self.text_size = text_size
         self.image_scale = image_scale
 
 
 class FilesOptions:
     def __init__(
         self,
         input: str,
-        output: Union[None, str] = None,
+        output: Union[None, str],
     ) -> None:
         input = os.path.join(os.getcwd(), input)
 
         if not os.path.exists(input):
             raise ValueError("Input file or directory does not exist.")
         elif os.path.isdir(input):
             if output is not None and output.endswith(".pdf"):
@@ -100,36 +95,43 @@
     def __iter__(self):
         return iter(zip(self.input_files, self.output_files))
 
     def __next__(self):
         return next(zip(self.input_files, self.output_files))
 
 
-class UserInputs:
+class GridOptions:
     def __init__(
         self,
-        file: str,
-        watermark: str,
-        save: Union[None, str] = None,
-        opacity=0.1,
-        angle: float = 45,
-        horizontal_boxes: int = 3,
-        vertical_boxes: int = 6,
-        margin: bool = False,
-        text_color: str = "#000000",
-        text_font: str = "Helvetica",
-        text_size: int = 12,
-        image_scale: float = 1,
+        horizontal_boxes: int,
+        vertical_boxes: int,
+        margin: bool,
+    ) -> None:
+        self.horizontal_boxes = horizontal_boxes
+        self.vertical_boxes = vertical_boxes
+        self.margin = margin
+
+
+class Alignments(Enum):
+    LEFT = "left"
+    RIGHT = "right"
+    CENTER = "center"
+
+    @classmethod
+    def has_value(cls, value):
+        return value in cls._value2member_map_
+
+
+class InsertOptions:
+    def __init__(
+        self,
+        y: float,
+        x: float,
+        horizontal_alignment: List[Alignments],
     ) -> None:
-        self.files_options = FilesOptions(file, save)
-        self.drawing_options = DrawingOptions(
-            watermark=watermark,
-            opacity=opacity,
-            angle=angle,
-            horizontal_boxes=horizontal_boxes,
-            vertical_boxes=vertical_boxes,
-            margin=margin,
-            text_color=text_color,
-            text_font=text_font,
-            text_size=text_size,
-            image_scale=image_scale,
-        )
+        if not Alignments.has_value(horizontal_alignment):
+            raise Exception(
+                "Invalid argument. Horizontal alignment must be either left, right or center."
+            )
+        self.y = y
+        self.x = x
+        self.horizontal_alignment = horizontal_alignment
```

### Comparing `pdf-watermark-1.0.1/pdf_watermark.egg-info/PKG-INFO` & `pdf-watermark-2.0.0/pdf_watermark.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-watermark
-Version: 1.0.1
+Version: 2.0.0
 Summary: A python CLI tool to add watermarks to a PDF
 Home-page: https://github.com/bastienlc/pdf-watermark
 Author: Bastien Le Chenadec
 Author-email: bastien.lechenadec@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
@@ -16,28 +16,36 @@
 
 A python CLI tool to add watermarks to a PDF. Support for bulk processing of multiple PDF files, with nice saving options.
 
 ## Description
 
 There are multiple similar tools out there but I couldn't find one that really suited my needs. This project also serves as an excuse to play with building and distributing a python CLI tool.
 
-With this tool you can add a watermark to a PDF file. The watermark can either be a text string that you provide, or an image (PNG being the recommanded format). The watermark is repeated multiple times on each page.
+With this tool you can add a watermark to a PDF file. The watermark can either be a text string that you provide, or an image (PNG being the recommanded format).
 
-Below this is an example of a PDF before using this tool, after using this tool with a text watermark, and after using this tool with an image watermark.
+This tool provides two commands.
+* **insert**: The watermark is placed once on each page at a specific position.
+* **grid**: The watermark is repeated multiple times on each page in a grid pattern.
+
+Below is an example of a PDF before using this tool, after using this tool with the *grid* command and a text watermark, and after using this tool with the *grid* command and an image watermark.
 
 <p align="middle">
   <img src="https://raw.githubusercontent.com/bastienlc/pdf-watermark/master/images/before.png" width="29%" />
   <img src="https://raw.githubusercontent.com/bastienlc/pdf-watermark/master/images/text.png" width="29%" />
   <img src="https://raw.githubusercontent.com/bastienlc/pdf-watermark/master/images/image.png" width="29%" />
 </p>
 
-You can control the opacity of the watermark and its inclination. You can also control the number of repetitions along the horizontal and vertical directions, as well as wether to leave a margin around the page or not.
+You can control the opacity of the watermark and its inclination.
 
 There are also specific options for text and image watermarks. For text watermarks, you can control the color, font and font size. For image watermarks, you can add a scale factor (by default, the image is scaled to fit nicely in the rectangles created by the horizontal and vertical repetitions).
 
+With the *grid* command, you can control the number of repetitions along the horizontal and vertical directions, as well as wether to leave a margin around the page or not.
+
+With the *insert* command, you can control the x and y coordinates at which the watermark is inserted, as well as the horizontal alignment relative to x (left, center or right).
+
 ## Getting Started
 
 ### Dependencies
 
 * This project was built with python 3.11. However it should also run just fine with older versions.
 * See `requirements.txt` for the list of dependencies.
 
@@ -48,34 +56,91 @@
 ```
 pip install pdf-watermark
 ```
 
 ### Usage
 
 ```
-Usage: watermark [OPTIONS] FILE WATERMARK
+Usage: watermark [OPTIONS] COMMAND [ARGS]...
+
+  Add a watermark to one or more PDF files.
+
+  The watermark can be repeated in a grid pattern using the grid command, or
+  inserted at a specific position using the insert command.
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  grid    Add a watermark in a grid pattern.
+  insert  Add a watermark at a specific position.
+```
+
+**insert** command:
+```
+Usage: watermark insert [OPTIONS] FILE WATERMARK
+
+  Add a watermark at a specific position.
 
   Add a WATERMARK to one or more PDF files referenced by FILE. WATERMARK can
   be either a string or a path to an image file. FILE can be a single file or
   a directory, in which case all PDF files in the directory will be
   watermarked.
 
 Options:
+  -y, --y FLOAT                   Position of the watermark with respect to
+                                  the vertical direction. Must be between 0
+                                  and 1.
+  -x, --x FLOAT                   Position of the watermark with respect to
+                                  the horizontal direction. Must be between 0
+                                  and 1.
+  -ha, --horizontal-alignment TEXT
+                                  Alignment of the watermark with respect to
+                                  the horizontal direction. Can be one of
+                                  'left', 'right' and 'center'.
   -s, --save TEXT                 File or folder to save results to. By
                                   default, the input files are overwritten.
   -o, --opacity FLOAT             Watermark opacity between 0 (invisible) and
                                   1 (no transparency).
   -a, --angle FLOAT               Watermark inclination in degrees.
+  -tc, --text-color TEXT          Text color in hexadecimal format, e.g.
+                                  #000000.
+  -tf, --text-font TEXT           Text font to use. Supported fonts are those
+                                  supported by reportlab.
+  -ts, --text-size INTEGER        Text font size.
+  -is, --image-scale FLOAT        Scale factor for the image. Note that before
+                                  this factor is applied, the image is already
+                                  scaled down to fit in the boxes.
+  --help                          Show this message and exit.
+```
+
+**grid** command:
+```
+Usage: watermark grid [OPTIONS] FILE WATERMARK
+
+  Add a watermark in a grid pattern.
+
+  Add a WATERMARK to one or more PDF files referenced by FILE. WATERMARK can
+  be either a string or a path to an image file. FILE can be a single file or
+  a directory, in which case all PDF files in the directory will be
+  watermarked.
+
+Options:
   -h, --horizontal-boxes INTEGER  Number of repetitions of the watermark along
                                   the horizontal direction.
   -v, --vertical-boxes INTEGER    Number of repetitions of the watermark along
                                   the vertical direction.
   -m, --margin BOOLEAN            Wether to leave a margin around the page or
                                   not. When False (default), the watermark
                                   will be cut on the PDF edges.
+  -s, --save TEXT                 File or folder to save results to. By
+                                  default, the input files are overwritten.
+  -o, --opacity FLOAT             Watermark opacity between 0 (invisible) and
+                                  1 (no transparency).
+  -a, --angle FLOAT               Watermark inclination in degrees.
   -tc, --text-color TEXT          Text color in hexadecimal format, e.g.
                                   #000000.
   -tf, --text-font TEXT           Text font to use. Supported fonts are those
                                   supported by reportlab.
   -ts, --text-size INTEGER        Text font size.
   -is, --image-scale FLOAT        Scale factor for the image. Note that before
                                   this factor is applied, the image is already
@@ -90,14 +155,17 @@
 ## Version History
 
 * 1.0.0
     * Add text watermark support.
     * Add image watermark support.
     * Add CLI.
     * Add complex directories support.
+* 2.0.0
+    * Move tool to subcommand **grid**.
+    * Add **insert** command.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Acknowledgments
```

### Comparing `pdf-watermark-1.0.1/setup.py` & `pdf-watermark-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 setup(
     name="pdf-watermark",
-    version="1.0.1",
+    version="2.0.0",
     author="Bastien Le Chenadec",
     author_email="bastien.lechenadec@gmail.com",
     license="MIT License",
     description="A python CLI tool to add watermarks to a PDF",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bastienlc/pdf-watermark",
```

