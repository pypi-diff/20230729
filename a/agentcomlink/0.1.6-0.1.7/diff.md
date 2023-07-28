# Comparing `tmp/agentcomlink-0.1.6.tar.gz` & `tmp/agentcomlink-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentcomlink-0.1.6.tar", last modified: Fri Jul 28 17:15:41 2023, max compression
+gzip compressed data, was "agentcomlink-0.1.7.tar", last modified: Fri Jul 28 23:34:49 2023, max compression
```

## Comparing `agentcomlink-0.1.6.tar` & `agentcomlink-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:15:41.979947 agentcomlink-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 17:15:41.979947 agentcomlink-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:15:41.979947 agentcomlink-0.1.6/agentcomlink/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/agentcomlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/agentcomlink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/agentcomlink/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/agentcomlink/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/agentcomlink/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:15:41.979947 agentcomlink-0.1.6/agentcomlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 17:15:41.000000 agentcomlink-0.1.6/agentcomlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 17:15:41.000000 agentcomlink-0.1.6/agentcomlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:15:41.000000 agentcomlink-0.1.6/agentcomlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 17:15:41.000000 agentcomlink-0.1.6/agentcomlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:15:41.000000 agentcomlink-0.1.6/agentcomlink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:15:41.979947 agentcomlink-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 17:15:26.000000 agentcomlink-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:49.502014 agentcomlink-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 23:34:49.502014 agentcomlink-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:49.502014 agentcomlink-0.1.7/agentcomlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/agentcomlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/agentcomlink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/agentcomlink/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/agentcomlink/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/agentcomlink/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:49.502014 agentcomlink-0.1.7/agentcomlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-28 23:34:49.000000 agentcomlink-0.1.7/agentcomlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 23:34:49.000000 agentcomlink-0.1.7/agentcomlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:34:49.000000 agentcomlink-0.1.7/agentcomlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 23:34:49.000000 agentcomlink-0.1.7/agentcomlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 23:34:49.000000 agentcomlink-0.1.7/agentcomlink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:34:49.502014 agentcomlink-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 23:34:39.000000 agentcomlink-0.1.7/setup.py
```

### Comparing `agentcomlink-0.1.6/LICENSE` & `agentcomlink-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.6/PKG-INFO` & `agentcomlink-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.6/README.md` & `agentcomlink-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.6/agentcomlink/__init__.py` & `agentcomlink-0.1.7/agentcomlink/__init__.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.6/agentcomlink/files.py` & `agentcomlink-0.1.7/agentcomlink/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
 def list_files_formatted(path="."):
     check_files()
     files = os.listdir(os.path.join(storage_path, path))
     files_formatted = []
     for file in files:
         if os.path.isdir(os.path.join(storage_path, path, file)):
-            files_formatted.append(file + "/")
+            files_formatted.append(os.path.join(storage_path, file + "/"))
         else:
-            files_formatted.append(file)
+            files_formatted.append(os.path.join(storage_path, file))
     return "User's Files:\n" + "\n".join(files_formatted)
 
 def get_file(path):
     check_files()
     with open(os.path.join(storage_path, path), "r") as f:  # 'r' for reading
         content = f.read()
     return content
```

### Comparing `agentcomlink-0.1.6/agentcomlink/page.py` & `agentcomlink-0.1.7/agentcomlink/page.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.6/agentcomlink/server.py` & `agentcomlink-0.1.7/agentcomlink/server.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.6/agentcomlink.egg-info/PKG-INFO` & `agentcomlink-0.1.7/agentcomlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.6/setup.py` & `agentcomlink-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentcomlink',
-    version='0.1.6',
+    version='0.1.7',
     description='Simple chat, debug and file management panel for agents',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentcomlink',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

