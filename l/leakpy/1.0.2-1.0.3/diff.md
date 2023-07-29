# Comparing `tmp/leakpy-1.0.2-py3-none-any.whl.zip` & `tmp/leakpy-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3327 bytes, number of entries: 5
--rwxr-xr-x  2.0 unx     4655 b- defN 23-Jul-29 17:38 leakpy-1.0.2.data/scripts/leakpy
--rw-r--r--  2.0 unx     1131 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      382 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/RECORD
-5 files, 6261 bytes uncompressed, 2613 bytes compressed:  58.3%
+Zip file size: 3330 bytes, number of entries: 5
+-rwxr-xr-x  2.0 unx     4690 b- defN 23-Jul-29 19:14 leakpy-1.0.3.data/scripts/leakpy
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jul-29 19:14 leakpy-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 19:14 leakpy-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-29 19:14 leakpy-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      382 b- defN 23-Jul-29 19:14 leakpy-1.0.3.dist-info/RECORD
+5 files, 6296 bytes uncompressed, 2616 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: leakpy-1.0.2.data/scripts/leakpy
+Filename: leakpy-1.0.3.data/scripts/leakpy
 Comment: 
 
-Filename: leakpy-1.0.2.dist-info/METADATA
+Filename: leakpy-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: leakpy-1.0.2.dist-info/WHEEL
+Filename: leakpy-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: leakpy-1.0.2.dist-info/top_level.txt
+Filename: leakpy-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: leakpy-1.0.2.dist-info/RECORD
+Filename: leakpy-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `leakpy-1.0.2.data/scripts/leakpy` & `leakpy-1.0.3.data/scripts/leakpy`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,20 @@
         plugin_elements = row.find_all('div', {'class': 'col-sm-3'})
         for plugin in plugin_elements:
             plugin_link = plugin.find('a')
             if plugin_link is not None:
                 plugin_name = plugin_link.text.strip()
                 plugins.append(plugin_name)
 
+    plugins = list(set(plugins))
+
     return plugins
 
 
+
 def write_output(result, file_name):
     """Writes the result to the output file."""
     with open(file_name, "w") as f:
         result = list(dict.fromkeys(result))
         for line in result:
             f.write(f"{line}\n")
     console.print(
```

## Comparing `leakpy-1.0.2.dist-info/METADATA` & `leakpy-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leakpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: LeakIX API Client 
 Home-page: https://github.com/Chocapikk/LeakPy
 Author: Valentin Lobstein
 Author-email: balgogan@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

