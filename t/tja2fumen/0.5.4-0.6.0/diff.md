# Comparing `tmp/tja2fumen-0.5.4.tar.gz` & `tmp/tja2fumen-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.5.4.tar", last modified: Thu Jul 20 03:22:34 2023, max compression
+gzip compressed data, was "tja2fumen-0.6.0.tar", last modified: Sat Jul 29 01:46:41 2023, max compression
```

## Comparing `tja2fumen-0.5.4.tar` & `tja2fumen-0.6.0.tar`

### file list

```diff
@@ -1,67 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 03:22:34.194047 tja2fumen-0.5.4/
--rw-rw-rw-   0        0        0     1083 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5595 2023-07-20 03:22:34.194047 tja2fumen-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/README.md
--rw-rw-rw-   0        0        0      897 2023-07-20 03:22:23.000000 tja2fumen-0.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 03:22:34.194047 tja2fumen-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:22:34.147173 tja2fumen-0.5.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 03:22:34.162798 tja2fumen-0.5.4/src/tja2fumen/
--rw-rw-rw-   0        0        0     1754 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     2030 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    21207 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    18755 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:22:34.194047 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    20989 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-1.csv
--rw-rw-rw-   0        0        0    20505 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-2-3.csv
--rw-rw-rw-   0        0        0    21140 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-4-5.csv
--rw-rw-rw-   0        0        0    20349 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-1-2.csv
--rw-rw-rw-   0        0        0    20328 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-3.csv
--rw-rw-rw-   0        0        0    20390 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-4.csv
--rw-rw-rw-   0        0        0    20545 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-5-8.csv
--rw-rw-rw-   0        0        0    20516 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-1-2.csv
--rw-rw-rw-   0        0        0    20482 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-3.csv
--rw-rw-rw-   0        0        0    20393 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-4.csv
--rw-rw-rw-   0        0        0    21000 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-5-7.csv
--rw-rw-rw-   0        0        0    20458 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-1-7.csv
--rw-rw-rw-   0        0        0    20435 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-8.csv
--rw-rw-rw-   0        0        0    20464 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-9-10.csv
--rw-rw-rw-   0        0        0    20661 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-1.csv
--rw-rw-rw-   0        0        0    20385 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-2-3.csv
--rw-rw-rw-   0        0        0    20976 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-4-5.csv
--rw-rw-rw-   0        0        0    20222 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-1-2.csv
--rw-rw-rw-   0        0        0    20145 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-3.csv
--rw-rw-rw-   0        0        0    20136 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-4.csv
--rw-rw-rw-   0        0        0    20182 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-5-8.csv
--rw-rw-rw-   0        0        0    20294 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-1-2.csv
--rw-rw-rw-   0        0        0    20289 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-3.csv
--rw-rw-rw-   0        0        0    20245 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-4.csv
--rw-rw-rw-   0        0        0    20715 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-5-7.csv
--rw-rw-rw-   0        0        0    19707 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-1-7.csv
--rw-rw-rw-   0        0        0    19785 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-8.csv
--rw-rw-rw-   0        0        0    19777 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-9-10.csv
--rw-rw-rw-   0        0        0    23889 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-9-10.csv
--rw-rw-rw-   0        0        0    12628 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/types.py
--rw-rw-rw-   0        0        0     1574 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     1664 2023-07-20 03:21:09.000000 tja2fumen-0.5.4/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-20 03:22:34.162798 tja2fumen-0.5.4/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     5595 2023-07-20 03:22:34.000000 tja2fumen-0.5.4/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2582 2023-07-20 03:22:34.000000 tja2fumen-0.5.4/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 03:22:34.000000 tja2fumen-0.5.4/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-20 03:22:34.000000 tja2fumen-0.5.4/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-20 03:22:34.000000 tja2fumen-0.5.4/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 03:22:34.000000 tja2fumen-0.5.4/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/
+-rw-rw-rw-   0        0        0     1085 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       37 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11858 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10129 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/README.md
+-rw-rw-rw-   0        0        0     1084 2023-07-29 01:46:25.000000 tja2fumen-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.049666 tja2fumen-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/src/tja2fumen/
+-rw-rw-rw-   0        0        0     2094 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     2821 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    18498 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0   307495 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/hp_values.csv
+-rw-rw-rw-   0        0        0    22522 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/parsers.py
+-rw-rw-rw-   0        0        0    18235 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/types.py
+-rw-rw-rw-   0        0        0     2468 2023-07-29 01:45:18.000000 tja2fumen-0.6.0/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-29 01:46:41.065293 tja2fumen-0.6.0/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0    11858 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 01:46:41.000000 tja2fumen-0.6.0/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.5.4/LICENSE.txt` & `tja2fumen-0.6.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `tja2fumen-0.5.4/pyproject.toml` & `tja2fumen-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.5.4"
+version = "0.6.0"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
@@ -14,15 +14,23 @@
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 tja2fumen = "tja2fumen:main"
 
 [project.optional-dependencies]
-dev = ["pytest", "build", "pyinstaller", "twine", "toml-cli"]
+dev = ["pytest", "build", "pyinstaller", "twine", "toml-cli",
+       "flake8", "pyproject-flake8"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.pytest.ini_options]
 addopts = "-vv --tb=short"
-console_output_style = "count"
+console_output_style = "count"
+
+[tool.flake8]
+exclude = "venv/"
+per-file-ignores = """
+    ./src/tja2fumen/types.py: E221
+    ./testing/test_conversion.py: E221, E272
+"""
```

### Comparing `tja2fumen-0.5.4/src/tja2fumen/__init__.py` & `tja2fumen-0.6.0/src/tja2fumen/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import argparse
 import os
 import sys
 
 from tja2fumen.parsers import parse_tja
-from tja2fumen.writers import write_fumen
 from tja2fumen.converters import convert_tja_to_fumen
+from tja2fumen.writers import write_fumen
 from tja2fumen.constants import COURSE_IDS
 
 
 def main(argv=None):
+    """
+    Main entry point for tja2fumen's command line interface.
+
+    Three steps are performed:
+       1. Parse TJA into multiple TJACourse objects. Then, for each course:
+          2. Convert TJACourse objects into FumenCourse objects.
+          3. Write each FumenCourse to its own .bin file.
+    """
     if not argv:
         argv = sys.argv[1:]
 
     parser = argparse.ArgumentParser(
         description="tja2fumen"
     )
     parser.add_argument(
@@ -22,30 +30,32 @@
     args = parser.parse_args(argv)
     fname_tja = getattr(args, "file.tja")
     base_name = os.path.splitext(fname_tja)[0]
 
     # Parse lines in TJA file
     parsed_tja = parse_tja(fname_tja)
 
-    # Convert parsed TJA courses to Fumen data, and write each course to `.bin` files
+    # Convert parsed TJA courses and write each course to `.bin` files
     for course in parsed_tja.courses.items():
-        convert_and_write(course, base_name, single_course=(len(parsed_tja.courses) == 1))
+        convert_and_write(course, base_name,
+                          single_course=(len(parsed_tja.courses) == 1))
 
 
 def convert_and_write(parsed_course, base_name, single_course=False):
+    """Process the parsed data for a single TJA course."""
     course_name, tja_data = parsed_course
     fumen_data = convert_tja_to_fumen(tja_data)
     # Add course ID (e.g. '_x', '_x_1', '_x_2') to the output file's base name
     output_name = base_name
     if single_course:
-        pass  # Replicate tja2bin.exe behavior by excluding course ID if there's only one course
+        pass  # Replicate tja2bin.exe behavior by excluding course ID
     else:
-        split_name = course_name.split("P")  # e.g. 'OniP2' -> ['Oni', '2'], 'Oni' -> ['Oni']
+        split_name = course_name.split("P")  # e.g. 'OniP2' -> ['Oni', '2']
         output_name += f"_{COURSE_IDS[split_name[0]]}"
         if len(split_name) == 2:
-            output_name += f"_{split_name[1]}"  # Add "_1" or "_2" if P1/P2 chart
+            output_name += f"_{split_name[1]}"  # Add "_1"/"_2" if P1/P2 chart
     write_fumen(f"{output_name}.bin", fumen_data)
 
 
 # NB: This entry point is necessary for the Pyinstaller executable
 if __name__ == "__main__":
     main()
```

### Comparing `tja2fumen-0.5.4/src/tja2fumen/converters.py` & `tja2fumen-0.6.0/src/tja2fumen/converters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,99 @@
 import re
 
 from tja2fumen.types import TJAMeasureProcessed, FumenCourse, FumenNote
 
 
 def process_tja_commands(tja):
     """
-    Merge TJA 'data' and 'event' fields into a single measure property, and split
-    measures into sub-measures whenever a mid-measure BPM/SCROLL/GOGO change occurs.
+    Process each #COMMAND present in a TJASong's measures, and assign their
+    values as attributes to each measure.
 
-    The TJA parser produces measure objects with two important properties:
-      - 'data': Contains the note data (1: don, 2: ka, etc.) along with spacing (s)
-      - 'events' Contains event commands such as MEASURE, BPMCHANGE, GOGOTIME, etc.
+    This function takes care of two main tasks:
+        1. Keeping track of what the current values are for BPM, scroll,
+           gogotime, barline, and time signature (#MEASURE).
+        2. Detecting when a command is placed in the middle of a measure,
+           and splitting that measure into sub-measures.
+
+    ((Note: We split measures into sub-measures because official `.bin` files
+      can only have 1 value for BPM/SCROLL/GOGO per measure. So, if a TJA
+      measure has multiple BPMs/SCROLLs/GOGOs, it has to be split up.))
 
-    However, notes and events can be intertwined within a single measure. So, it's
-    not possible to process them separately; they must be considered as single sequence.
-
-    A particular danger is BPM changes. TJA allows multiple BPMs within a single measure,
-    but the fumen format permits one BPM per measure. So, a TJA measure must be split up
-    if it has multiple BPM changes within a measure.
-
-    In the future, this logic should probably be moved into the TJA parser itself.
+    After this function is finished, all the #COMMANDS will be gone, and each
+    measure will have attributes (e.g. measure.bpm, measure.scroll) instead.
     """
-    tja_branches_processed = {branch_name: [] for branch_name in tja.branches.keys()}
+    tja_branches_processed = {branch_name: []
+                              for branch_name in tja.branches.keys()}
     for branch_name, branch_measures_tja in tja.branches.items():
         current_bpm = tja.BPM
         current_scroll = 1.0
         current_gogo = False
         current_barline = True
         current_dividend = 4
         current_divisor = 4
         for measure_tja in branch_measures_tja:
-            # Split measure into submeasure
             measure_tja_processed = TJAMeasureProcessed(
                 bpm=current_bpm,
-                scroll=current_scroll, 
-                gogo=current_gogo, 
-                barline=current_barline, 
-                time_sig=[current_dividend, current_divisor], 
+                scroll=current_scroll,
+                gogo=current_gogo,
+                barline=current_barline,
+                time_sig=[current_dividend, current_divisor],
                 subdivisions=len(measure_tja.notes),
             )
             for data in measure_tja.combined:
                 # Handle note data
                 if data.name == 'note':
                     measure_tja_processed.data.append(data)
 
-                # Handle commands that can only be placed between measures (i.e. no mid-measure variations)
+                # Handle commands that can only be placed between measures
+                # (i.e. no mid-measure variations)
                 elif data.name == 'delay':
                     measure_tja_processed.delay = data.value * 1000  # ms -> s
                 elif data.name == 'branch_start':
                     measure_tja_processed.branch_start = data.value
                 elif data.name == 'section':
                     measure_tja_processed.section = data.value
+                elif data.name == 'levelhold':
+                    measure_tja_processed.levelhold = True
                 elif data.name == 'barline':
                     current_barline = bool(int(data.value))
                     measure_tja_processed.barline = current_barline
                 elif data.name == 'measure':
                     match_measure = re.match(r"(\d+)/(\d+)", data.value)
                     if not match_measure:
                         continue
                     current_dividend = int(match_measure.group(1))
                     current_divisor = int(match_measure.group(2))
-                    measure_tja_processed.time_sig = [current_dividend, current_divisor]
+                    measure_tja_processed.time_sig = [current_dividend,
+                                                      current_divisor]
 
-                # Handle commands that can be placed in the middle of a measure.
-                #    NB: For fumen files, if there is a mid-measure change to BPM/SCROLL/GOGO, then the measure will
-                #    actually be split into two small submeasures. So, we need to start a new measure in those cases.
+                # Handle commands that can be placed in the middle of a
+                # measure. (For fumen files, if there is a mid-measure change
+                # to BPM/SCROLL/GOGO, then the measure will actually be split
+                # into two small submeasures. So, we need to start a new
+                # measure in those cases.)
                 elif data.name in ['bpm', 'scroll', 'gogo']:
                     # Parse the values
                     if data.name == 'bpm':
                         new_val = current_bpm = float(data.value)
                     elif data.name == 'scroll':
                         new_val = current_scroll = data.value
                     elif data.name == 'gogo':
                         new_val = current_gogo = bool(int(data.value))
                     # Check for mid-measure commands
-                    # - Case 1: Command happens at the start of a measure; just change the value directly
+                    # - Case 1: Command happens at the start of a measure;
+                    #           just change the value directly
                     if data.pos == 0:
                         measure_tja_processed.__setattr__(data.name, new_val)
-                    # - Case 2: Command occurs mid-measure, so start a new sub-measure
+                    # - Case 2: Command happens in the middle of a measure;
+                    #           start a new sub-measure
                     else:
                         measure_tja_processed.pos_end = data.pos
-                        tja_branches_processed[branch_name].append(measure_tja_processed)
+                        tja_branches_processed[branch_name]\
+                            .append(measure_tja_processed)
                         measure_tja_processed = TJAMeasureProcessed(
                             bpm=current_bpm,
                             scroll=current_scroll,
                             gogo=current_gogo,
                             barline=current_barline,
                             time_sig=[current_dividend, current_divisor],
                             subdivisions=len(measure_tja.notes),
@@ -95,246 +104,278 @@
                     print(f"Unexpected event type: {data.name}")
 
             measure_tja_processed.pos_end = len(measure_tja.notes)
             tja_branches_processed[branch_name].append(measure_tja_processed)
 
     has_branches = all(len(b) for b in tja_branches_processed.values())
     if has_branches:
-        branch_lens = [len(b) for b in tja.branches.values()]
-        if not branch_lens.count(branch_lens[0]) == len(branch_lens):
-            raise ValueError("Branches do not have the same number of measures.")
-        else:
-            branch_corrected_lens = [len(b) for b in tja_branches_processed.values()]
-            if not branch_corrected_lens.count(branch_corrected_lens[0]) == len(branch_corrected_lens):
-                raise ValueError("Branches do not have matching GOGO/SCROLL/BPM commands.")
+        if len(set([len(b) for b in tja.branches.values()])) != 1:
+            raise ValueError(
+                "Branches do not have the same number of measures. (This "
+                "check was performed prior to splitting up the measures due "
+                "to mid-measure commands. Please check the number of ',' you"
+                "have in each branch.)"
+            )
+        if len(set([len(b) for b in tja_branches_processed.values()])) != 1:
+            raise ValueError(
+                "Branches do not have the same number of measures. (This "
+                "check was performed after splitting up the measures due "
+                "to mid-measure commands. Please check any GOGO, BPMCHANGE, "
+                "and SCROLL commands you have in your branches, and make sure"
+                "that each branch has the same number of commands.)"
+            )
 
     return tja_branches_processed
 
 
 def convert_tja_to_fumen(tja):
+    """
+    Convert TJA data to Fumen data by calculating Fumen-specific values.
+
+    Fumen files (`.bin`) use a very strict file structure. Certain values are
+    expected at very specific byte locations in the file, such as:
+      - Header metadata (first 520 bytes). The header stores information such
+        as branch points for each note type, soul gauge behavior, etc.
+      - Note data (millisecond offset values, drumroll duration, etc.)
+      - Branch condition info for each measure
+
+    Since TJA files only contain notes and commands, we must compute all of
+    these extra values ourselves. The values are then stored in new "Fumen"
+    Python objects that mimic the structure of the fumen `.bin` files:
+
+    FumenCourse
+    ├─ FumenMeasure
+    │  ├─ FumenBranch ('normal')
+    │  │  ├─ FumenNote
+    │  │  ├─ FumenNote
+    │  │  └─ ...
+    │  ├─ FumenBranch ('professional')
+    │  └─ FumenBranch ('master')
+    ├─ FumenMeasure
+    ├─ FumenMeasure
+    └─ ...
+
+    ((Note: The fumen file structure is the opposite of the TJA file structure;
+    branch data is stored within the measure object, rather than measure data
+    being stored within the branch object.))
+    """
     # Preprocess commands
-    processed_tja_branches = process_tja_commands(tja)
+    tja_branches_processed = process_tja_commands(tja)
 
     # Pre-allocate the measures for the converted TJA
+    n_measures = len(tja_branches_processed['normal'])
     fumen = FumenCourse(
-        measures=len(processed_tja_branches['normal']),
+        measures=n_measures,
         score_init=tja.score_init,
         score_diff=tja.score_diff,
     )
 
+    # Set song metadata using information from the processed measures
+    fumen.header.b512_b515_number_of_measures = n_measures
+    fumen.header.b432_b435_has_branches = int(all(
+        [len(b) for b in tja_branches_processed.values()]
+    ))
+
     # Iterate through the different branches in the TJA
-    total_notes = {'normal': 0, 'advanced': 0, 'master': 0}
-    for current_branch, branch_measures_tja_processed in processed_tja_branches.items():
-        if not len(branch_measures_tja_processed):
+    total_notes = {'normal': 0, 'professional': 0, 'master': 0}
+    for current_branch, branch_tja in tja_branches_processed.items():
+        if not len(branch_tja):
             continue
-        total_notes_branch = 0
-        note_counter_branch = 0
+        branch_points_total = 0
+        branch_points_measure = 0
         current_drumroll = None
+        current_levelhold = False
         branch_conditions = []
         course_balloons = tja.balloon.copy()
 
         # Iterate through the measures within the branch
-        for idx_m, measure_tja_processed in enumerate(branch_measures_tja_processed):
-            # Fetch a pair of measures
-            measure_fumen_prev = fumen.measures[idx_m-1] if idx_m != 0 else None
+        for idx_m, measure_tja in enumerate(branch_tja):
+            # Fetch the corresponding fumen measure
             measure_fumen = fumen.measures[idx_m]
 
-            # Copy over basic measure properties from the TJA (that don't depend on notes or commands)
-            measure_fumen.branches[current_branch].speed = measure_tja_processed.scroll
-            measure_fumen.gogo = measure_tja_processed.gogo
-            measure_fumen.bpm = measure_tja_processed.bpm
+            # Copy over basic measure properties from the TJA
+            measure_fumen.branches[current_branch].speed = measure_tja.scroll
+            measure_fumen.gogo = measure_tja.gogo
+            measure_fumen.bpm = measure_tja.bpm
 
             # Compute the duration of the measure
-            # First, we compute the duration for a full 4/4 measure
-            measure_duration_full_measure = 4 * 60_000 / measure_tja_processed.bpm
-            # Next, we adjust this duration based on both:
-            #   1. The *actual* measure size (e.g. #MEASURE 1/8, #MEASURE 5/4, etc.)
-            measure_size = measure_tja_processed.time_sig[0] / measure_tja_processed.time_sig[1]
-            #   2. Whether this is a "submeasure" (i.e. it contains mid-measure commands, which split up the measure)
-            #      - If this is a submeasure, then `measure_length` will be less than the total number of subdivisions.
-            measure_length = measure_tja_processed.pos_end - measure_tja_processed.pos_start
-            #      - In other words, `measure_ratio` will be less than 1.0:
-            measure_ratio = (1.0 if measure_tja_processed.subdivisions == 0.0  # Avoid division by 0 for empty measures
-                            else (measure_length / measure_tja_processed.subdivisions))
-            # Apply the 2 adjustments to the measure duration
-            measure_fumen.duration = measure_duration = measure_duration_full_measure * measure_size * measure_ratio
-
-            # Compute the millisecond offsets for the start and end of each measure
-            #  - Start: When the notes first appear on screen (to the right)
-            #  - End:   When the notes arrive at the judgment line, and the note gets hit.
-            if idx_m == 0:
-                measure_fumen.fumen_offset_start = (tja.offset * 1000 * -1) - measure_duration_full_measure
-            else:
-                # First, start the measure using the end timing of the previous measure (plus any #DELAY commands)
-                measure_fumen.fumen_offset_start = measure_fumen_prev.fumen_offset_end + measure_tja_processed.delay
-                # Next, adjust the start timing to account for #BPMCHANGE commands (!!! Discovered by tana :3 !!!)
-                # To understand what's going on here, imagine the following simple example:
-                #   * You have a very slow-moving note (i.e. low BPM), like the big DON in Donkama 2000.
-                #   * All the other notes move fast (i.e. high BPM), moving past the big slow note.
-                #   * To get this overlapping to work, you need the big slow note to START EARLY, but also END LATE:
-                #      - An early start means you need to subtract a LOT of time from the starting fumenOffset.
-                #      - Thankfully, the low BPM of the slow note will create a HUGE `measure_offset_adjustment`,
-                #        since we are dividing by the BPMs, and dividing by a small number will result in a big number.
-                measure_offset_adjustment = (4 * 60_000 / measure_fumen.bpm) - (4 * 60_000 / measure_fumen_prev.bpm)
-                #      - When we subtract this adjustment from the fumen_offset_start, we get the "START EARLY" part:
-                measure_fumen.fumen_offset_start -= measure_offset_adjustment
-                #      - The low BPM of the slow note will also create a HUGE measure duration.
-                #      - When we add this long duration to the EARLY START, we end up with the "END LATE" part:
-            measure_fumen.fumen_offset_end = measure_fumen.fumen_offset_start + measure_fumen.duration
-
-            # Best guess at what 'barline' status means for each measure:
-            # - 'True' means the measure lands on a barline (i.e. most measures), and thus barline should be shown
-            # - 'False' means that the measure doesn't land on a barline, and thus barline should be hidden.
-            #   For example:
+            measure_length = measure_tja.pos_end - measure_tja.pos_start
+            measure_fumen.set_duration(
+                time_sig=measure_tja.time_sig,
+                measure_length=measure_length,
+                subdivisions=measure_tja.subdivisions
+            )
+
+            # Compute the millisecond offsets for the start/end of each measure
+            measure_fumen.set_ms_offsets(
+                song_offset=tja.offset,
+                delay=measure_tja.delay,
+                prev_measure=(fumen.measures[idx_m-1] if idx_m else None),
+                first_measure=(idx_m == 0)
+            )
+
+            # Handle whether barline should be hidden:
             #     1. Measures where #BARLINEOFF has been set
             #     2. Sub-measures that don't fall on the barline
-            if measure_tja_processed.barline is False or (measure_ratio != 1.0 and measure_tja_processed.pos_start != 0):
+            barline_off = measure_tja.barline is False
+            is_submeasure = (measure_length < measure_tja.subdivisions and
+                             measure_tja.pos_start != 0)
+            if barline_off or is_submeasure:
                 measure_fumen.barline = False
 
-            # If a #SECTION command occurs in isolation, and it has a valid condition, then treat it like a branch_start
-            if (measure_tja_processed.section is not None and measure_tja_processed.section != 'not_available'
-                    and not measure_tja_processed.branch_start):
-                branch_condition = measure_tja_processed.section
-            else:
-                branch_condition = measure_tja_processed.branch_start
-
             # Check to see if the measure contains a branching condition
+            branch_condition = measure_tja.branch_start
             if branch_condition:
-                # Determine which values to assign based on the type of branching condition
-                if branch_condition[0] == 'p':
-                    vals = []
-                    for percent in branch_condition[1:]:
-                        # Ensure percentage is between 0% and 100%
-                        if 0 <= percent <= 1:
-                            val = total_notes_branch * percent * 20
-                            # If the result is very close, then round to account for lack of precision in percentage
-                            if abs(val - round(val)) < 0.1:
-                                val = round(val)
-                            vals.append(int(val))
-                        # If it is above 100%, then it means a guaranteed "level down". Fumens use 999 for this.
-                        elif percent > 1:
-                            vals.append(999)
-                        # If it is below 0%, it is a guaranteed "level up". Fumens use 0 for this.
-                        else:
-                            vals.append(0)
-                    if current_branch == 'normal':
-                        measure_fumen.branch_info[0:2] = vals
-                    elif current_branch == 'advanced':
-                        measure_fumen.branch_info[2:4] = vals
-                    elif current_branch == 'master':
-                        measure_fumen.branch_info[4:6] = vals
-
-                # If it's a drumroll, then the values to use depends on whether there is a #SECTION in the same measure
-                #   - If there is a #SECTION, then accuracy is reset, so repeat the same condition for all 3 branches
-                #   - If there isn't a #SECTION, but it's the first branch condition, repeat for all 3 branches as well
-                #   - If there isn't a #SECTION, and there are previous branch conditions, the outcomes now matter:
-                #        * If the player failed to go from Normal -> Advanced/Master, then they must stay in Normal,
-                #          hence the 999 values (which force them to stay in Normal)
-                #        * If the player made it to Advanced, then both condition values still apply (for either
-                #          staying in Advanced or leveling up to Master)
-                #        * If the player made it to Master, then only use the "master condition" value (2), otherwise
-                #          they fall back to Normal.
-                #   - The "no-#SECTION" behavior can be seen in songs like "Shoutoku Taiko no 「Hi Izuru Made Asuka」"
-                elif branch_condition[0] == 'r':
-                    if current_branch == 'normal':
-                        measure_fumen.branch_info[0:2] = (branch_condition[1:] if measure_tja_processed.section or
-                                                        not measure_tja_processed.section and not branch_conditions
-                                                        else [999, 999])
-                    elif current_branch == 'advanced':
-                        measure_fumen.branch_info[2:4] = branch_condition[1:]
-                    elif current_branch == 'master':
-                        measure_fumen.branch_info[4:6] = (branch_condition[1:] if measure_tja_processed.section or
-                                                        not measure_tja_processed.section and not branch_conditions
-                                                        else [branch_condition[2]] * 2)
-
-                # Reset the note counter corresponding to this branch (i.e. reset the accuracy)
-                total_notes_branch = 0
-                # Cache branch conditions, but skip conditions where the only purpose is to level down to 'normal'
-                if measure_fumen.branch_info != [999, 999, 999, 999, 999, 999]:
-                    branch_conditions.append(branch_condition)
+                # Update the branch_info values for the measure
+                measure_fumen.set_branch_info(
+                    branch_condition, branch_points_total, current_branch,
+                    first_branch_condition=(not branch_conditions),
+                    has_section=bool(measure_tja.section),
+                    has_levelhold=current_levelhold
+                )
+                # Reset the points to prepare for the next `#BRANCHSTART p`
+                branch_points_total = 0
+                # Reset the levelhold value (so that future branch_conditions
+                # work normally)
+                current_levelhold = False
+                # Keep track of the branch conditions (to later determine how
+                # to set the header bytes for branches)
+                branch_conditions.append(branch_condition)
 
-            # NB: We update the branch condition note counter *after* we check the current measure's branch condition.
+            # NB: We update the branch condition note counter *after*
+            # we check the current measure's branch condition.
             # This is because the TJA spec says:
-            #    "The requirement is calculated one measure before #BRANCHSTART, changing the branch visually when it
+            #    "The requirement is calculated one measure before
+            #     #BRANCHSTART, changing the branch visually when it
             #     is calculated and changing the notes after #BRANCHSTART."
-            # So, by delaying the summation by one measure, we perform the calculation with notes "one measure before".
-            total_notes_branch += note_counter_branch
+            # So, by delaying the summation by one measure, we perform the
+            # calculation with notes "one measure before".
+            branch_points_total += branch_points_measure
+
+            # LEVELHOLD essentially means "ignore the branch condition for
+            # the next `#BRANCHSTART` command", so we check this value after
+            # we've already processed the branch condition for this measure.
+            if measure_tja.levelhold:
+                current_levelhold = True
 
             # Create notes based on TJA measure data
-            note_counter_branch = 0
-            note_counter = 0
-            for idx_d, data in enumerate(measure_tja_processed.data):
-                if data.name == 'note':
-                    note = FumenNote()
-                    # Note positions must be calculated using the base measure duration (that uses a single BPM value)
-                    # (In other words, note positions do not take into account any mid-measure BPM change adjustments.)
-                    note.pos = measure_duration * (data.pos - measure_tja_processed.pos_start) / measure_length
-                    # Handle the note that represents the end of a drumroll/balloon
-                    if data.value == "EndDRB":
-                        # If a drumroll spans a single measure, then add the difference between start/end position
-                        if not current_drumroll.multimeasure:
-                            current_drumroll.duration += (note.pos - current_drumroll.pos)
-                        # Otherwise, if a drumroll spans multiple measures, then we want to add the duration between
-                        # the start of the measure (i.e. pos=0.0) and the drumroll's end position.
-                        else:
-                            current_drumroll.duration += (note.pos - 0.0)
-                        # 1182, 1385, 1588, 2469, 1568, 752, 1568
-                        current_drumroll.duration = float(int(current_drumroll.duration))
-                        current_drumroll = None
-                        continue
-                    # The TJA spec technically allows you to place double-Kusudama notes:
-                    #    "Use another 9 to specify when to lower the points for clearing."
-                    # But this is unsupported in fumens, so just skip the second Kusudama note.
-                    if data.value == "Kusudama" and current_drumroll:
-                        continue
-                    # Handle the remaining non-EndDRB, non-double Kusudama notes
-                    note.type = data.value
-                    note.score_init = tja.score_init
-                    note.score_diff = tja.score_diff
-                    # Handle drumroll/balloon-specific metadata
-                    if note.type in ["Balloon", "Kusudama"]:
+            branch_points_measure = 0
+            for idx_d, data in enumerate(measure_tja.data):
+                # Compute the ms position of the note
+                pos_ratio = ((data.pos - measure_tja.pos_start) /
+                             (measure_tja.pos_end - measure_tja.pos_start))
+                note_pos = (measure_fumen.duration * pos_ratio)
+
+                # Handle '8' notes (end of a drumroll/balloon)
+                if data.value == "EndDRB":
+                    # If a drumroll spans a single measure, then add the
+                    # difference between start/end position
+                    if not current_drumroll.multimeasure:
+                        current_drumroll.duration += (note_pos -
+                                                      current_drumroll.pos)
+                    # Otherwise, if a drumroll spans multiple measures,
+                    # then we want to add the duration between the start
+                    # of the measure and the drumroll's end position.
+                    else:
+                        current_drumroll.duration += (note_pos - 0.0)
+                    current_drumroll.duration = float(int(
+                        current_drumroll.duration
+                    ))
+                    current_drumroll = None
+                    continue
+
+                # The TJA spec technically allows you to place
+                # double-Kusudama notes. But this is unsupported in
+                # fumens, so just skip the second Kusudama note.
+                if data.value == "Kusudama" and current_drumroll:
+                    continue
+
+                # Handle note metadata
+                note = FumenNote()
+                note.pos = note_pos
+                note.note_type = data.value
+                note.score_init = tja.score_init
+                note.score_diff = tja.score_diff
+
+                # Handle drumroll notes
+                if note.note_type in ["Balloon", "Kusudama"]:
+                    try:
                         note.hits = course_balloons.pop(0)
-                        current_drumroll = note
-                        total_notes[current_branch] -= 1
-                    if note.type in ["Drumroll", "DRUMROLL"]:
-                        current_drumroll = note
-                        total_notes[current_branch] -= 1
-                    # Count dons, kas, and balloons for the purpose of tracking branching accuracy
-                    if note.type.lower() in ['don', 'ka']:
-                        note_counter_branch += 1
-                    elif note.type.lower() in ['balloon', 'kusudama']:
-                        note_counter_branch += 1.5
-                    measure_fumen.branches[current_branch].notes.append(note)
-                    note_counter += 1
+                    except IndexError:
+                        raise ValueError(f"Not enough values for 'BALLOON: "
+                                         f"{','.join(course_balloons)}'")
+                    current_drumroll = note
+                elif note.note_type in ["Drumroll", "DRUMROLL"]:
+                    current_drumroll = note
+
+                # Track Don/Ka notes (to later compute header values)
+                elif (note.note_type.lower().startswith('don')
+                        or note.note_type.lower().startswith('ka')):
+                    total_notes[current_branch] += 1
+
+                # Track branch points (to later compute `#BRANCHSTART p` vals)
+                if note.note_type in ['Don', 'Ka']:
+                    pts_to_add = fumen.header.b468_b471_branch_points_good
+                elif note.note_type in ['DON', 'KA']:
+                    pts_to_add = fumen.header.b484_b487_branch_points_good_big
+                elif note.note_type == 'Balloon':
+                    pts_to_add = fumen.header.b496_b499_branch_points_balloon
+                elif note.note_type == 'Kusudama':
+                    pts_to_add = fumen.header.b500_b503_branch_points_kusudama
+                else:
+                    pts_to_add = 0  # Drumrolls not relevant for `p` conditions
+                branch_points_measure += pts_to_add
+
+                # Add the note to the branch for this measure
+                measure_fumen.branches[current_branch].notes.append(note)
+                measure_fumen.branches[current_branch].length += 1
 
-            # If drumroll hasn't ended by the end of this measure, increase duration by measure timing
+            # If drumroll hasn't ended by this measure, increase duration
             if current_drumroll:
-                if current_drumroll.duration == 0.0:
-                    current_drumroll.duration += (measure_duration - current_drumroll.pos)
-                    current_drumroll.multimeasure = True
+                # If drumroll spans multiple measures, add full duration
+                if current_drumroll.multimeasure:
+                    current_drumroll.duration += measure_fumen.duration
+                # Otherwise, add the partial duration spanned by the drumroll
                 else:
-                    current_drumroll.duration += measure_duration
-
-            measure_fumen.branches[current_branch].length = note_counter
-            total_notes[current_branch] += note_counter
+                    current_drumroll.multimeasure = True
+                    current_drumroll.duration += (measure_fumen.duration -
+                                                  current_drumroll.pos)
 
-    # Set song-specific metadata
-    fumen.header.b512_b515_number_of_measures = len(fumen.measures)
-    fumen.header.b432_b435_has_branches = int(all([len(b) for b in processed_tja_branches.values()]))
+    # Compute the header bytes that dictate the soul gauge bar behavior
     fumen.header.set_hp_bytes(total_notes['normal'], tja.course, tja.level)
 
-    # If song has only drumroll branching conditions, then only drumrolls should contribute to branching
-    if all([condition[0] == 'r' for condition in branch_conditions]):
+    # If song has only drumroll branching conditions (also allowing percentage
+    # conditions that force a level up/level down), then set the header bytes
+    # so that only drumrolls contribute to branching.
+    drumroll_only = branch_conditions != [] and all([
+        (cond[0] == 'r') or
+        (cond[0] == 'p' and cond[1] == 0.0 and cond[2] == 0.0) or
+        (cond[0] == 'p' and cond[1] > 1.00 and cond[2] > 1.00)
+        for cond in branch_conditions
+    ])
+    if drumroll_only:
         fumen.header.b468_b471_branch_points_good = 0
         fumen.header.b484_b487_branch_points_good_big = 0
         fumen.header.b472_b475_branch_points_ok = 0
         fumen.header.b488_b491_branch_points_ok_big = 0
         fumen.header.b496_b499_branch_points_balloon = 0
         fumen.header.b500_b503_branch_points_kusudama = 0
 
-    # Compute the ratio between normal and advanced/master branches (just in case the note counts differ)
-    if total_notes['advanced']:
-        fumen.header.b460_b463_normal_professional_ratio = int(65536 * (total_notes['normal'] / total_notes['advanced']))
+    # Alternatively, if the song has only percentage-based conditions, then set
+    # the header bytes so that only notes and balloons contribute to branching.
+    percentage_only = branch_conditions != [] and all([
+        (condition[0] != 'r')
+        for condition in branch_conditions
+    ])
+    if percentage_only:
+        fumen.header.b480_b483_branch_points_drumroll = 0
+        fumen.header.b492_b495_branch_points_drumroll_big = 0
+
+    # Compute the ratio between normal and professional/master branches
+    if total_notes['professional']:
+        fumen.header.b460_b463_normal_professional_ratio = \
+            int(65536 * (total_notes['normal'] / total_notes['professional']))
     if total_notes['master']:
-        fumen.header.b464_b467_normal_master_ratio = int(65536 * (total_notes['normal'] / total_notes['master']))
+        fumen.header.b464_b467_normal_master_ratio = \
+            int(65536 * (total_notes['normal'] / total_notes['master']))
 
     return fumen
```

### Comparing `tja2fumen-0.5.4/src/tja2fumen/parsers.py` & `tja2fumen-0.6.0/src/tja2fumen/parsers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,301 +1,399 @@
 import os
 import re
+import struct
 from copy import deepcopy
 
-from tja2fumen.utils import read_struct, short_hex
-from tja2fumen.constants import NORMALIZE_COURSE, TJA_NOTE_TYPES, BRANCH_NAMES, FUMEN_NOTE_TYPES
-from tja2fumen.types import (TJASong, TJAMeasure, TJAData,
-                             FumenCourse, FumenMeasure, FumenBranch, FumenNote, FumenHeader)
-
-########################################################################################################################
-# TJA-parsing functions ( Original source: https://github.com/WHMHammer/tja-tools/blob/master/src/js/parseTJA.js)
-########################################################################################################################
+from tja2fumen.types import (TJASong, TJAMeasure, TJAData, FumenCourse,
+                             FumenMeasure, FumenBranch, FumenNote, FumenHeader)
+from tja2fumen.constants import (NORMALIZE_COURSE, COURSE_NAMES, BRANCH_NAMES,
+                                 TJA_NOTE_TYPES, FUMEN_NOTE_TYPES)
+
+###############################################################################
+#                          TJA-parsing functions                              #
+###############################################################################
 
 
 def parse_tja(fname_tja):
+    """Read in lines of a .tja file and load them into a TJASong object."""
     try:
         tja_text = open(fname_tja, "r", encoding="utf-8-sig").read()
     except UnicodeDecodeError:
         tja_text = open(fname_tja, "r", encoding="shift-jis").read()
 
-    lines = [line for line in tja_text.splitlines() if line.strip() != '']
-    parsed_tja = get_course_data(lines)
-    for course in parsed_tja.courses.values():
-        parse_course_measures(course)
+    tja_lines = [line for line in tja_text.splitlines() if line.strip() != '']
+    tja = split_tja_lines_into_courses(tja_lines)
+    for course in tja.courses.values():
+        parse_tja_course_data(course)
 
-    return parsed_tja
+    return tja
 
 
-def get_course_data(lines):
-    parsed_tja = None
-    current_course = ''
-    current_course_cached = ''
-    song_bpm = 0
-    song_offset = 0
+def split_tja_lines_into_courses(lines):
+    """
+    Parse TJA metadata in order to split TJA lines into separate courses.
 
-    for line in lines:
-        # Case 1: Header metadata
-        match_header = re.match(r"^([A-Z]+):(.*)", line)
-        if match_header:
-            name_upper = match_header.group(1).upper()
-            value = match_header.group(2).strip()
-
-            # Global header fields
-            if name_upper in ['BPM', 'OFFSET']:
-                if name_upper == 'BPM':
-                    song_bpm = value
-                elif name_upper == 'OFFSET':
-                    song_offset = value
-                if song_bpm and song_offset:
-                    parsed_tja = TJASong(song_bpm, song_offset)
+    In TJA files, metadata lines are denoted by a colon (':'). These lines
+    provide general info about the song (BPM, TITLE, OFFSET, etc.). They also
+    define properties for each course in the song (difficulty, level, etc.).
+
+    This function processes each line of metadata, and assigns the metadata
+    to TJACourse objects (one for each course). To separate each course, this
+    function uses the `COURSE:` metadata and any `#START P1/P2` commands,
+    resulting in the following structure:
+
+    TJASong
+    ├─ TJACourse (e.g. Ura)
+    │  ├─ Course metadata (level, balloons, scoreinit, scorediff, etc.)
+    │  └─ Unparsed data (notes, commands)
+    ├─ TJACourse (e.g. Ura-P1)
+    ├─ TJACourse (e.g. Ura-P2)
+    ├─ TJACourse (e.g. Oni)
+    ├─ TJACourse (e.g. Hard)
+    └─ ...
 
-            # Course-specific header fields
-            elif name_upper == 'COURSE':
+    The data for each TJACourse can then be parsed individually using the
+    `parse_tja_course_data()` function.
+    """
+    # Strip leading/trailing whitespace and comments ('// Comment')
+    lines = [line.split("//")[0].strip() for line in lines
+             if line.split("//")[0].strip()]
+
+    # Initialize song with BPM and OFFSET global metadata
+    bpm = [line.split(":")[1] for line in lines
+           if line.startswith("BPM")][0]
+    offset = [line.split(":")[1] for line in lines
+              if line.startswith("OFFSET")][0]
+    parsed_tja = TJASong(bpm, offset)
+
+    current_course = ''
+    current_course_basename = ''
+    for line in lines:
+        # Only metadata and #START commands are relevant for this function
+        match_metadata = re.match(r"^([A-Z]+):(.*)", line)
+        match_start = re.match(r"^#START(?:\s+(.+))?", line)
+
+        # Case 1: Metadata lines
+        if match_metadata:
+            name_upper = match_metadata.group(1).upper()
+            value = match_metadata.group(2).strip()
+
+            # Course-specific metadata fields
+            if name_upper == 'COURSE':
+                if value not in NORMALIZE_COURSE.keys():
+                    raise ValueError(f"Invalid COURSE value: '{value}'")
                 current_course = NORMALIZE_COURSE[value]
-                current_course_cached = current_course
-                if current_course not in parsed_tja.courses.keys():
-                    raise ValueError()
+                current_course_basename = current_course
             elif name_upper == 'LEVEL':
-                parsed_tja.courses[current_course].level = int(value) if value else 0
-            # NB: If there are multiple SCOREINIT/SCOREDIFF values, use the last one (shinuti)
+                if value not in ['1', '2', '3', '4', '5',
+                                 '6', '7', '8', '9', '10']:
+                    raise ValueError(f"Invalid LEVEL value: '{value}")
+                parsed_tja.courses[current_course].level = int(value)
             elif name_upper == 'SCOREINIT':
-                parsed_tja.courses[current_course].score_init = int(value.split(",")[-1]) if value else 0
+                parsed_tja.courses[current_course].score_init = \
+                    int(value.split(",")[-1]) if value else 0
             elif name_upper == 'SCOREDIFF':
-                parsed_tja.courses[current_course].score_diff = int(value.split(",")[-1]) if value else 0
+                parsed_tja.courses[current_course].score_diff = \
+                    int(value.split(",")[-1]) if value else 0
             elif name_upper == 'BALLOON':
                 if value:
                     balloons = [int(v) for v in value.split(",") if v]
                     parsed_tja.courses[current_course].balloon = balloons
             elif name_upper == 'STYLE':
-                # Reset the course name to remove "P1/P2" that may have been added by a previous STYLE:DOUBLE chart
+                # Reset the course name to remove "P1/P2" that may have been
+                # added by a previous STYLE:DOUBLE chart
                 if value == 'Single':
-                    current_course = current_course_cached
+                    current_course = current_course_basename
             else:
-                pass  # Ignore other header fields such as 'TITLE', 'SUBTITLE', 'WAVE', etc.
+                pass  # Ignore 'TITLE', 'SUBTITLE', 'WAVE', etc.
 
-        # Case 2: Commands and note data (to be further processed course-by-course later on)
-        elif not re.match(r"//.*", line):  # Exclude comment-only lines ('//')
-            match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
-            match_notes = re.match(r"^(([0-9]|A|B|C|F|G)*,?).*$", line)
-            if match_command:
-                name_upper = match_command.group(1).upper()
-                value = match_command.group(2).strip() if match_command.group(2) else ''
-                # For STYLE:Double, #START P1/P2 indicates the start of a new chart
-                # But, we want multiplayer charts to inherit the metadata from the course as a whole, so we deepcopy
-                if name_upper == "START":
-                    if value in ["P1", "P2"]:
-                        current_course = current_course_cached + value
-                        parsed_tja.courses[current_course] = deepcopy(parsed_tja.courses[current_course_cached])
-                        parsed_tja.courses[current_course].data = list()  # Keep the metadata, but reset the note data
-                        value = ''  # Once we've made the new course, we can reset this to a normal #START command
-                    elif value:
-                        raise ValueError(f"Invalid value '{value}' for #START command.")
-            elif match_notes:
-                name_upper = 'NOTES'
-                value = match_notes.group(1)
-            parsed_tja.courses[current_course].data.append(TJAData(name_upper, value))
-            
-    # If a course has no song data, then this is likely because the course has "STYLE: Double" but no "STYLE: Single".
-    # To fix this, we copy over the P1 chart from "STYLE: Double" to fill the "STYLE: Single" role.
-    for course_name, course in parsed_tja.courses.items():
-        if not course.data:
-            if course_name+"P1" in parsed_tja.courses.keys():
-                parsed_tja.courses[course_name] = deepcopy(parsed_tja.courses[course_name+"P1"])
+        # Case 2: #START commands
+        elif match_start:
+            value = match_start.group(1) if match_start.group(1) else ''
+            # For STYLE:Double, #START P1/P2 indicates the start of a new
+            # chart. But, we want multiplayer charts to inherit the
+            # metadata from the course as a whole, so we deepcopy the
+            # existing course for that difficulty.
+            if value in ["P1", "P2"]:
+                current_course = current_course_basename + value
+                parsed_tja.courses[current_course] = \
+                    deepcopy(parsed_tja.courses[current_course_basename])
+                parsed_tja.courses[current_course].data = list()
+            elif value:
+                raise ValueError(f"Invalid value '{value}' for #START.")
 
-    # Remove any charts (e.g. P1/P2) not present in the TJA file
-    for course_name in [k for k, v in parsed_tja.courses.items() if not v.data]:
+            # Since P1/P2 has been handled, we can just use a normal '#START'
+            parsed_tja.courses[current_course].data.append("#START")
+
+        # Case 3: For other commands and data, simply copy as-is (parse later)
+        else:
+            parsed_tja.courses[current_course].data.append(line)
+
+    # If a .tja has "STYLE: Double" but no "STYLE: Single", then it will be
+    # missing data for the "single player" chart. To fix this, we copy over
+    # the P1 chart from "STYLE: Double" to fill the "STYLE: Single" role.
+    for course_name in COURSE_NAMES:
+        course_single_player = parsed_tja.courses[course_name]
+        course_player_one = parsed_tja.courses[course_name+"P1"]
+        if course_player_one.data and not course_single_player.data:
+            parsed_tja.courses[course_name] = deepcopy(course_player_one)
+
+    # Remove any charts (e.g. P1/P2) not present in the TJA file (empty data)
+    for course_name in [k for k, v in parsed_tja.courses.items()
+                        if not v.data]:
         del parsed_tja.courses[course_name]
 
     return parsed_tja
 
 
-def parse_course_measures(course):
-    # Check if the course has branches or not
-    has_branches = True if [l for l in course.data if l.name == 'BRANCHSTART'] else False
+def parse_tja_course_data(course):
+    """
+    Parse course data (notes, commands) into a nested song structure.
+
+    The goal of this function is to take raw note and command strings
+    (e.g. '1020,', '#BPMCHANGE') and parse their values into appropriate
+    types (e.g. lists, ints, floats, etc.).
+
+    This function also processes measure separators (',') and branch commands
+    ('#BRANCHSTART`, '#N`, '#E', '#M') to split the data into branches and
+    measures, resulting in the following structure:
+
+    TJACourse
+    ├─ TJABranch ('normal')
+    │  ├─ TJAMeasure
+    │  │  ├─ TJAData (notes, commands)
+    │  │  ├─ TJAData
+    │  │  └─ ...
+    │  ├─ TJAMeasure
+    │  ├─ TJAMeasure
+    │  └─ ...
+    ├─ TJABranch ('professional')
+    └─ TJABranch ('master')
+
+    This provides a faithful, easy-to-inspect tree-style representation of the
+    branches and measures within each course of the .tja file.
+    """
+    has_branches = bool([d for d in course.data if d.startswith('#BRANCH')])
     current_branch = 'all' if has_branches else 'normal'
     branch_condition = None
-    flag_levelhold = False
 
     # Process course lines
     idx_m = 0
     idx_m_branchstart = 0
     for idx_l, line in enumerate(course.data):
+        # 0. Check to see whether line is a command or note data
+        command, value, notes = None, None, None
+        match_command = re.match(r"^#([A-Z]+)(?:\s+(.+))?", line)
+        if match_command:
+            command, value = match_command.groups()
+        else:
+            notes = line  # If not a command, then line must be note data
+
         # 1. Parse measure notes
-        if line.name == 'NOTES':
-            notes = line.value
-            # If measure has ended, then add notes to the current measure, then start a new one by incrementing idx_m
+        if notes:
+            # If measure has ended, then add notes to the current measure,
+            # then start a new measure by incrementing idx_m
             if notes.endswith(','):
-                for branch in course.branches.keys() if current_branch == 'all' else [current_branch]:
+                for branch in (course.branches.keys()
+                               if current_branch == 'all'
+                               else [current_branch]):
                     course.branches[branch][idx_m].notes += notes[0:-1]
                     course.branches[branch].append(TJAMeasure())
                 idx_m += 1
             # Otherwise, keep adding notes to the current measure ('idx_m')
             else:
-                for branch in course.branches.keys() if current_branch == 'all' else [current_branch]:
+                for branch in (course.branches.keys()
+                               if current_branch == 'all'
+                               else [current_branch]):
                     course.branches[branch][idx_m].notes += notes
 
         # 2. Parse measure commands that produce an "event"
-        elif line.name in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF', 'DELAY',
-                           'SCROLL', 'BPMCHANGE', 'MEASURE', 'SECTION', 'BRANCHSTART']:
+        elif command in ['GOGOSTART', 'GOGOEND', 'BARLINEON', 'BARLINEOFF',
+                         'DELAY', 'SCROLL', 'BPMCHANGE', 'MEASURE',
+                         'LEVELHOLD', 'SECTION', 'BRANCHSTART']:
             # Get position of the event
-            for branch in course.branches.keys() if current_branch == 'all' else [current_branch]:
+            for branch in (course.branches.keys() if current_branch == 'all'
+                           else [current_branch]):
                 pos = len(course.branches[branch][idx_m].notes)
 
             # Parse event type
-            if line.name == 'GOGOSTART':
+            if command == 'GOGOSTART':
                 current_event = TJAData('gogo', '1', pos)
-            elif line.name == 'GOGOEND':
+            elif command == 'GOGOEND':
                 current_event = TJAData('gogo', '0', pos)
-            elif line.name == 'BARLINEON':
+            elif command == 'BARLINEON':
                 current_event = TJAData('barline', '1', pos)
-            elif line.name == 'BARLINEOFF':
+            elif command == 'BARLINEOFF':
                 current_event = TJAData('barline', '0', pos)
-            elif line.name == 'DELAY':
-                current_event = TJAData('delay', float(line.value), pos)
-            elif line.name == 'SCROLL':
-                current_event = TJAData('scroll', float(line.value), pos)
-            elif line.name == 'BPMCHANGE':
-                current_event = TJAData('bpm', float(line.value), pos)
-            elif line.name == 'MEASURE':
-                current_event = TJAData('measure', line.value, pos)
-            elif line.name == 'SECTION':
-                if branch_condition is None:
-                    current_event = TJAData('section', 'not_available', pos)
-                else:
-                    current_event = TJAData('section', branch_condition, pos)
-                # If the command immediately after #SECTION is #BRANCHSTART, then we need to make sure that #SECTION
-                # is put on every branch. (We can't do this unconditionally because #SECTION commands can also exist
-                # in isolation in the middle of separate branches.)
-                if course.data[idx_l+1].name == 'BRANCHSTART':
+            elif command == 'DELAY':
+                current_event = TJAData('delay', float(value), pos)
+            elif command == 'SCROLL':
+                current_event = TJAData('scroll', float(value), pos)
+            elif command == 'BPMCHANGE':
+                current_event = TJAData('bpm', float(value), pos)
+            elif command == 'MEASURE':
+                current_event = TJAData('measure', value, pos)
+            elif command == 'LEVELHOLD':
+                current_event = TJAData('levelhold', None, pos)
+            elif command == 'SECTION':
+                # If #SECTION occurs before a #BRANCHSTART, then ensure that
+                # it's present on every branch. Otherwise, #SECTION will only
+                # be present on the current branch, and so the `branch_info`
+                # values won't be correctly set for the other two branches.
+                if course.data[idx_l+1].startswith('#BRANCHSTART'):
+                    current_event = TJAData('section', None, pos)
                     current_branch = 'all'
-            elif line.name == 'BRANCHSTART':
-                if flag_levelhold:
-                    continue
-                current_branch = 'all'  # Ensure that the #BRANCHSTART command is present for all branches
-                branch_condition = line.value.split(',')
+                # Otherwise, #SECTION exists in isolation. In this case, to
+                # reset the accuracy, we just repeat the previous #BRANCHSTART.
+                else:
+                    current_event = TJAData('branch_start', branch_condition,
+                                            pos)
+            elif command == 'BRANCHSTART':
+                # Ensure that the #BRANCHSTART command is added to all branches
+                current_branch = 'all'
+                branch_condition = value.split(',')
                 if branch_condition[0] == 'r':  # r = drumRoll
-                    branch_condition[1] = int(branch_condition[1])  # # of drumrolls
-                    branch_condition[2] = int(branch_condition[2])  # # of drumrolls
+                    branch_condition[1] = int(branch_condition[1])  # drumrolls
+                    branch_condition[2] = int(branch_condition[2])  # drumrolls
                 elif branch_condition[0] == 'p':  # p = Percentage
                     branch_condition[1] = float(branch_condition[1]) / 100  # %
                     branch_condition[2] = float(branch_condition[2]) / 100  # %
                 current_event = TJAData('branch_start', branch_condition, pos)
-                idx_m_branchstart = idx_m  # Preserve the index of the BRANCHSTART command to re-use for each branch
+                # Preserve the index of the BRANCHSTART command to re-use
+                idx_m_branchstart = idx_m
 
             # Append event to the current measure's events
-            for branch in course.branches.keys() if current_branch == 'all' else [current_branch]:
+            for branch in (course.branches.keys() if current_branch == 'all'
+                           else [current_branch]):
                 course.branches[branch][idx_m].events.append(current_event)
 
-        # 3. Parse commands that don't create an event (e.g. simply changing the current branch)
+        # 3. Parse commands that don't create an event
+        #    (e.g. simply changing the current branch)
         else:
-            if line.name == 'START' or line.name == 'END':
+            if command == 'START' or command == 'END':
                 current_branch = 'all' if has_branches else 'normal'
-                flag_levelhold = False
-            elif line.name == 'LEVELHOLD':
-                flag_levelhold = True
-            elif line.name == 'N':
+            elif command == 'N':
                 current_branch = 'normal'
                 idx_m = idx_m_branchstart
-            elif line.name == 'E':
-                current_branch = 'advanced'
+            elif command == 'E':
+                current_branch = 'professional'
                 idx_m = idx_m_branchstart
-            elif line.name == 'M':
+            elif command == 'M':
                 current_branch = 'master'
                 idx_m = idx_m_branchstart
-            elif line.name == 'BRANCHEND':
+            elif command == 'BRANCHEND':
                 current_branch = 'all'
 
             else:
-                print(f"Ignoring unsupported command '{line.name}'")
+                print(f"Ignoring unsupported command '{command}'")
 
-    # Delete the last measure in the branch if no notes or events were added to it (due to preallocating empty measures)
+    # Delete the last measure in the branch if no notes or events
+    # were added to it (due to preallocating empty measures)
     for branch in course.branches.values():
         if not branch[-1].notes and not branch[-1].events:
             del branch[-1]
 
     # Merge measure data and measure events in chronological order
     for branch_name, branch in course.branches.items():
         for measure in branch:
             notes = [TJAData('note', TJA_NOTE_TYPES[note], i)
-                     for i, note in enumerate(measure.notes) if note != '0']
+                     for i, note in enumerate(measure.notes) if
+                     TJA_NOTE_TYPES[note] != 'Blank']
             events = measure.events
             while notes or events:
                 if events and notes:
                     if notes[0].pos >= events[0].pos:
                         measure.combined.append(events.pop(0))
                     else:
                         measure.combined.append(notes.pop(0))
                 elif events:
                     measure.combined.append(events.pop(0))
                 elif notes:
                     measure.combined.append(notes.pop(0))
 
     # Ensure all branches have the same number of measures
     if has_branches:
-        branch_lens = [len(b) for b in course.branches.values()]
-        if not branch_lens.count(branch_lens[0]) == len(branch_lens):
-            raise ValueError("Branches do not have the same number of measures.")
-
-
-########################################################################################################################
-# Fumen-parsing functions
-########################################################################################################################
+        if len(set([len(b) for b in course.branches.values()])) != 1:
+            raise ValueError(
+                "Branches do not have the same number of measures. (This "
+                "check was performed prior to splitting up the measures due "
+                "to mid-measure commands. Please check the number of ',' you"
+                "have in each branch.)"
+            )
 
-# Fumen format reverse engineering TODOs
-# TODO: Figure out what drumroll bytes are (8 bytes after every drumroll)
-#       NB: fumen2osu.py assumed these were padding bytes, but they're not!! They contain some sort of metadata.
-# TODO: Figure out what the unknown Wii1, Wii4, and PS4 notes represent (just in case they're important somehow)
 
+###############################################################################
+#                          Fumen-parsing functions                            #
+###############################################################################
 
-def read_fumen(fumen_file, exclude_empty_measures=False):
+def parse_fumen(fumen_file, exclude_empty_measures=False):
     """
-    Parse bytes of a fumen .bin file into nested measure, branch, and note dictionaries.
+    Parse bytes of a fumen .bin file into nested measures, branches, and notes.
 
-    For more information on any of the terms used in this function (e.g. score_init, score_diff),
-    please refer to KatieFrog's excellent guide: https://gist.github.com/KatieFrogs/e000f406bbc70a12f3c34a07303eec8b
+    Fumen files use a very strict file structure. Certain values are expected
+    at very specific byte locations in the file. Here, we parse these specific
+    byte locations into the following structure:
+
+    FumenCourse
+    ├─ FumenHeader
+    │  ├─ Timing windows
+    │  ├─ Branch points
+    │  ├─ Soul gauge bytes
+    │  └─ ...
+    ├─ FumenMeasure
+    │  ├─ FumenBranch ('normal')
+    │  │  ├─ FumenNote
+    │  │  ├─ FumenNote
+    │  │  └─ ...
+    │  ├─ FumenBranch ('professional')
+    │  └─ FumenBranch ('master')
+    ├─ FumenMeasure
+    ├─ FumenMeasure
+    └─ ...
     """
     file = open(fumen_file, "rb")
     size = os.fstat(file.fileno()).st_size
 
     song = FumenCourse(
         header=FumenHeader(raw_bytes=file.read(520))
     )
 
     for measure_number in range(song.header.b512_b515_number_of_measures):
         # Parse the measure data using the following `format_string`:
         #   "ffBBHiiiiiii" (12 format characters, 40 bytes per measure)
-        #     - 'f': BPM              (represented by one float (4 bytes))
-        #     - 'f': fumenOffset      (represented by one float (4 bytes))
-        #     - 'B': gogo             (represented by one unsigned char (1 byte))
-        #     - 'B': barline           (represented by one unsigned char (1 byte))
-        #     - 'H': <padding>        (represented by one unsigned short (2 bytes))
-        #     - 'iiiiii': branch_info  (represented by six integers (24 bytes))
-        #     - 'i': <padding>        (represented by one integer (4 bytes)
-        measure_struct = read_struct(file, song.header.order, format_string="ffBBHiiiiiii")
+        #     - 'f': BPM               (one float (4 bytes))
+        #     - 'f': fumenOffset       (one float (4 bytes))
+        #     - 'B': gogo              (one unsigned char (1 byte))
+        #     - 'B': barline           (one unsigned char (1 byte))
+        #     - 'H': <padding>         (one unsigned short (2 bytes))
+        #     - 'iiiiii': branch_info  (six integers (24 bytes))
+        #     - 'i': <padding>         (one integer (4 bytes)
+        measure_struct = read_struct(file, song.header.order,
+                                     format_string="ffBBHiiiiiii")
 
         # Create the measure dictionary using the newly-parsed measure data
         measure = FumenMeasure(
             bpm=measure_struct[0],
-            fumen_offset_start=measure_struct[1],
+            offset_start=measure_struct[1],
             gogo=measure_struct[2],
             barline=measure_struct[3],
             padding1=measure_struct[4],
             branch_info=list(measure_struct[5:11]),
             padding2=measure_struct[11]
         )
 
         # Iterate through the three branch types
         for branch_name in BRANCH_NAMES:
             # Parse the measure data using the following `format_string`:
             #   "HHf" (3 format characters, 8 bytes per branch)
-            #     - 'H': total_notes (represented by one unsigned short (2 bytes))
-            #     - 'H': <padding>  (represented by one unsigned short (2 bytes))
-            #     - 'f': speed      (represented by one float (4 bytes)
-            branch_struct = read_struct(file, song.header.order, format_string="HHf")
+            #     - 'H': total_notes ( one unsigned short (2 bytes))
+            #     - 'H': <padding>  ( one unsigned short (2 bytes))
+            #     - 'f': speed      ( one float (4 bytes)
+            branch_struct = read_struct(file, song.header.order,
+                                        format_string="HHf")
 
             # Create the branch dictionary using the newly-parsed branch data
             total_notes = branch_struct[0]
             branch = FumenBranch(
                 length=total_notes,
                 padding=branch_struct[1],
                 speed=branch_struct[2],
@@ -309,25 +407,19 @@
                 #     - 'f': note position
                 #     - 'i': item
                 #     - 'f': <padding>
                 #     - 'H': score_init
                 #     - 'H': score_diff
                 #     - 'f': duration
                 # NB: 'item' doesn't seem to be used at all in this function.
-                note_struct = read_struct(file, song.header.order, format_string="ififHHf")
-
-                # Validate the note type
-                note_type = note_struct[0]
-                if note_type not in FUMEN_NOTE_TYPES:
-                    raise ValueError("Error: Unknown note type '{0}' at offset {1}".format(
-                        short_hex(note_type).upper(),
-                        hex(file.tell() - 0x18))
-                    )
+                note_struct = read_struct(file, song.header.order,
+                                          format_string="ififHHf")
 
                 # Create the note dictionary using the newly-parsed note data
+                note_type = note_struct[0]
                 note = FumenNote(
                     note_type=FUMEN_NOTE_TYPES[note_type],
                     pos=note_struct[1],
                     item=note_struct[2],
                     padding=note_struct[3],
                 )
 
@@ -338,15 +430,15 @@
                 else:
                     song.score_init = note.score_init = note_struct[4]
                     song.score_diff = note.score_diff = note_struct[5] // 4
 
                 # Drumroll/balloon duration
                 note.duration = note_struct[6]
 
-                # Seek forward 8 bytes to account for padding bytes at the end of drumrolls
+                # Account for padding at the end of drumrolls
                 if note_type == 0x6 or note_type == 0x9 or note_type == 0x62:
                     note.drumroll_bytes = file.read(8)
 
                 # Assign the note to the branch
                 branch.notes.append(note)
 
             # Assign the branch to the measure
@@ -355,16 +447,48 @@
         # Assign the measure to the song
         song.measures.append(measure)
         if file.tell() >= size:
             break
 
     file.close()
 
-    # NB: Official fumens often include empty measures as a way of inserting barlines for visual effect.
-    #     But, TJA authors tend not to add these empty measures, because even without them, the song plays correctly.
-    #     So, in tests, if we want to only compare the timing of the non-empty measures between an official fumen and
-    #     a converted non-official TJA, then it's useful to  exclude the empty measures.
+    # NB: Official fumens often include empty measures as a way of inserting
+    # barlines for visual effect. But, TJA authors tend not to add these empty
+    # measures, because even without them, the song plays correctly. So, in
+    # tests, if we want to only compare the timing of the non-empty measures
+    # between an official fumen and a converted non-official TJA, then it's
+    # useful to exclude the empty measures.
     if exclude_empty_measures:
         song.measures = [m for m in song.measures
-                         if m.branches['normal'].length or m.branches['advanced'].length or m.branches['master'].length]
+                         if m.branches['normal'].length
+                         or m.branches['professional'].length
+                         or m.branches['master'].length]
 
     return song
+
+
+def read_struct(file, order, format_string, seek=None):
+    """
+    Interpret bytes as packed binary data.
+
+    Arguments:
+        - file: The fumen's file object (presumably in 'rb' mode).
+        - order: '<' or '>' (little or big endian).
+        - format_string: String made up of format characters that describes
+                         the data layout. Full list of available characters:
+          (https://docs.python.org/3/library/struct.html#format-characters)
+        - seek: The position of the read pointer to be used within the file.
+
+    Return values:
+        - interpreted_string: A string containing interpreted byte values,
+                              based on the specified 'fmt' format characters.
+    """
+    if seek:
+        file.seek(seek)
+    expected_size = struct.calcsize(order + format_string)
+    byte_string = file.read(expected_size)
+    # One "official" fumen (AC11\deo\deo_n.bin) runs out of data early
+    # This workaround fixes the issue by appending 0's to get the size to match
+    if len(byte_string) != expected_size:
+        byte_string += (b'\x00' * (expected_size - len(byte_string)))
+    interpreted_string = struct.unpack(order + format_string, byte_string)
+    return interpreted_string
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tja2fumen-0.5.4/src/tja2fumen/writers.py` & `tja2fumen-0.6.0/src/tja2fumen/writers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,55 @@
-from tja2fumen.utils import write_struct
+import struct
+
 from tja2fumen.constants import BRANCH_NAMES, FUMEN_TYPE_NOTES
 
 
 def write_fumen(path_out, song):
+    """
+    Write the values in a FumenCourse object to a `.bin` file.
+
+    This operation is the reverse of the `parse_fumen` function. Please refer
+    to that function for more details about the fumen file structure.
+    """
     with open(path_out, "wb") as file:
         file.write(song.header.raw_bytes)
 
         for measure_number in range(len(song.measures)):
             measure = song.measures[measure_number]
-            measure_struct = [measure.bpm, measure.fumen_offset_start, int(measure.gogo), int(measure.barline)]
-            measure_struct.extend([measure.padding1] + measure.branch_info + [measure.padding2])
-            write_struct(file, song.header.order, format_string="ffBBHiiiiiii", value_list=measure_struct)
+            measure_struct = ([measure.bpm, measure.offset_start,
+                               int(measure.gogo), int(measure.barline),
+                               measure.padding1] + measure.branch_info +
+                              [measure.padding2])
+            write_struct(file, song.header.order,
+                         format_string="ffBBHiiiiiii",
+                         value_list=measure_struct)
 
             for branch_number in range(len(BRANCH_NAMES)):
                 branch = measure.branches[BRANCH_NAMES[branch_number]]
                 branch_struct = [branch.length, branch.padding, branch.speed]
-                write_struct(file, song.header.order, format_string="HHf", value_list=branch_struct)
+                write_struct(file, song.header.order,
+                             format_string="HHf",
+                             value_list=branch_struct)
 
                 for note_number in range(branch.length):
                     note = branch.notes[note_number]
-                    note_struct = [FUMEN_TYPE_NOTES[note.type], note.pos, note.item, note.padding]
+                    note_struct = [FUMEN_TYPE_NOTES[note.note_type], note.pos,
+                                   note.item, note.padding]
                     if note.hits:
-                        note_struct.extend([note.hits, note.hits_padding, note.duration])
+                        extra_vals = [note.hits, note.hits_padding]
                     else:
-                        note_struct.extend([note.score_init, note.score_diff * 4, note.duration])
-                    write_struct(file, song.header.order, format_string="ififHHf", value_list=note_struct)
+                        extra_vals = [note.score_init, note.score_diff * 4]
+                    note_struct.extend(extra_vals + [note.duration])
+                    write_struct(file, song.header.order,
+                                 format_string="ififHHf",
+                                 value_list=note_struct)
 
-                    if note.type.lower() == "drumroll":
+                    if note.note_type.lower() == "drumroll":
                         file.write(note.drumroll_bytes)
+
+
+def write_struct(file, order, format_string, value_list, seek=None):
+    """Pack (int, float, etc.) values into a string of bytes, then write."""
+    if seek:
+        file.seek(seek)
+    packed_bytes = struct.pack(order + format_string, *value_list)
+    file.write(packed_bytes)
```

