# Comparing `tmp/comandor-0.2.9.tar.gz` & `tmp/comandor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comandor-0.2.9.tar", last modified: Mon May 15 17:36:48 2023, max compression
+gzip compressed data, was "comandor-0.4.0.tar", last modified: Sat Jul 29 17:51:59 2023, max compression
```

## Comparing `comandor-0.2.9.tar` & `comandor-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 17:36:34.000000 comandor-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-15 17:36:48.582849 comandor-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-15 17:36:34.000000 comandor-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/comandor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-15 17:36:34.000000 comandor-0.2.9/comandor/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/comandor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 17:36:48.000000 comandor-0.2.9/comandor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:36:48.582849 comandor-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 17:36:34.000000 comandor-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:36:48.582849 comandor-0.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-15 17:36:34.000000 comandor-0.2.9/test/test_comandor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:59.963257 comandor-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 17:51:40.000000 comandor-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-29 17:51:59.963257 comandor-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-29 17:51:40.000000 comandor-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:59.959257 comandor-0.4.0/comandor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 17:51:40.000000 comandor-0.4.0/comandor/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:59.959257 comandor-0.4.0/comandor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-29 17:51:59.000000 comandor-0.4.0/comandor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-29 17:51:59.000000 comandor-0.4.0/comandor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:51:59.000000 comandor-0.4.0/comandor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 17:51:59.000000 comandor-0.4.0/comandor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 17:51:59.000000 comandor-0.4.0/comandor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 17:51:59.000000 comandor-0.4.0/comandor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:51:59.963257 comandor-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-29 17:51:40.000000 comandor-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:51:59.963257 comandor-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-29 17:51:40.000000 comandor-0.4.0/test/test_comandor.py
```

### Comparing `comandor-0.2.9/LICENSE` & `comandor-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comandor-0.2.9/PKG-INFO` & `comandor-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comandor
-Version: 0.2.9
+Version: 0.4.0
 Summary: A Very Simple Script for Run your command!
 Home-page: https://github.com/NoobforAl/comandor
 Author: NoobforAl
 Author-email: FarshadSarmali@pm.me
 License: MIT License
 Keywords: command line,script
 Classifier: Development Status :: 1 - Planning
@@ -26,15 +26,15 @@
 ## How Install
 
 > pip install comandor
 
 ### How Use
 
 - make file .comandor  
-- setup config like this
+- setup config like this (json file)
 
 ```json
 {
   "name": "Update Apps!",
   "debug": true, // run debug mode ( not necessary )
   "logfile": "./logs.log", // where save logs ( not necessary )
   "actions": [
@@ -47,20 +47,47 @@
       "timeout": 5000
     }
     // you can add more action
   ]
 }
 ```  
 
+OR yaml file:
+
+```yaml
+name: "test rund command"
+debug: true
+logfile: "./logs.log"
+actions:
+  - action_name: "test12"
+    path: "."
+    commands:
+      - "cd ."
+    timeout: 5000
+
+```
+
 - you can see .comandor.example for more example  
 - and run this command
 
 > comandor
 
 ### Command Line Help
 
-| Command |                                      Info                                              |
-| -----   | :--------------------------------------------------------------------------------------: |
-| -h      |                                      see help                                            |
-| -l < path log file >  | where save logFile, if don't use this, not save logs |
-| -c  < path config file > | setup yor config file instead of .comandor file |
-| -d   | run program debug mode |
+```txt
+❯ comandor -h
+usage: comandor [-h] [-l LOGFILE] [-c CONFIG] [-d] [-sk SKIP]
+
+options:
+  -h, --help            show this help message and exit
+  -l LOGFILE, --logfile LOGFILE
+                        where save logfile
+  -c CONFIG, --config CONFIG
+                        where you have config file
+  -d, --debug           run debug mod
+  -sk SKIP, --skip SKIP
+                        skip with text,check text and if found match skip
+```
+
+### How run tests?
+
+> python -m unittest  test/test_comandor.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `comandor-0.2.9/README.md` & `comandor-0.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## How Install
 
 > pip install comandor
 
 ### How Use
 
 - make file .comandor  
-- setup config like this
+- setup config like this (json file)
 
 ```json
 {
   "name": "Update Apps!",
   "debug": true, // run debug mode ( not necessary )
   "logfile": "./logs.log", // where save logs ( not necessary )
   "actions": [
@@ -28,20 +28,47 @@
       "timeout": 5000
     }
     // you can add more action
   ]
 }
 ```  
 
+OR yaml file:
+
+```yaml
+name: "test rund command"
+debug: true
+logfile: "./logs.log"
+actions:
+  - action_name: "test12"
+    path: "."
+    commands:
+      - "cd ."
+    timeout: 5000
+
+```
+
 - you can see .comandor.example for more example  
 - and run this command
 
 > comandor
 
 ### Command Line Help
 
-| Command |                                      Info                                              |
-| -----   | :--------------------------------------------------------------------------------------: |
-| -h      |                                      see help                                            |
-| -l < path log file >  | where save logFile, if don't use this, not save logs |
-| -c  < path config file > | setup yor config file instead of .comandor file |
-| -d   | run program debug mode |
+```txt
+❯ comandor -h
+usage: comandor [-h] [-l LOGFILE] [-c CONFIG] [-d] [-sk SKIP]
+
+options:
+  -h, --help            show this help message and exit
+  -l LOGFILE, --logfile LOGFILE
+                        where save logfile
+  -c CONFIG, --config CONFIG
+                        where you have config file
+  -d, --debug           run debug mod
+  -sk SKIP, --skip SKIP
+                        skip with text,check text and if found match skip
+```
+
+### How run tests?
+
+> python -m unittest  test/test_comandor.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `comandor-0.2.9/comandor/models.py` & `comandor-0.4.0/comandor/models.py`

 * *Files identical despite different names*

### Comparing `comandor-0.2.9/comandor.egg-info/PKG-INFO` & `comandor-0.4.0/comandor.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comandor
-Version: 0.2.9
+Version: 0.4.0
 Summary: A Very Simple Script for Run your command!
 Home-page: https://github.com/NoobforAl/comandor
 Author: NoobforAl
 Author-email: FarshadSarmali@pm.me
 License: MIT License
 Keywords: command line,script
 Classifier: Development Status :: 1 - Planning
@@ -26,15 +26,15 @@
 ## How Install
 
 > pip install comandor
 
 ### How Use
 
 - make file .comandor  
-- setup config like this
+- setup config like this (json file)
 
 ```json
 {
   "name": "Update Apps!",
   "debug": true, // run debug mode ( not necessary )
   "logfile": "./logs.log", // where save logs ( not necessary )
   "actions": [
@@ -47,20 +47,47 @@
       "timeout": 5000
     }
     // you can add more action
   ]
 }
 ```  
 
+OR yaml file:
+
+```yaml
+name: "test rund command"
+debug: true
+logfile: "./logs.log"
+actions:
+  - action_name: "test12"
+    path: "."
+    commands:
+      - "cd ."
+    timeout: 5000
+
+```
+
 - you can see .comandor.example for more example  
 - and run this command
 
 > comandor
 
 ### Command Line Help
 
-| Command |                                      Info                                              |
-| -----   | :--------------------------------------------------------------------------------------: |
-| -h      |                                      see help                                            |
-| -l < path log file >  | where save logFile, if don't use this, not save logs |
-| -c  < path config file > | setup yor config file instead of .comandor file |
-| -d   | run program debug mode |
+```txt
+❯ comandor -h
+usage: comandor [-h] [-l LOGFILE] [-c CONFIG] [-d] [-sk SKIP]
+
+options:
+  -h, --help            show this help message and exit
+  -l LOGFILE, --logfile LOGFILE
+                        where save logfile
+  -c CONFIG, --config CONFIG
+                        where you have config file
+  -d, --debug           run debug mod
+  -sk SKIP, --skip SKIP
+                        skip with text,check text and if found match skip
+```
+
+### How run tests?
+
+> python -m unittest  test/test_comandor.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `comandor-0.2.9/setup.py` & `comandor-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='comandor',
-    version='0.2.9',
+    version='0.4.0',
     description='A Very Simple Script for Run your command!',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='https://github.com/NoobforAl/comandor',
     author='NoobforAl',
     author_email='FarshadSarmali@pm.me',
     license='MIT License',
```

