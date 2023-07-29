# Comparing `tmp/wordcel-0.0.2.tar.gz` & `tmp/wordcel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordcel-0.0.2.tar", max compression
+gzip compressed data, was "wordcel-0.0.3.tar", max compression
```

## Comparing `wordcel-0.0.2.tar` & `wordcel-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-25 01:08:30.881980 wordcel-0.0.2/LICENSE
--rw-r--r--   0        0        0     2783 2023-07-25 21:14:13.262827 wordcel-0.0.2/README.md
--rw-r--r--   0        0        0      333 2023-07-26 01:15:24.770466 wordcel-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 00:46:00.681902 wordcel-0.0.2/wordcel/__init__.py
--rw-r--r--   0        0        0     2243 2023-07-25 21:36:33.162657 wordcel-0.0.2/wordcel/featurize.py
--rw-r--r--   0        0        0     1042 2023-07-25 00:48:13.299968 wordcel-0.0.2/wordcel/llm_providers.py
--rw-r--r--   0        0        0     3603 1970-01-01 00:00:00.000000 wordcel-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-25 01:08:30.881980 wordcel-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2783 2023-07-25 21:14:13.262827 wordcel-0.0.3/README.md
+-rw-r--r--   0        0        0      333 2023-07-29 04:10:21.768151 wordcel-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 00:46:00.681902 wordcel-0.0.3/wordcel/__init__.py
+-rw-r--r--   0        0        0     2348 2023-07-29 04:09:11.930935 wordcel-0.0.3/wordcel/featurize.py
+-rw-r--r--   0        0        0     1042 2023-07-25 00:48:13.299968 wordcel-0.0.3/wordcel/llm_providers.py
+-rw-r--r--   0        0        0     3603 1970-01-01 00:00:00.000000 wordcel-0.0.3/PKG-INFO
```

### Comparing `wordcel-0.0.2/LICENSE` & `wordcel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.2/README.md` & `wordcel-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.2/wordcel/featurize.py` & `wordcel-0.0.3/wordcel/featurize.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def apply_io_bound_function(
     df,
     user_function,
     text_column=None,
     id_column=None,
     num_threads=4,
-    cache_folder="cache",
+    cache_folder=None,
 ):
     """
     Apply an I/O bound user-provided function to a specific column in a Pandas DataFrame with threading and caching.
 
     Parameters:
         df (pd.DataFrame): Pandas DataFrame containing the data.
         user_function (function): User-provided function that takes text as input and returns a JSON.
@@ -25,33 +25,35 @@
         cache_folder (str): Folder to store the cached JSON outputs.
 
     Returns:
         pd.DataFrame: The original DataFrame with an additional 'result' column containing the JSON outputs.
     """
     assert text_column is not None, "The 'text_column' argument must be specified."
 
-    if not os.path.exists(cache_folder):
+    if cache_folder and not os.path.exists(cache_folder):
         os.makedirs(cache_folder)
 
     if id_column is None:
         id_column = df.index.name if df.index.name else "index"
 
     def process_text_with_caching(text, identifier):
-        # Check if result is already cached
-        identifier = identifier.replace("/", "_")
-        cache_file = os.path.join(cache_folder, f"{identifier}.json")
-        if os.path.exists(cache_file):
-            with open(cache_file, "r") as f:
-                return json.load(f)
+        if cache_folder:
+            # Check if result is already cached
+            identifier = str(identifier).replace("/", "_")
+            cache_file = os.path.join(cache_folder, f"{identifier}.json")
+            if os.path.exists(cache_file):
+                with open(cache_file, "r") as f:
+                    return json.load(f)
 
         result = user_function(text)
 
-        # Cache the result
-        with open(cache_file, "w") as f:
-            json.dump(result, f)
+        if cache_folder:
+            # Cache the result
+            with open(cache_file, "w") as f:
+                json.dump(result, f)
 
         return result
 
     def process_row(row):
         idx, row = row
         text = row[text_column]
         identifier = row[id_column]
```

### Comparing `wordcel-0.0.2/wordcel/llm_providers.py` & `wordcel-0.0.3/wordcel/llm_providers.py`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.2/PKG-INFO` & `wordcel-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordcel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create text-based features from large language models
 Author: Andrew Han
 Author-email: handrew11@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

