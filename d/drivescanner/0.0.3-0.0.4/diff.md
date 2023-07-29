# Comparing `tmp/drivescanner-0.0.3.tar.gz` & `tmp/drivescanner-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drivescanner-0.0.3.tar", last modified: Mon Apr  3 10:58:47 2023, max compression
+gzip compressed data, was "drivescanner-0.0.4.tar", last modified: Sat Jul 29 18:21:22 2023, max compression
```

## Comparing `drivescanner-0.0.3.tar` & `drivescanner-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 10:58:47.329556 drivescanner-0.0.3/
--rw-rw-rw-   0        0        0    35821 2023-03-10 06:45:55.000000 drivescanner-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2433 2023-04-03 10:58:47.327003 drivescanner-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2023-03-16 11:40:15.000000 drivescanner-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 10:58:47.277105 drivescanner-0.0.3/drivescanner/
--rw-rw-rw-   0        0        0      479 2023-03-10 06:45:55.000000 drivescanner-0.0.3/drivescanner/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-03-10 06:45:55.000000 drivescanner-0.0.3/drivescanner/evaluate.py
--rw-rw-rw-   0        0        0     7338 2023-03-10 06:45:55.000000 drivescanner-0.0.3/drivescanner/file_index.py
--rw-rw-rw-   0        0        0     4294 2023-03-10 06:45:55.000000 drivescanner-0.0.3/drivescanner/ingest.py
--rw-rw-rw-   0        0        0    16311 2023-02-07 09:52:45.000000 drivescanner-0.0.3/drivescanner/rules.py
--rw-rw-rw-   0        0        0     2046 2023-03-10 06:45:55.000000 drivescanner-0.0.3/drivescanner/scan.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:58:47.325650 drivescanner-0.0.3/drivescanner.egg-info/
--rw-rw-rw-   0        0        0     2433 2023-04-03 10:58:46.000000 drivescanner-0.0.3/drivescanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-03 10:58:47.000000 drivescanner-0.0.3/drivescanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 10:58:46.000000 drivescanner-0.0.3/drivescanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-04-03 10:58:46.000000 drivescanner-0.0.3/drivescanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-03 10:58:46.000000 drivescanner-0.0.3/drivescanner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 10:58:47.329556 drivescanner-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1426 2023-03-16 11:40:15.000000 drivescanner-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 18:21:22.909322 drivescanner-0.0.4/
+-rw-rw-rw-   0        0        0    35821 2023-03-10 06:45:55.000000 drivescanner-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2454 2023-07-29 18:21:22.903980 drivescanner-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1960 2023-06-16 19:16:27.000000 drivescanner-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 18:21:22.703089 drivescanner-0.0.4/drivescanner/
+-rw-rw-rw-   0        0        0      107 2023-06-26 15:06:36.000000 drivescanner-0.0.4/drivescanner/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-03-10 06:45:55.000000 drivescanner-0.0.4/drivescanner/evaluate.py
+-rw-rw-rw-   0        0        0     7700 2023-06-18 07:34:11.000000 drivescanner-0.0.4/drivescanner/file_index.py
+-rw-rw-rw-   0        0        0     8520 2023-07-29 18:19:49.000000 drivescanner-0.0.4/drivescanner/ingest.py
+-rw-rw-rw-   0        0        0    16303 2023-07-29 18:11:32.000000 drivescanner-0.0.4/drivescanner/rules.py
+-rw-rw-rw-   0        0        0     3567 2023-07-29 18:11:32.000000 drivescanner-0.0.4/drivescanner/scan.py
+drwxrwxrwx   0        0        0        0 2023-07-29 18:21:22.756583 drivescanner-0.0.4/drivescanner.egg-info/
+-rw-rw-rw-   0        0        0     2454 2023-07-29 18:21:22.000000 drivescanner-0.0.4/drivescanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-29 18:21:22.000000 drivescanner-0.0.4/drivescanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 18:21:22.000000 drivescanner-0.0.4/drivescanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-07-29 18:21:22.000000 drivescanner-0.0.4/drivescanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 18:21:22.000000 drivescanner-0.0.4/drivescanner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 18:21:22.909322 drivescanner-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-07-28 06:50:17.000000 drivescanner-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 18:21:22.900940 drivescanner-0.0.4/tests/
+-rw-rw-rw-   0        0        0    34016 2023-06-18 07:34:11.000000 drivescanner-0.0.4/tests/test_file_index.py
+-rw-rw-rw-   0        0        0    17014 2023-06-18 07:34:11.000000 drivescanner-0.0.4/tests/test_ingest.py
+-rw-rw-rw-   0        0        0    14426 2023-06-18 07:34:11.000000 drivescanner-0.0.4/tests/test_rules.py
+-rw-rw-rw-   0        0        0     7572 2023-06-18 07:34:11.000000 drivescanner-0.0.4/tests/test_scan.py
```

### Comparing `drivescanner-0.0.3/LICENSE` & `drivescanner-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drivescanner-0.0.3/PKG-INFO` & `drivescanner-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: drivescanner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scan your filesystem to look for files that are a potential GDPR risk
 Home-page: https://dev.azure.com/Cmotions/Packages/_git/DriveScanner
-Author: Wouter van Gils, Wim Verboom, Sem Frankenberg, Steven Goos, Rick Flamand, Jeanine Schoonemann
+Author: Wouter van Gils, Wim Verboom, Sem Frankenberg, Rick Flamand, Jeanine Schoonemann, Kjeld Vissers, Philip Vermeij, Matthijs Otten
 Author-email: service@cmotions.nl
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DriveScanner
@@ -51,9 +51,9 @@
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 
 ## License
 [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
 
 ## Contributors
-Jeanine Schoonemann, Rick Flamand, Sem Frankenberg, Steven Goos, Wim Verboom and Wouter van Gils<br>
+Jeanine Schoonemann, Rick Flamand, Sem Frankenberg, Wim Verboom and Wouter van Gils<br>
 [Contact us](mailto:info@theanalyticslab.nl)
```

### Comparing `drivescanner-0.0.3/README.md` & `drivescanner-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 
 ## License
 [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
 
 ## Contributors
-Jeanine Schoonemann, Rick Flamand, Sem Frankenberg, Steven Goos, Wim Verboom and Wouter van Gils<br>
+Jeanine Schoonemann, Rick Flamand, Sem Frankenberg, Wim Verboom and Wouter van Gils<br>
 [Contact us](mailto:info@theanalyticslab.nl)
```

### Comparing `drivescanner-0.0.3/drivescanner/evaluate.py` & `drivescanner-0.0.4/drivescanner/evaluate.py`

 * *Files identical despite different names*

### Comparing `drivescanner-0.0.3/drivescanner/file_index.py` & `drivescanner-0.0.4/drivescanner/file_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 import pandas as pd
 import hashlib
 from collections import Counter
 from pathlib import Path
 
+
 def _replace_backslash(dir_path: str) -> str:
     """
     It takes a string as input and returns a string with all the backslashes replaced with forward
     slashes
 
     Args:
       dir_path (str): The path to the directory you want to convert.
@@ -31,24 +32,28 @@
       A hash of the text.
     """
     return str(hashlib.md5(text.encode("utf-8")).hexdigest())
 
 
 def _get_extension(filepath: str) -> str:
     """
-    It takes a filepath as a string, splits it into the filename and extension, converts the extension
-    to lowercase, and removes the leading period
+    It takes a filepath as a string, splits it into the filename and extension, and converts
+    the extension to lowercase
 
     Args:
       filepath (str): The path to the file you want to get the extension of.
 
     Returns:
       The file extension of the filepath.
     """
-    return os.path.splitext(filepath)[1].lower().replace(".", "", 1)
+    filename = _replace_backslash(filepath).split("/")[-1]
+    if filename.find(".") > -1:
+        return filename.split(".")[-1].lower()
+    else:
+        return ""
 
 
 def _get_extension_list(list_files: list[str]) -> list[str]:
     """
     It takes a list of files, and returns a list with only the file extensions
 
     Args:
@@ -100,23 +105,23 @@
     ), "Input should be a list of strings"
     assert len(list_files) > 0, "Input is an empty list"
 
     all_sizes = list(map(_get_filesize, list_files))
     return all_sizes
 
 
-def list_all_files(dir_path: str) -> list[str]:
+def list_all_files(dir_path: str) -> dict:
     """
-    It takes a directory path as input and returns a list of file paths.
+    It takes a directory path as input and returns a dict of file paths.
 
     Args:
       dir_path (str): The path to the directory containing the files.
 
     Returns:
-      A list of strings.
+      A dict of strings.
     """
     dir_path = _replace_backslash(dir_path)
 
     if not os.path.exists(dir_path):
         raise ValueError(f"The directory doesn't exist.")
 
     if not os.path.isdir(dir_path):
@@ -125,55 +130,93 @@
     file_paths = []
     for dirname, _, files in os.walk(dir_path):
         file_paths += [os.path.join(dirname, entry) for entry in files]
 
     if len(file_paths) == 0:
         raise ValueError(f"Could not find any files in the directory.")
 
-    return file_paths
+    file_paths = list(map(_replace_backslash, file_paths))
 
+    return _create_file_dict(file_paths)
 
-def extension_stats(list_files: list[str]) -> pd.DataFrame:
+
+def extension_stats(dict_files: list[str]) -> pd.DataFrame:
     """
     It takes a list of files and returns a dataframe with the number of files per extension
 
     Args:
       list_files (list[str]): list[str]
 
     Returns:
       A dataframe with the extension and the count of files with that extension.
     """
-    all_extensions = _get_extension_list(list_files=list_files)
+    all_extensions = [d["extension"] for d in dict_files.values()]
 
     # count nr of files per extensions
     count_extensions = Counter([ext for ext in all_extensions])
     df_ext_stats = pd.DataFrame.from_dict(
         count_extensions, orient="index"
     ).reset_index()
     df_ext_stats.columns = ["extension", "count"]
     df_ext_stats = df_ext_stats.sort_values(by="count", ascending=False)
     return df_ext_stats
 
 
-def select_files(
-    list_files: list[str], include: list[str] = None, exclude: list[str] = None
-) -> list[str]:
+def _create_file_dict(list_files: list[str]) -> dict:
     """
-    It takes a list of files, and returns a list of files that have extensions that are in the include
-    list, but not in the exclude list
+    It takes a list of file paths and returns a dictionary of file paths with their corresponding hash, extension and size
 
     Args:
       list_files (list[str]): list[str]
+
+    Returns:
+      A dictionary of dictionaries with information about the files.
+    """
+    all_extensions = _get_extension_list(list_files=list_files)
+    all_sizes = _get_filesize_list(list_files=list_files)
+    file_dict = {
+        _create_hash(list_files[i]): {
+            "filepath": list_files[i],
+            "filename": Path(list_files[i]).name,
+            "extension": all_extensions[i],
+            "filesize": all_sizes[i],
+        }
+        for i in range(len(list_files))
+    }
+    return file_dict
+
+
+def select_files(
+    dict_files: dict,
+    include: list[str] = None,
+    exclude: list[str] = None,
+    size_cap_mb: float = None,
+) -> dict:
+    """
+    It takes a dict of files, and returns a list of files that have extensions that are in the include
+    list, but not in the exclude list.
+    Optionally only select files of less MB than stated in the size_cap_mb.
+
+    Args:
+      dict_files (dict): dict
       include (list[str]): list[str] = None
       exclude (list[str]): list[str] = None
+      size_cap_mb (float): float = None
 
     Returns:
-      list_files
+      capped_file_list
     """
 
+    if size_cap_mb is not None:
+        dict_files = {
+            k: v
+            for k, v in dict_files.items()
+            if (v["filesize"] == None) or (v["filesize"] / 1024 / 1000 <= size_cap_mb)
+        }
+
     if include is not None:
         assert isinstance(
             include, list
         ), "Include parameter should be a list of strings"
         assert all(
             isinstance(elem, str) for elem in include
         ), "Include parameter should be a list of strings"
@@ -187,52 +230,20 @@
         assert all(
             isinstance(elem, str) for elem in exclude
         ), "Exclude parameter should be a list of strings"
         assert len(exclude) > 0, "Exclude parameter is an empty list"
         exclude = [elem.lower() for elem in exclude]
 
     if (include is not None) and (exclude is not None):
-        list_files = [
-            entry
-            for entry, ext in zip(list_files, _get_extension_list(list_files))
-            if (ext in include) & (ext not in exclude)
-        ]
-    elif (include is not None) and (exclude is None):
-        list_files = [
-            entry
-            for entry, ext in zip(list_files, _get_extension_list(list_files))
-            if ext in include
-        ]
+        dict_files = {
+            k: v
+            for k, v in dict_files.items()
+            if (v["extension"] in include) and (v["extension"] not in exclude)
+        }
     elif (include is None) and (exclude is not None):
-        list_files = [
-            entry
-            for entry, ext in zip(list_files, _get_extension_list(list_files))
-            if ext not in exclude
-        ]
+        dict_files = {k: v for k, v in dict_files.items() if (v["extension"] not in exclude)}
+    elif (include is not None) and (exclude is None):
+        dict_files = {k: v for k, v in dict_files.items() if (v["extension"] in include)}
     else:
-        list_files
-
-    return list_files
-
-
-def create_file_dict(list_files: list[str]) -> dict:
-    """
-    It takes a list of file paths and returns a dictionary of file paths with their corresponding hash, extension and size
+        dict_files
 
-    Args:
-      list_files (list[str]): list[str]
-
-    Returns:
-      A dictionary of dictionaries with information about the files.
-    """
-    all_extensions = _get_extension_list(list_files=list_files)
-    all_sizes = _get_filesize_list(list_files=list_files)
-    file_dict = {
-        _create_hash(list_files[i]): {
-            "filepath": list_files[i],
-            "filename": Path(list_files[i]).name,
-            "extension": all_extensions[i],
-            "filesize": all_sizes[i],
-        }
-        for i in range(len(list_files))
-    }
-    return file_dict
+    return dict_files
```

### Comparing `drivescanner-0.0.3/drivescanner/rules.py` & `drivescanner-0.0.4/drivescanner/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
         output_dict[type] = []
 
     # extract iban from text
     iban_numbers = _extract_iban(text_file)
     output_dict["iban"] += iban_numbers
     text_file = _remove_entities(text_file, iban_numbers)
 
-    # extract bsn numbers from text
+    # extract bsn from text
     bsn_numbers = _extract_ssn(text_file)
     output_dict["bsn"] += bsn_numbers
     text_file = _remove_entities(text_file, bsn_numbers)
 
     # extract email from text
     emails = _extract_email(text_file)
     output_dict["email"] += emails
```

### Comparing `drivescanner-0.0.3/drivescanner.egg-info/PKG-INFO` & `drivescanner-0.0.4/drivescanner.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: drivescanner
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scan your filesystem to look for files that are a potential GDPR risk
 Home-page: https://dev.azure.com/Cmotions/Packages/_git/DriveScanner
-Author: Wouter van Gils, Wim Verboom, Sem Frankenberg, Steven Goos, Rick Flamand, Jeanine Schoonemann
+Author: Wouter van Gils, Wim Verboom, Sem Frankenberg, Rick Flamand, Jeanine Schoonemann, Kjeld Vissers, Philip Vermeij, Matthijs Otten
 Author-email: service@cmotions.nl
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DriveScanner
@@ -51,9 +51,9 @@
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 
 ## License
 [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
 
 ## Contributors
-Jeanine Schoonemann, Rick Flamand, Sem Frankenberg, Steven Goos, Wim Verboom and Wouter van Gils<br>
+Jeanine Schoonemann, Rick Flamand, Sem Frankenberg, Wim Verboom and Wouter van Gils<br>
 [Contact us](mailto:info@theanalyticslab.nl)
```

