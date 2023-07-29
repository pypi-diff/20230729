# Comparing `tmp/tambus-0.0.1.tar.gz` & `tmp/tambus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tambus-0.0.1.tar", last modified: Sat Jul 29 19:35:49 2023, max compression
+gzip compressed data, was "tambus-0.2.0.tar", last modified: Sat Jul 29 19:58:43 2023, max compression
```

## Comparing `tambus-0.0.1.tar` & `tambus-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 19:35:49.194960 tambus-0.0.1/
--rw-rw-rw-   0        0        0     1063 2023-07-29 19:13:07.000000 tambus-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1093 2023-07-29 19:35:49.193953 tambus-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      689 2023-07-29 19:10:30.000000 tambus-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 19:35:49.195962 tambus-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      620 2023-07-29 19:12:19.000000 tambus-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:35:49.153695 tambus-0.0.1/tambus/
--rw-rw-rw-   0        0        0       32 2023-07-29 19:14:03.000000 tambus-0.0.1/tambus/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-07-29 19:05:00.000000 tambus-0.0.1/tambus/engine.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:35:49.192728 tambus-0.0.1/tambus.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-07-29 19:35:48.000000 tambus-0.0.1/tambus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-29 19:35:49.000000 tambus-0.0.1/tambus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 19:35:48.000000 tambus-0.0.1/tambus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 19:35:48.000000 tambus-0.0.1/tambus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 19:58:43.145374 tambus-0.2.0/
+-rw-rw-rw-   0        0        0     1063 2023-07-29 19:13:07.000000 tambus-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1024 2023-07-29 19:58:43.141381 tambus-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-07-29 19:57:54.000000 tambus-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 19:58:43.146383 tambus-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      620 2023-07-29 19:58:30.000000 tambus-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:58:43.088303 tambus-0.2.0/tambus/
+-rw-rw-rw-   0        0        0       39 2023-07-29 19:53:54.000000 tambus-0.2.0/tambus/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-07-29 19:05:00.000000 tambus-0.2.0/tambus/engine.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:58:43.127389 tambus-0.2.0/tambus.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/top_level.txt
```

### Comparing `tambus-0.0.1/LICENSE` & `tambus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tambus-0.0.1/PKG-INFO` & `tambus-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: tambus
-Version: 0.0.1
+Version: 0.2.0
 Summary: Bambus Template Engine
 Home-page: https://github.com/somespi/tambus
 Author: Someone.
 Author-email: someonegithub@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<center>
+![logo](./assets/banner.svg)
 
-<img src="./assets/banner.svg" width="300">
 
 
-##### Bambus Template Engine 
-</center>
-
 
 
 ## Usage 
 
 ```py
 
 import tambus
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: tambus Version: 0.0.1 Summary: Bambus Template
+Metadata-Version: 2.1 Name: tambus Version: 0.2.0 Summary: Bambus Template
 Engine Home-page: https://github.com/somespi/tambus Author: Someone. Author-
 email: someonegithub@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
-              [./assets/banner.svg] ##### Bambus Template Engine
-## Usage ```py import tambus t = tambus.TambusEngine() # rendering HTML with
-open("/templates/index.html") as f: print(t.translate(f.read(),
-hello="world!")) ``` And if we assume that the content of `/templates/
-index.html` is: ```html
+![logo](./assets/banner.svg) ## Usage ```py import tambus t =
+tambus.TambusEngine() # rendering HTML with open("/templates/index.html") as f:
+print(t.translate(f.read(), hello="world!")) ``` And if we assume that the
+content of `/templates/index.html` is: ```html
 ****** Hello {hello} ******
 ``` The output would be: ```html
 ****** Hello world! ******
 ```
```

### Comparing `tambus-0.0.1/README.md` & `tambus-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-<center>
+![logo](./assets/banner.svg)
 
-<img src="./assets/banner.svg" width="300">
 
 
-##### Bambus Template Engine 
-</center>
-
 
 
 ## Usage 
 
 ```py
 
 import tambus
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-              [./assets/banner.svg] ##### Bambus Template Engine
-## Usage ```py import tambus t = tambus.TambusEngine() # rendering HTML with
-open("/templates/index.html") as f: print(t.translate(f.read(),
-hello="world!")) ``` And if we assume that the content of `/templates/
-index.html` is: ```html
+![logo](./assets/banner.svg) ## Usage ```py import tambus t =
+tambus.TambusEngine() # rendering HTML with open("/templates/index.html") as f:
+print(t.translate(f.read(), hello="world!")) ``` And if we assume that the
+content of `/templates/index.html` is: ```html
 ****** Hello {hello} ******
 ``` The output would be: ```html
 ****** Hello world! ******
 ```
```

### Comparing `tambus-0.0.1/setup.py` & `tambus-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tambus",
-    version="0.0.1",
+    version="0.2.0",
     author="Someone.",
     author_email="someonegithub@gmail.com",
     description="Bambus Template Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/somespi/tambus",
     packages=setuptools.find_packages(),
```

### Comparing `tambus-0.0.1/tambus/engine.py` & `tambus-0.2.0/tambus/engine.py`

 * *Files identical despite different names*

### Comparing `tambus-0.0.1/tambus.egg-info/PKG-INFO` & `tambus-0.2.0/tambus.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: tambus
-Version: 0.0.1
+Version: 0.2.0
 Summary: Bambus Template Engine
 Home-page: https://github.com/somespi/tambus
 Author: Someone.
 Author-email: someonegithub@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<center>
+![logo](./assets/banner.svg)
 
-<img src="./assets/banner.svg" width="300">
 
 
-##### Bambus Template Engine 
-</center>
-
 
 
 ## Usage 
 
 ```py
 
 import tambus
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: tambus Version: 0.0.1 Summary: Bambus Template
+Metadata-Version: 2.1 Name: tambus Version: 0.2.0 Summary: Bambus Template
 Engine Home-page: https://github.com/somespi/tambus Author: Someone. Author-
 email: someonegithub@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
-              [./assets/banner.svg] ##### Bambus Template Engine
-## Usage ```py import tambus t = tambus.TambusEngine() # rendering HTML with
-open("/templates/index.html") as f: print(t.translate(f.read(),
-hello="world!")) ``` And if we assume that the content of `/templates/
-index.html` is: ```html
+![logo](./assets/banner.svg) ## Usage ```py import tambus t =
+tambus.TambusEngine() # rendering HTML with open("/templates/index.html") as f:
+print(t.translate(f.read(), hello="world!")) ``` And if we assume that the
+content of `/templates/index.html` is: ```html
 ****** Hello {hello} ******
 ``` The output would be: ```html
 ****** Hello world! ******
 ```
```

