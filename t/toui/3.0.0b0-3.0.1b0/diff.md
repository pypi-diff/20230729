# Comparing `tmp/toui-3.0.0b0.tar.gz` & `tmp/toui-3.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.0.0b0.tar", last modified: Sat Jul 29 19:36:00 2023, max compression
+gzip compressed data, was "toui-3.0.1b0.tar", last modified: Sat Jul 29 19:49:22 2023, max compression
```

## Comparing `toui-3.0.0b0.tar` & `toui-3.0.1b0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.268970 toui-3.0.0b0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.0.0b0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.0.0b0/MANIFEST.in
--rw-rw-rw-   0        0        0     4265 2023-07-29 19:36:00.268970 toui-3.0.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.0.0b0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.173201 toui-3.0.0b0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.0.0b0/examples/advanced_example_2_toui_with_javascript.py
--rw-rw-rw-   0        0        0     1810 2023-07-29 13:30:14.000000 toui-3.0.0b0/examples/advanced_example_3_toui_with_google_sign_in.py
--rw-rw-rw-   0        0        0     3698 2023-07-29 16:55:17.000000 toui-3.0.0b0/examples/advanced_example_4_toui_with_firebase.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.178306 toui-3.0.0b0/images/
--rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.0.0b0/images/icon.png
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.0.0b0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-07-29 19:36:00.268970 toui-3.0.0b0/setup.cfg
--rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.0.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.257218 toui-3.0.0b0/toui/
--rw-rw-rw-   0        0        0      288 2023-07-29 12:54:43.000000 toui-3.0.0b0/toui/__init__.py
--rw-rw-rw-   0        0        0     2088 2023-07-29 18:05:12.000000 toui-3.0.0b0/toui/_cmd.py
--rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.0.0b0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.0.0b0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.0.0b0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.0.0b0/toui/_signals.py
--rw-rw-rw-   0        0        0    48705 2023-07-29 19:32:52.000000 toui-3.0.0b0/toui/apps.py
--rw-rw-rw-   0        0        0    23208 2023-07-29 16:31:59.000000 toui-3.0.0b0/toui/elements.py
--rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.0.0b0/toui/exceptions.py
--rw-rw-rw-   0        0        0    20631 2023-07-29 12:11:25.000000 toui-3.0.0b0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.0.0b0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.267795 toui-3.0.0b0/toui.egg-info/
--rw-rw-rw-   0        0        0     4265 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      925 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      217 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:22.280111 toui-3.0.1b0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.0.1b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.0.1b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4265 2023-07-29 19:49:22.280111 toui-3.0.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.0.1b0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:22.001824 toui-3.0.1b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.0.1b0/examples/advanced_example_2_toui_with_javascript.py
+-rw-rw-rw-   0        0        0     1810 2023-07-29 13:30:14.000000 toui-3.0.1b0/examples/advanced_example_3_toui_with_google_sign_in.py
+-rw-rw-rw-   0        0        0     3698 2023-07-29 16:55:17.000000 toui-3.0.1b0/examples/advanced_example_4_toui_with_firebase.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.0.1b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:22.008439 toui-3.0.1b0/images/
+-rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.0.1b0/images/icon.png
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.0.1b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-07-29 19:49:22.280111 toui-3.0.1b0/setup.cfg
+-rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.0.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:22.009382 toui-3.0.1b0/tests/
+-rw-rw-rw-   0        0        0      484 2023-05-15 13:04:45.000000 toui-3.0.1b0/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:22.270362 toui-3.0.1b0/toui/
+-rw-rw-rw-   0        0        0      288 2023-07-29 19:48:37.000000 toui-3.0.1b0/toui/__init__.py
+-rw-rw-rw-   0        0        0     2277 2023-07-29 19:47:21.000000 toui-3.0.1b0/toui/_cmd.py
+-rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.0.1b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.0.1b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.0.1b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.0.1b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    48705 2023-07-29 19:32:52.000000 toui-3.0.1b0/toui/apps.py
+-rw-rw-rw-   0        0        0    23208 2023-07-29 16:31:59.000000 toui-3.0.1b0/toui/elements.py
+-rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.0.1b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    20631 2023-07-29 12:11:25.000000 toui-3.0.1b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.0.1b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:49:22.280111 toui-3.0.1b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     4265 2023-07-29 19:49:21.000000 toui-3.0.1b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      948 2023-07-29 19:49:21.000000 toui-3.0.1b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 19:49:21.000000 toui-3.0.1b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-29 19:49:21.000000 toui-3.0.1b0/toui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      217 2023-07-29 19:49:21.000000 toui-3.0.1b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-29 19:49:21.000000 toui-3.0.1b0/toui.egg-info/top_level.txt
```

### Comparing `toui-3.0.0b0/LICENSE` & `toui-3.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/PKG-INFO` & `toui-3.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.0.0b0
+Version: 3.0.1b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.0.0b0/README.md` & `toui-3.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/advanced_example_1_toui_blueprint.py` & `toui-3.0.1b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/advanced_example_2_toui_with_javascript.py` & `toui-3.0.1b0/examples/advanced_example_2_toui_with_javascript.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/advanced_example_3_toui_with_google_sign_in.py` & `toui-3.0.1b0/examples/advanced_example_3_toui_with_google_sign_in.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/advanced_example_4_toui_with_firebase.py` & `toui-3.0.1b0/examples/advanced_example_4_toui_with_firebase.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/example_1_simple_website.py` & `toui-3.0.1b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/example_2_simple_desktop_app.py` & `toui-3.0.1b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/example_3_updating_page.py` & `toui-3.0.1b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/example_4_function_with_arg.py` & `toui-3.0.1b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/examples/example_5_user_variables.py` & `toui-3.0.1b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/images/icon.png` & `toui-3.0.1b0/images/icon.png`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/images/logo.png` & `toui-3.0.1b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/setup.py` & `toui-3.0.1b0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui/_cmd.py` & `toui-3.0.1b0/toui/_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,21 +25,24 @@
         Displays this help text.
 """
 def main():
     pkg_directory = os.path.dirname(os.path.dirname(os.path.abspath(sys.argv[0])))
     if "--help" in sys.argv or len(sys.argv) == 1:
         print(help_text)
 
-    if "--minimal-reqs" in sys.argv:
-        subprocess.check_call([sys.executable, '-m', 'pip', 'install', "-r", f"{pkg_directory}/requirements.txt"])
-
-    if "--all-reqs" in sys.argv:
-        subprocess.check_call([sys.executable, '-m', 'pip', 'install', "-r", f"{pkg_directory}/requirements.txt"])
-        subprocess.check_call([sys.executable, '-m', 'pip', 'install', "-r", f"{pkg_directory}/optional_requirements.txt"])
+    try:
+        if "--minimal-reqs" in sys.argv:
+            subprocess.check_call([sys.executable, '-m', 'pip', 'install', "-r", f"{pkg_directory}/requirements.txt"])
 
+        if "--all-reqs" in sys.argv:
+            subprocess.check_call([sys.executable, '-m', 'pip', 'install', "-r", f"{pkg_directory}/requirements.txt"])
+            subprocess.check_call([sys.executable, '-m', 'pip', 'install', "-r", f"{pkg_directory}/optional_requirements.txt"])
+    except subprocess.CalledProcessError as e:
+        print("An error occured while installing the requirements. Please try again.")
+        print(e.output)
     if "init" in sys.argv:
         if not "--full" in sys.argv:
             response = requests.get("https://github.com/mubarakalmehairbi/BasicToUIProject/archive/master.zip", stream=True)
             project_path = "MyBasicToUIProject"
             if os.path.exists(project_path):
                 i = 1
                 project_path = f"MyBasicToUIProject_{i}"
```

### Comparing `toui-3.0.0b0/toui/_helpers.py` & `toui-3.0.1b0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui/_javascript_templates.py` & `toui-3.0.1b0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui/_signals.py` & `toui-3.0.1b0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui/apps.py` & `toui-3.0.1b0/toui/apps.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui/elements.py` & `toui-3.0.1b0/toui/elements.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui/pages.py` & `toui-3.0.1b0/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui/structure.py` & `toui-3.0.1b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.0b0/toui.egg-info/PKG-INFO` & `toui-3.0.1b0/toui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.0.0b0
+Version: 3.0.1b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.0.0b0/toui.egg-info/SOURCES.txt` & `toui-3.0.1b0/toui.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 examples/example_3_updating_page.py
 examples/example_4_function_with_arg.py
 examples/example_5_user_variables.py
 examples/example_6_quick_website.py
 examples/example_7_quick_desktop_app.py
 images/icon.png
 images/logo.png
+tests/test_examples.py
 toui/__init__.py
 toui/_cmd.py
 toui/_defaults.py
 toui/_helpers.py
 toui/_javascript_templates.py
 toui/_signals.py
 toui/apps.py
```

