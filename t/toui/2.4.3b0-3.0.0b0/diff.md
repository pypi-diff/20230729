# Comparing `tmp/toui-2.4.3b0.tar.gz` & `tmp/toui-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.4.3b0.tar", last modified: Sat May 27 06:01:49 2023, max compression
+gzip compressed data, was "toui-3.0.0b0.tar", last modified: Sat Jul 29 19:36:00 2023, max compression
```

## Comparing `toui-2.4.3b0.tar` & `toui-3.0.0b0.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.444718 toui-2.4.3b0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.3b0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.3b0/MANIFEST.in
--rw-rw-rw-   0        0        0     3296 2023-05-27 06:01:49.444718 toui-2.4.3b0/PKG-INFO
--rw-rw-rw-   0        0        0     2921 2023-05-26 03:58:02.000000 toui-2.4.3b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.123546 toui-2.4.3b0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.3b0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.170696 toui-2.4.3b0/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.3b0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-27 06:01:49.452885 toui-2.4.3b0/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-23 17:57:05.000000 toui-2.4.3b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.437279 toui-2.4.3b0/toui/
--rw-rw-rw-   0        0        0      271 2023-05-27 05:58:40.000000 toui-2.4.3b0/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-23 15:00:55.000000 toui-2.4.3b0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-2.4.3b0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-2.4.3b0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-2.4.3b0/toui/_signals.py
--rw-rw-rw-   0        0        0    31569 2023-05-27 04:41:53.000000 toui-2.4.3b0/toui/apps.py
--rw-rw-rw-   0        0        0    22886 2023-05-24 15:46:55.000000 toui-2.4.3b0/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.3b0/toui/exceptions.py
--rw-rw-rw-   0        0        0    18047 2023-05-23 16:30:18.000000 toui-2.4.3b0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.3b0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-27 06:01:49.444718 toui-2.4.3b0/toui.egg-info/
--rw-rw-rw-   0        0        0     3296 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-27 06:01:48.000000 toui-2.4.3b0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.268970 toui-3.0.0b0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.0.0b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.0.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4265 2023-07-29 19:36:00.268970 toui-3.0.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.0.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.173201 toui-3.0.0b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.0.0b0/examples/advanced_example_2_toui_with_javascript.py
+-rw-rw-rw-   0        0        0     1810 2023-07-29 13:30:14.000000 toui-3.0.0b0/examples/advanced_example_3_toui_with_google_sign_in.py
+-rw-rw-rw-   0        0        0     3698 2023-07-29 16:55:17.000000 toui-3.0.0b0/examples/advanced_example_4_toui_with_firebase.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.0.0b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.178306 toui-3.0.0b0/images/
+-rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.0.0b0/images/icon.png
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.0.0b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-07-29 19:36:00.268970 toui-3.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.0.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.257218 toui-3.0.0b0/toui/
+-rw-rw-rw-   0        0        0      288 2023-07-29 12:54:43.000000 toui-3.0.0b0/toui/__init__.py
+-rw-rw-rw-   0        0        0     2088 2023-07-29 18:05:12.000000 toui-3.0.0b0/toui/_cmd.py
+-rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.0.0b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.0.0b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.0.0b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.0.0b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    48705 2023-07-29 19:32:52.000000 toui-3.0.0b0/toui/apps.py
+-rw-rw-rw-   0        0        0    23208 2023-07-29 16:31:59.000000 toui-3.0.0b0/toui/elements.py
+-rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.0.0b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    20631 2023-07-29 12:11:25.000000 toui-3.0.0b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.0.0b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-07-29 19:36:00.267795 toui-3.0.0b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     4265 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      925 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      217 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-29 19:36:00.000000 toui-3.0.0b0/toui.egg-info/top_level.txt
```

### Comparing `toui-2.4.3b0/LICENSE` & `toui-3.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/PKG-INFO` & `toui-3.0.0b0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-Metadata-Version: 2.1
-Name: toui
-Version: 2.4.3b0
-Summary: Creates user interfaces (websites and desktop apps) from HTML easily
-Author: Mubarak Almehairbi
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![ToUI Image](https://github.com/mubarakalmehairbi/ToUI/blob/main/images/logo.png?raw=True)
 
 ![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
 ![Latest version](https://img.shields.io/pypi/v/toui)
 ![Docs](https://img.shields.io/readthedocs/toui)
 
 # Overview
-ToUI is a Python package for creating user interfaces (websites and desktop apps)
-from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
+ToUI is a Python framework for creating user interfaces (web apps and desktop apps)
+from HTML code easily. It allows you to call your Python functions from HTML. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
-- Converts HTML files into a responsive app.
+- Converts HTML and CSS files into a fast-responsive app using Python alone.
 - Simple to understand for programmers who only know Python and HTML.
+- Edit HTML files dynamically.
 - The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to a desktop app and vice versa.
+- Contains features that will greatly support you while creating your apps, such as:
+    - **Sign-in feature**
+    - **User-specific database**
+    - **Uploading and downloading files**
+    - **Google sign in (experimental)**
+    - **Firebase (experimental)**
+    - **Password protection for your app**
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
+To install only the required dependencies, run these commands:
+```shell
+pip install --no-deps toui
+toui --minimal-reqs
+```
 
 # How to create a basic website
 Import the required classes:
 ```python
 from toui import Website, Page
 ```
 Create a `Website` object:
@@ -76,27 +78,37 @@
 main_page = Page(html_file="path/to/html", url="/")
 app.add_pages(main_page)
 
 if __name__ == "__main__":
     app.run()
 ```
 
+# Start with a template
+To start with a basic template for a ToUI project. Run the command:
+```
+toui init
+```
+Alternatively, use this [template](https://github.com/mubarakalmehairbi/BasicToUIProject).
+
 # Make the app responsive
 Check this [example](https://toui.readthedocs.io/en/latest/Examples.example_1_simple_website.html)
 and [other examples](https://toui.readthedocs.io/en/latest/Examples.html) to learn how
 to make the website / desktop app responsive.
 
 # Deploy the app
 You can deploy the web app the same way you deploy a `Flask` app ([How to deploy Flask app](https://flask.palletsprojects.com/deploying/)).
 The only difference is that you need to access the `Flask` object first:
 ```python
 app = Website(__name__)
 flask_app = app.flask_app
 ```
 Then you need to deploy the `flask_app` and not the `app`.
 
+# How to contribute
+ToUI welcomes contribution, small or big. For anyone who wants to contribute please check the [contribution page](https://toui.readthedocs.io/en/latest/CONTRIBUTING.html).
+
 # License and Copyrights
 Copyrights (c) 2023 Mubarak Almehairbi.
 This package is licensed under the MIT license.
 
 # Documentation
 You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io).
```

### Comparing `toui-2.4.3b0/examples/advanced_example_1_toui_blueprint.py` & `toui-3.0.0b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/examples/example_1_simple_website.py` & `toui-3.0.0b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/examples/example_2_simple_desktop_app.py` & `toui-3.0.0b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/examples/example_3_updating_page.py` & `toui-3.0.0b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/examples/example_4_function_with_arg.py` & `toui-3.0.0b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/examples/example_5_user_variables.py` & `toui-3.0.0b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/images/logo.png` & `toui-3.0.0b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/setup.py` & `toui-3.0.0b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,16 @@
 version = __version__
 author = "Mubarak Almehairbi"
 description = "Creates user interfaces (websites and desktop apps) from HTML easily"
 package_name = "toui"
 requirements = []
 optional_requirements = ['flask-login', 'flask-sqlalchemy', 'flask-basicauth']
 
-reqs_txt = \
-"""beautifulsoup4==4.12.2
-Flask==2.2.5
-Flask_BasicAuth==0.2.0
-Flask_Session==0.4.1
-Flask_Caching==2.0.2
-Flask_Login==0.6.2
-flask_sock==0.6.0
-flask_sqlalchemy==3.0.3
-pywebview==4.1
-tinycss==0.4"""
+reqs_txt = open("requirements.txt", "r").read()
+reqs_txt += "\n" + open("optional_requirements.txt", "r").read()
 
 for pkg in reqs_txt.splitlines():
     pkg_name = pkg.split("==")[0]
     if pkg_name.lower().replace("_","-") in optional_requirements and small:
         continue
     pkg_version = pkg.split("==")[1]
     pkg_major_version = pkg_version.split(".")[0]
@@ -46,14 +37,15 @@
     author=author,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={'images': ['images/*']},
+    entry_points={'console_scripts': ['toui=toui._cmd:main']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     py_modules=[package_name],
     install_requires=requirements
```

### Comparing `toui-2.4.3b0/toui/_helpers.py` & `toui-3.0.0b0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/toui/_javascript_templates.py` & `toui-3.0.0b0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/toui/_signals.py` & `toui-3.0.0b0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/toui/apps.py` & `toui-3.0.0b0/toui/apps.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 A module that creates web apps and desktop apps.
 """
 import __main__
 import threading
 import json
-import inspect
+import uuid
 import time
 import os
+import requests
 from copy import copy
 from abc import ABCMeta, abstractmethod
+from collections import UserDict
 from collections.abc import MutableMapping
 from functools import wraps
-from typing import Any
-from flask import Flask, session, request, send_file
+from typing import Any, Union
+from flask import Flask, session, request, send_file, make_response, redirect
 from flask_sock import Sock
-from flask_caching import Cache
-from flask_session import Session
 import webview
 from toui._helpers import warn, info, debug, error
 from toui.pages import Page
-from toui.exceptions import ToUIWrongPlaceException, ToUINotAddedError
+from toui.exceptions import ToUIWrongPlaceException, ToUINotAddedError, ToUIOverlapException
 from toui._defaults import validate_ws, validate_data
 
 _imported_optional_reqs = {'flask-login':False,
                           'flask-sqlalchemy':False,
-                          'flask-basicauth':False}
+                          'flask-basicauth':False,
+                          'firebase_admin': False}
 
 try:
     from flask_login import LoginManager, UserMixin, current_user, login_user, logout_user, AnonymousUserMixin
     _imported_optional_reqs['flask-login'] = True
 except ModuleNotFoundError: pass
 
 try:
@@ -37,14 +38,24 @@
 except ModuleNotFoundError: pass
 
 try:
     from flask_basicauth import BasicAuth
     _imported_optional_reqs['flask-basicauth'] = True
 except ModuleNotFoundError: pass
 
+try:
+    import firebase_admin
+    import firebase_admin.db
+    import firebase_admin.firestore
+    import firebase_admin.credentials
+    import firebase_admin.storage
+    import firebase_admin.auth
+    _imported_optional_reqs['firebase_admin'] = True
+except ModuleNotFoundError: pass
+
 
 class _ReqsChecker:
 
     def __init__(self, reqs) -> None:
         self.reqs = reqs
 
     def __call__(self, func) -> Any:
@@ -57,65 +68,60 @@
                     raise ModuleNotFoundError(f"You have not installed the optional package `{req}` yet, to install it run:\n\tpip install {req}")
         return new_func
 
 
 class _App(metaclass=ABCMeta):
     """The base class for DesktopApp and Website"""
 
-    def __init__(self, name=None, assets_folder=None, secret_key=None):
+    def __init__(self, name=None, assets_folder=None, secret_key=None, vars_timeout=86400, gen_sid_algo=None):
         """
 
         Parameters
         ----------
         name: str (optional)
             The name of the app.
 
         assets_folder: str (optional)
             The path to the folder that contains the HTML files and other assets.
 
         secret_key: str (optional)
             Sets the `secret_key` attribute for `flask.Flask`. You can also set the environment variable SECRET_KEY from
             the command line and ToUI will get it using `os.environ`.
 
+        vars_timeout: int (optional)
+            The timeout interval before the temporary user-specific variables are deleted from `user_vars` attribute.
+            The default is 86400 seconds (1 day).
+
+        gen_sid_algo: Callable (optional)
+            A callable that generates a unique user id so that ToUI can store data for each user/browser. If ``None``, the
+            IP address, user agent, and secret key will be used.
+
             
         Attributes
         ----------
         flask_app: Flask
             ToUI creates applications using `Flask`. You can access the `Flask` object using the attribute `flask_app`.
 
         forbidden_urls: list
             These are URLs that ToUI does not allow the user to use because ToUI uses them.
 
         user_vars: dict
-            A dictionary that stores temporary data unique to each user. The data are stored in a `Cache` object from `flask-caching`
-            package.
+            A dictionary that stores temporary data unique to each user.
 
         pages: list
             A list of added `Page` objects.
 
 
-        Warning
-        -------
-        A folder called 'flask_session' will be created in the main directory when calling this class.
-
-
         .. admonition:: Behind The Scenes
             :class: tip
             
             ToUI uses `Flask` and its extenstions to create apps. When creating an instance of this class, the following
             extensions are used:
 
-            - `Session` class extension from `Flask-Session` package.
             - `Sock` class extension from `Flask-Sock` package.
-            - `Cache` class extension from `Flask-Caching` package.
-
-            The following `Flask` configurations are also set:
-
-            - `CACHE_TYPE = "SimpleCache"`
-            - `SESSION_TYPE = "filesystem"`
 
         """
         self._functions = {}
         if not name:
             if hasattr(__main__, "__file__"):
                 name = os.path.basename(__main__.__file__).split(".")[0]
             else:
@@ -127,24 +133,27 @@
             self.flask_app.secret_key = secret_key
         elif os.environ.get('SECRET_KEY') is not None:
             self.flask_app.secret_key = os.environ.get('SECRET_KEY')
         else:
             warn("No secret key was set. Generating a random secret key for Flask.")
             self.flask_app.secret_key = os.urandom(50)
         self.pages = []
-        self.flask_app.config['SESSION_TYPE'] = "filesystem"
-        Session(self.flask_app)
         self._add_communication_method()
-        self._add_user_vars()
+        self._add_user_vars(timeout_interval=vars_timeout, gen_sid_algo=gen_sid_algo)
         self.flask_app.route("/toui-download-<path_id>", methods=['POST', 'GET'])(self._download)
-        self.forbidden_urls = ['/toui-communicate', "/toui-download-<path_id>"]
+        self.flask_app.route("/toui-google-sign-in", methods=['POST', 'GET'])(self._sign_in_using_google)
+        self.forbidden_urls = ['/toui-communicate', "/toui-download-<path_id>", "/toui-google-sign-in"]
         self._validate_ws = validate_ws
         self._validate_data = validate_data
         self._auth = None
         self._user_cls = None
+        self._user_db_type = None
+        self._firebase_app = None
+        self._firebase_db = None
+        self._google_data = {}
 
     @abstractmethod
     def run(self): pass
 
     def add_pages(self, *pages, do_copy=False, blueprint=None, endpoint=None):
         """
         Adds pages to the app.
@@ -246,33 +255,105 @@
         """
         path_id = 0
         while self._user_vars._get(f'toui-download-{path_id}'):
             path_id += 1
         self._user_vars._set(f'toui-download-{path_id}', filepath)
         self.open_new_page(f"/toui-download-{path_id}", new=new)
 
+    @_ReqsChecker(['firebase_admin'])
+    def add_firebase(self, firebase_config: Union[dict, str], **options):
+        """
+        Adds Firebase to the app.
+
+        Parameters
+        ----------
+        firebase_config: dict, str
+            The Firebase configuration dictionary or the path of credentials JSON.
+
+        options (optional)
+            Extra options for initializing Firebase. See `Google's documentation <https://firebase.google.com/docs/reference/admin/python/firebase_admin#initialize_app>`_.
+        """
+        certificate = firebase_admin.credentials.Certificate(firebase_config)
+        self._firebase_app = firebase_admin.initialize_app(certificate, options)
+
+    def store_file_using_firebase(self, destination_path, file_path, bucket_name=None):
+        """
+        Uploads a file to Firebase storage.
+
+        Parameters
+        ----------
+        destination_path: str
+            The path of the file in Firebase storage.
+
+        file_path: str
+            The path of the file on the server.
+
+        bucket_name: str, default = None
+            The name of the bucket. If ``None``, the default bucket will be used. However, if you did not specify "storageBucket"
+            option in the Firebase configuration, you must specify the bucket name in this function.
+
+        Returns
+        -------
+        None
+
+        """
+        bucket = firebase_admin.storage.bucket(name=bucket_name)
+        blob = bucket.blob(destination_path)
+        blob.upload_from_filename(file_path)
+
+    def get_file_from_firebase(self, source_path, new_file_path, bucket_name=None):
+        """
+        Downloads a file from Firebase storage.
+
+        Parameters
+        ----------
+        source_path: str
+            The path of the file in Firebase storage.
+
+        new_file_path: str
+            The path of the file on the server.
+
+        bucket_name: str, default = None
+            The name of the bucket. If ``None``, the default bucket will be used. However, if you did not specify "storageBucket"
+            option in the Firebase configuration, you must specify the bucket name in this function.
+
+        Returns
+        -------
+        None
+
+        """
+        bucket = firebase_admin.storage.bucket(name=bucket_name)
+        blob = bucket.blob(source_path)
+        blob.download_to_filename(new_file_path)
+
     @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
-    def add_user_database(self, database_uri, other_columns=[], user_cls=None):
+    def add_user_database_using_sql(self, database_uri, other_columns=[], user_cls=None):
         """
         Creates a simple database that has data specific to each user.
 
-        The database is a table that contains the following columns: `username`, `password`, and `id`. To add other columns,
-        add their names in `other_columns` list.
+        The database has a table that contains the following columns: `username`, `password`, and `id`. To add other columns,
+        add their names in `other_columns` list.  Note that this is different from `user_vars` which is a stores temporary
+        data without the need to sign in.
+
+        Warning
+        -------
+        A table called `users` will be created in the database. If you already have a table with the same name, it might be
+        overwritten.
 
         Parameters
         ----------
         database_uri: str
             The URI of the database that you want to connect to.
 
         other_columns: list
-            The names of table columns other than `username`, `password`, and `id`.
+            The names of table columns other than `username`, `password`, `email` and `id`.
 
         user_cls: Callable, default=None
-            If this parameter is ``None``, a table called `User` will be created. However, if this parameter was set, the
-            table `User` will not be created and the parameter `user_cls` will be used instead.
+            If this parameter is ``None``, a table called `users` will be created. However, if this parameter was set, the
+            table `users` will not be created and the parameter `user_cls` will be used instead.
 
 
         .. admonition:: Behind The Scenes
             :class: tip
             
             The following flask extensions are used when calling this function:
 
@@ -280,36 +361,65 @@
             - `LoginManager` class extension from `Flask-Login` package.
 
             The following `Flask` configurations are also set:
 
             - `SQLALCHEMY_DATABASE_URI = database_uri`
 
         """
+        if self._user_db_type == "firebase":
+            raise ToUIOverlapException("This function cannot be called when using Firebase user database.")
+        self._user_db_type = "sql"
         self.flask_app.config['SQLALCHEMY_DATABASE_URI'] = database_uri
         self._db = SQLAlchemy(self.flask_app)
         self._login_manager = LoginManager(self.flask_app)
         self._load_user = self._login_manager.user_loader(self._load_user)
         if not user_cls:
             class User(UserMixin, self._db.Model):
-                __tablename__ = "user"
+                __tablename__ = "users"
 
                 id = self._db.Column(self._db.Integer, primary_key=True)
                 username = self._db.Column(self._db.String, nullable=False, unique=True)
-                password = self._db.Column(self._db.String, nullable=False, unique=False)
+                email = self._db.Column(self._db.String, nullable=True, unique=True)
+                password = self._db.Column(self._db.String, nullable=True, unique=False)
 
                 def __repr__(self):
                     return f'<User {self.username}>'
             for col in other_columns:
                 setattr(User, col, self._db.Column(self._db.String))
         else:
             User = user_cls
         self._user_cls = User
         with self.flask_app.app_context():
             self._db.create_all()
 
+    @_ReqsChecker(['firebase_admin'])
+    def add_user_database_using_firebase(self):
+        """
+        Adds Firebase user database to the app.
+
+        Make sure you create a firestore database (not realtime) in your Firebase app.
+
+        Warning
+        -------
+        A collection called `users` will be created in the database. If you already have a collection with the same name, it might be overwritten.
+
+        
+        .. admonition:: Behind The Scenes
+            :class: tip
+            
+            Firebase authentication and database are used when calling this function.
+            
+        """
+        if self._firebase_app is None:
+            raise ToUINotAddedError("Firebase is not added to the app. Use `add_firebase` to add it.")
+        if self._user_db_type == "sql":
+            raise ToUIOverlapException("This function cannot be called when using SQL user database.")
+        self._user_db_type = "firebase"
+        self._firebase_db = firebase_admin.firestore.client().collection("users")
+
     # Website-specific methods
     @staticmethod
     def get_request():
         """
         A static method that gets data sent from client using HTTP request.
 
         This method returns the `request` object of `Flask`. The `request` object has some useful attributes such as
@@ -351,47 +461,56 @@
             https://flask.palletsprojects.com/en/2.2.x/api/#flask.request
 
         Page.on_url_request
 
         """
         return request
 
-    @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
-    def signup_user(self, username, password, **other_info):
+    def signup_user(self, username, password=None, email=None, **other_info):
         """
         Creates a new user in the database.
         
         Parameters
         ----------
         username: str
 
         password: str
 
+        email: str
+
         other_info
             Other information required for signing up.
 
         Returns
         -------
         bool
             ``True`` if the user is created, and ``False`` if it is not created.
 
         """
         self._confirm_user_database_created()
-        if self.username_exists(username):
+        if self.username_exists(username) or self.email_exists(email):
             return False
-        new_user = self._user_cls(username=username, password=password, **other_info)
-        self._db.session.add(new_user)
-        self._db.session.commit()
-        if self.username_exists(username):
+        if self._user_db_type == "sql":
+            new_user = self._user_cls(username=username, password=password, email=email, **other_info)
+            self._db.session.add(new_user)
+            self._db.session.commit()
+        elif self._user_db_type == "firebase":
+            if password is not None:
+                if len(password) < 6:
+                    error("Password for Firebase authentication needs to be at least 6 characters")
+                    return False
+            user_record = firebase_admin.auth.create_user(password=password, display_name=username, email=email)
+            self._firebase_db.document(user_record.uid).set({"username": username, 'password': password,
+                                                                         'email': email, **other_info})
+        if self.username_exists(username) or self.email_exists(email):
             return True
         else:
             return False
 
-    @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
-    def signin_user(self, username, password, **other_info):
+    def signin_user(self, username, password=None, email=None, **other_info):
         """
         Loads the data of a user from database.
 
         Parameters
         ----------
         username: str
 
@@ -403,23 +522,28 @@
         Returns
         -------
         bool
             ``True`` if the user is signed in, and ``False`` if it is not signed in.
 
         """
         self._confirm_user_database_created()
-        user = self._user_cls.query.filter_by(username=username, password=password, **other_info).first()
-        if user:
-            login_user(user)
-            self._user_vars._set("user-id", user.id)
-            return True
-        else:
+        if not self.username_exists(username) and not self.email_exists(email):
             return False
+        if self._user_db_type == "sql":
+            user = self._user_cls.query.filter_by(username=username, password=password, email=email, **other_info).first()
+            if user:
+                login_user(user)
+                self._user_vars._set("user-id", user.id)
+                return True
+            else:
+                return False
+        elif self._user_db_type == "firebase":
+            user_id = self._firebase_db.where("username", "==", username).get()[0].id
+            return self.signin_user_from_id(user_id)
         
-    @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
     def signin_user_from_id(self, user_id, **other_info):
         """
         Loads the data of a user from database using the user's ID.
 
         Parameters
         ----------
         id: int
@@ -430,61 +554,218 @@
         Returns
         -------
         bool
             ``True`` if the user is signed in, and ``False`` if it is not signed in.
 
         """
         self._confirm_user_database_created()
-        user = self._user_cls.query.filter_by(id=user_id, **other_info).first()
-        if user:
-            login_user(user)
-            self._user_vars._set("user-id", user_id)
-            return True
-        else:
+        if self._user_db_type == "sql":
+            user = self._user_cls.query.filter_by(id=user_id, **other_info).first()
+            if user:
+                login_user(user)
+                self._user_vars._set("user-id", user_id)
+                return True
+            else:
+                return False
+        elif self._user_db_type == "firebase":
+            user = firebase_admin.auth.get_user(user_id)
+            if user:
+                self._user_vars._set("user-id", user_id)
+                return True
+            else:
+                return False
+            
+    def get_current_user_data(self, key):
+        """
+        Gets data specific to the currently signed in user from the database.
+
+        Parameters
+        ----------
+        key: str
+            The key (name) of the data. For example: "username", "email", "age", etc.
+
+        Returns
+        -------
+        Any
+            The value of the data.
+        """
+        self._confirm_user_database_created()
+        if not self.is_signed_in():
+            error("No user is signed in.")
+            return None
+        if self._user_db_type == "sql":
+            return getattr(current_user, key)
+        elif self._user_db_type == "firebase":
+            return self._firebase_db.document(self._user_vars._get("user-id")).get().to_dict().get(key)
+
+    def set_current_user_data(self, key, value):
+        """
+        Sets data specific to the currently signed in user in the database.
+
+        Parameters
+        ----------
+        key: str
+            The key (name) of the data. For example: "username", "email", "age", etc.
+
+        value: Any
+            The value of the data.
+
+        Returns
+        -------
+        bool
+            ``True`` if the data is set, and ``False`` if it is not set.
+
+        """
+        self._confirm_user_database_created()
+        if not self.is_signed_in():
+            error("No user is signed in.")
             return False
+        if self._user_db_type == "sql":
+            setattr(current_user, key, value)
+            self._db.session.commit()
+            return True
+        elif self._user_db_type == "firebase":
+            self._firebase_db.document(self._user_vars._get("user-id")).update({key: value})
+            return True
+        
+    def get_current_user_id(self):
+        """
+        Gets the ID of the currently signed in user.
+
+        Returns
+        -------
+        str
+            The ID of the user.
+        """
+        self._confirm_user_database_created()
+        if not self.is_signed_in():
+            error("No user is signed in.")
+            return None
+        return self._user_vars._get("user-id")
 
-    @_ReqsChecker(['flask-login'])
     def signout_user(self):
         """
         A method that signs out the current user.
         """
-        logout_user()
+        self._confirm_user_database_created()
+        if self._user_db_type == "sql":
+            logout_user()
         self._user_vars._del('user-id')
 
-    @_ReqsChecker(['flask-sqlalchemy'])
     def username_exists(self, username):
         """
         Checks if the username is exists in the database.
         
         Parameters
         ----------
         username: str
         
         Returns
         -------
         bool
             ``True`` if the username exists, otherwise ``False``.
             """
         self._confirm_user_database_created()
-        if self._user_cls.query.filter_by(username=username).first():
-            info(f"User {username} exists")
-            return True
-        else:
+        if self._user_db_type == "sql":
+            if self._user_cls.query.filter_by(username=username).first():
+                info(f"User {username} exists")
+                return True
+            else:
+                return False
+        elif self._user_db_type == "firebase":
+            if len(self._firebase_db.where("username", "==", username).get()) > 0:
+                info(f"User {username} exists")
+                return True
+            else:
+                return False
+            
+    def email_exists(self, email):
+        """
+        Checks if the email is exists in the database.
+        
+        Parameters
+        ----------
+        email: str
+        
+        Returns
+        -------
+        bool
+            ``True`` if the email exists, otherwise ``False``.
+        """
+        self._confirm_user_database_created()
+        if email is None:
             return False
+        if self._user_db_type == "sql":
+            if self._user_cls.query.filter_by(email=email).first():
+                info(f"Email {email} exists")
+                return True
+            else:
+                return False
+        elif self._user_db_type == "firebase":
+            if len(self._firebase_db.where("email", "==", email).get()) > 0:
+                return True
+            else:
+                return False
 
-    @staticmethod
-    @_ReqsChecker(['flask-login'])
-    def get_current_user():
+    def is_signed_in(self):
         """
-        A static method that returns the current user.
+        Checks if the user is signed in.
+
+        Returns
+        -------
+        bool
         """
-        if isinstance(current_user, AnonymousUserMixin):
-            return None
+        self._confirm_user_database_created()
+        if self.user_vars._get('user-id'):
+            if self._user_db_type == "sql":
+                login_user(self._user_cls.query.filter_by(id=self._user_vars._get("user-id")).first())
+            return True
         else:
-            return current_user
+            return False
+        
+    def sign_in_using_google(self, client_id, client_secret, after_auth_url, additional_scopes=None, custom_username=None, **other_params):
+        """
+        Signs in a user using Google (Experimental).
+
+        Make sure to create a Google app first. Also, add the following as an authorized redirect URI to your Google app:
+        ``https://<your-domain>/toui-google-sign-in``
+        
+        Parameters
+        ----------
+        client_id: str
+            The client ID of the Google app.
+
+        client_secret: str
+            The client secret of the Google app.
+
+        after_auth_url: str
+            The URL to redirect to after completing authentication. This is not the same as the redirect uri of the Google app, so
+            you do not need to register it as an authorized redirect URI in your Google app.
+
+        additional_scopes: list, default=None (optional)
+            By default, the user allows the app to only access non-sensitive information such as the user's name and email. If you
+            want to access more information, you can pass a list of scopes. For more information, see `Google's documentation <https://developers.google.com/identity/protocols/oauth2/scopes>`_.
+
+        custom_username: str, default=None (optional)
+            If you want to use a custom username instead of the user's email, you can pass it here.
+
+        other_params: kwargs (optional)
+            Keyword arguments that can be passed as parameters to authorization url.For more information, see
+            `Google's documentation <https://developers.google.com/identity/protocols/oauth2/web-server#httprest_1>`_.
+        """
+
+        self._google_data = {"client_id": client_id, "client_secret": client_secret}
+        scope = "https://www.googleapis.com/auth/userinfo.email https://www.googleapis.com/auth/userinfo.profile"
+        if additional_scopes:
+            for s in additional_scopes:
+                scope += f" {s}"
+        url = f"/toui-google-sign-in?after_auth_url={after_auth_url}&scope={scope}"
+        for key, value in other_params.items():
+            url += f"&{key}={value}"
+        self.open_new_page(url=url)
 
     @_ReqsChecker(['flask-basicauth'])
     def add_restriction(self, username, password):
         """
         Makes the app private.
 
         Adds a username and password to the app.
@@ -585,18 +866,16 @@
         self.flask_app.register_blueprint(blueprint=blueprint, **options)
 
     def _add_communication_method(self):
         self.flask_app.config['SOCK_SERVER_OPTIONS'] = {'ping_interval': 25}
         self._socket = Sock(self.flask_app)
         self._socket.route("/toui-communicate")(self._communicate)
 
-    def _add_user_vars(self):
-        self.flask_app.config["CACHE_TYPE"] = "SimpleCache"
-        self._cache = Cache(self.flask_app)
-        self._user_vars = _UserVars(self._cache)
+    def _add_user_vars(self, timeout_interval, gen_sid_algo):
+        self._user_vars = _UserVars(self, timeout_interval=timeout_interval, gen_sid_algo=gen_sid_algo)
 
     def _session_check(self):
         """This is a private function."""
         try:
             session.keys()
         except RuntimeError as e:
             return False
@@ -605,17 +884,15 @@
         if not "_user_id" in session.keys():
             user_id = self._user_vars._get('user-id')
             if user_id:
                 session['_user_id'] = user_id
         return True
     
     def _download(self, path_id):
-        debug(f"PATH: {path_id}")
         file_to_download = self._user_vars._get(f'toui-download-{path_id}')
-        debug(f"File to download: {file_to_download}")
         if file_to_download:
             return send_file(file_to_download, as_attachment=True)
 
     def _communicate(self, ws):
         """This is a private function."""
         validation = self._validate_ws(ws)
         if not validation:
@@ -635,19 +912,17 @@
                     continue
                 s = time.time()
                 data_dict = json.loads(data_from_js)
                 if data_dict.get("type") == "page":
                     ws.pending_pages.append(data_dict)
                     valid_message = True
             while True:
-                debug(f"Pages Before: {len(ws.pending_pages)}")
                 if len(ws.pending_pages) == 0:
                     break
                 data_dict = ws.pending_pages.pop(0)
-                debug(f"Pages After: {len(ws.pending_pages)}")
                 self._session_check()
                 func = data_dict['func']
                 args = data_dict['args']
                 url = data_dict['url']
                 new_html = data_dict['html']
                 new_page = Page(url=url)
                 new_page.from_str(new_html)
@@ -671,92 +946,202 @@
                 except Exception as e:
                     del session['user page']
                     raise e
                 e = time.time()
                 debug(f"TIME: {e - s}s")
 
     def _confirm_user_database_created(self):
-        if self._user_cls is None:
-            raise ToUINotAddedError("You have not created the user database yet. To create it, call the method: `add_user_database`.")
+        if self._user_db_type is None:
+            raise ToUINotAddedError("You have not created the user database yet. To create it, call the method: `add_user_database_using_sql` or `add_user_database_using_firebase`.")
 
     def _load_user(self, user_id):
         return self._user_cls.query.filter_by(id=int(user_id)).first()
+    
+    def _get_user_details_from_google_token(self, access_token, refresh_token=None):
+        headers = {"Authorization": f"Bearer {access_token}"}
+        r = requests.get("https://www.googleapis.com/oauth2/v1/userinfo", headers=headers)
+        if r.status_code == 200:
+            return r.json()
+        elif r.status_code == 401:
+            if refresh_token:
+                r = requests.post("https://oauth2.googleapis.com/token", data={
+                    "client_id": self._google_data['client_id'],
+                    "client_secret": self._google_data['client_secret'],
+                    "refresh_token": refresh_token,
+                    "grant_type": "refresh_token"
+                },
+                headers={"Content-Type": "application/x-www-form-urlencoded"})
+                if r.status_code == 200:
+                    return self._get_user_details_from_google_token(r.json()['access_token'])
+        raise Exception(f"Error getting user details from Google. Status code: {r.status_code}. Response: {r.text}")
+    
+    def _sign_in_using_google(self):
+        client_id = self._google_data['client_id']
+        client_secret = self._google_data['client_secret']
+        scope = request.args.get("scope")
+        redirect_uri = request.base_url
+        response_type = "code"
+        access_type = request.args.get("access_type")
+        state = request.args.get("state")
+        include_granted_scopes = request.args.get("include_granted_scopes")
+        enable_granular_consent = request.args.get("enable_granular_consent")
+        login_hint = request.args.get("login_hint")
+        prompt = request.args.get("prompt")
+        after_auth_url = request.args.get("after_auth_url")
+        if after_auth_url:
+            self.user_vars._set('google-after-auth-url', after_auth_url)
+        else:
+            after_auth_url = self.user_vars._get('google-after-auth-url')
+        username = request.args.get("username")
+        if "code" in request.args:
+            code = request.args.get("code")
+            dictToSend = {'code':code,
+                          'client_id':client_id,
+                          'client_secret':client_secret,
+                          'grant_type':'authorization_code',
+                          'redirect_uri':redirect_uri}
+            res = requests.post('https://oauth2.googleapis.com/token', data=dictToSend,
+                                headers={'Host': 'oauth2.googleapis.com',
+                                         'Content-Type':'application/x-www-form-urlencoded'})
+            dictFromServer = res.json()
+            self.user_vars._set('google-access-token', dictFromServer['access_token'])
+            if 'refresh_token' in dictFromServer:
+                self.user_vars._set('google-refresh-token', dictFromServer['refresh_token'])
+            user_details = self._get_user_details_from_google_token(access_token=dictFromServer['access_token'], refresh_token=self.user_vars._get('google-refresh-token'))
+            self.user_vars._set('google-user-details', user_details)
+            email = user_details['email']
+            if username is None:
+                username = email
+            if self.email_exists(email):
+                self.signin_user(email=email, username=username, password=None)
+            else:
+                self.signup_user(email=email, username=username, password=None)
+            return redirect(after_auth_url)
+        else:
+            redirect_to = f"https://accounts.google.com/o/oauth2/v2/auth?" \
+                      f"client_id={client_id}" \
+                      f"&response_type={response_type}" \
+                      f"&scope={scope}" \
+                      f"&redirect_uri={redirect_uri}"
+            
+            if access_type is not None:
+                redirect_to += f"&access_type={access_type}"
+            if state is not None:
+                redirect_to += f"&state={state}"
+            if include_granted_scopes is not None:
+                if include_granted_scopes is True:
+                    redirect_to += f"&include_granted_scopes=true"
+                elif include_granted_scopes is False:
+                    redirect_to += f"&include_granted_scopes=false"
+            if enable_granular_consent is not None:
+                if enable_granular_consent is True:
+                    redirect_to += f"&enable_granular_consent=true"
+                elif enable_granular_consent is False:
+                    redirect_to += f"&enable_granular_consent=false"
+            if login_hint is not None:
+                redirect_to += f"&login_hint={login_hint}"
+            if prompt is not None:
+                redirect_to += f"&prompt={' '.join(prompt)}"
+            return redirect(redirect_to)
 
 
 class _FuncWithPage:
     """Currently this class is unused, but it might be used later."""
     def __init__(self, func, page):
         self.func = func
         self.page = page
     def __call__(self, *args, **kwargs):
         return self.func(*args, **kwargs)
 
 
 class _UserVars(MutableMapping):
     """User-specific variables"""
 
-    def __init__(self, cache) -> None:
-        self._cache = cache
+    def __init__(self, app, timeout_interval, gen_sid_algo) -> None:
+        self._app = app
+        self._cache = UserDict()
+        self._cache.set = self._cache.__setitem__
         self._default_vars = {}
+        self._timeout_interval = timeout_interval
+        if gen_sid_algo:
+            self._gen_sid = gen_sid_algo
 
-    def _sid_check(self):
+    def _gen_sid(self):
         try:
-            session.keys()
-            session_exists = True
-        except:
-            session_exists = False
-        if session_exists:
-            user_dict = self._cache.get(session.sid)
+            if request.cookies.get('TOUI_SID'):
+                sid = request.cookies.get('TOUI_SID')
+                session['toui-sid'] = sid
+            else:
+                if "toui-sid" in session:
+                    sid = session['toui-sid']
+                else:
+                    sid = str(uuid.uuid4())
+                    session['toui-sid'] = sid
+                response = make_response()
+                response.set_cookie("TOUI_SID", sid, secure=True, httponly=True)
+                session['toui-response'] = response
+            return sid
+        except RuntimeError:
+            return None
+        
+    def _timeout(self, sid):
+        self._cache.delete(sid)
+
+    def _sid_check(self):
+        sid = self._gen_sid()
+        if sid:
+            user_dict = self._cache.get(sid)
             if user_dict is None:
-                self._cache.set(session.sid, {"toui-vars": self._default_vars})
-            return session.sid
+                self._cache.set(sid, {"toui-vars": self._default_vars.copy()})
+                threading.Timer(self._timeout_interval, self._timeout, args=[sid]).start()
+            return sid
 
     def _get_toui_vars(self):
         sid = self._sid_check()
         if sid:
             return self._cache.get(sid)['toui-vars']
         else:
             return self._default_vars
-    
-    def _set_toui_vars(self, toui_vars):
+
+    def _get(self, key):
         sid = self._sid_check()
         if sid:
-            self._cache.set(session.sid, {'toui-vars': toui_vars})
+            return self._cache.get(sid).get(key)
         else:
-            self._default_vars = toui_vars
-
-    def _get(self, key):
-        self._sid_check()
-        return self._cache.get(session.sid).get(key)
+            return self._default_vars
     
     def _set(self, key, value):
         """Avoid key='toui-vars'"""
-        self._sid_check()
-        sid_dict = self._cache.get(session.sid)
-        sid_dict[key] = value
-        self._cache.set(session.sid, sid_dict)
+        sid = self._sid_check()
+        if sid:
+            sid_dict = self._cache.get(sid)
+            sid_dict[key] = value
+        else:
+            self._default_vars[key] = value
 
     def _del(self, key):
-        self._sid_check()
-        sid_dict = self._cache.get(session.sid)
-        del sid_dict[key]
-        self._cache.set(session.sid, sid_dict)
+        sid = self._sid_check()
+        if sid:
+            sid_dict = self._cache.get(sid)
+            if key in sid_dict:
+                del sid_dict[key]
+        else:
+            if key in self._default_vars:
+                del self._default_vars[key]
 
     def __getitem__(self, key):
         return self._get_toui_vars()[key]
     
     def __setitem__(self, key, value):
         toui_vars = self._get_toui_vars()
         toui_vars[key] = value
-        self._set_toui_vars(toui_vars)
 
     def __delitem__(self, key: Any) -> None:
         toui_vars = self._get_toui_vars()
         del toui_vars[key]
-        self._set_toui_vars(toui_vars)
 
     def __iter__(self):
         for key in self._get_toui_vars():
             yield key
 
     def __len__(self) -> int:
         return len(self._get_toui_vars())
```

### Comparing `toui-2.4.3b0/toui/elements.py` & `toui-3.0.0b0/toui/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 A module that creates HTML elements.
 """
 from bs4 import BeautifulSoup
 from bs4.element import Tag
 from copy import copy
+from typing import List
 import tinycss
-from toui._signals import Signal
+from toui._signals import Signal, File
 from toui._helpers import warn, debug, selector_to_str, obj_converter
 
 
 class _ElementSignal(Signal):
     """
     Creates signals that will be sent to JavaScript.
 
@@ -131,18 +132,18 @@
         ----------
         html_str: str
 
         """
         soup = BeautifulSoup(html_str, features="html.parser")
         tags = soup.find_all()
         if len(tags) > 0:
-            tag = tags[0]
-            self._element = tag
+            new = tags[0]
         else:
-            warn("No element found in string")
+            new = html_str
+        self._element.replace_with(new)
 
     def to_str(self):
         """
         Converts the `Element` object to HTML code.
 
         Returns
         -------
@@ -471,24 +472,29 @@
         value
             The new value of the ``value`` attribute.
 
         """
         self.set_attr("value", value)
 
     @_ElementSignal(return_type="js")
-    def get_files(self, with_content=False):
+    def get_files(self, with_content=False) -> List[File]:
         """
         Gets uploaded files from element.
 
         This method is useful when uploading files using ``<input type="file">`` element.
 
+        Note
+        ----
+        Remember to validate the names, types, and sizes of the uploaded files before using them.
+
         Parameters
         ----------
         with_content: bool, default=False
-            If ``True``, the contents of the files will be included in the output.
+            If ``True``, the contents of the files will be included in the output. It is recommended to keep this parameter
+            as ``False`` and use :py:meth:`File.save() <toui._signals.File.save>` instead after validating the files.
 
         Returns
         -------
         list(File)
             A list of `File` objects.
 
         See Also
```

### Comparing `toui-2.4.3b0/toui/pages.py` & `toui-3.0.0b0/toui/pages.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 A module that creates web pages or windows.
 """
 import os
 import time
 from bs4 import BeautifulSoup
 import webview
 import json
-from flask import session
+from flask import session, redirect, request, Response
 from toui.elements import Element
 from toui._javascript_templates import custom_func, get_script
 from copy import copy
 from toui._helpers import warn, info, debug, selector_to_str, obj_converter
 from toui._signals import Signal
-from toui._defaults import view_func
 
 
 class _PageSignal(Signal):
     """
     Creates signals that will be sent to JavaScript.
 
     These signals are related the methods of the `Page` object.
@@ -149,36 +148,42 @@
         self.window_defaults = {}
 
         # Other internal attributes
         self._app = None
         self._signal_mode = False
         self._signals = []
         self._functions = {}
-        self._basic_view_func = lambda: view_func(self)
-        self._view_func = self._basic_view_func
+        self._view_func = self._on_url_request
         self._uid = None
+        self._navigation_bar = ""
 
     def __str__(self):
         return self.to_str()
 
     def __repr__(self):
         return self.to_str()
 
     def __copy__(self):
         new_pg = Page(html_file=self._html_file, url=self.url)
         new_pg.from_bs4_soup(self.to_bs4_soup())
         new_pg._signal_mode = self._signal_mode
+        new_pg._navigation_bar = self._navigation_bar
         new_pg._app = self._app
         return new_pg
     
     @_PageSignal()
     def from_str(self, html_str):
         """
         Converts HTML code to a `Page` object.
 
+        Warning
+        -------
+        If this method is called after the app starts running, it will call the JavaScript function `document.write()`. This
+        might lead to potential security issues so use it with care.
+
         Parameters
         ----------
         html_str: str
             HTML code.
 
         """
         self._html = BeautifulSoup(html_str, features="html.parser")
@@ -194,14 +199,19 @@
         """
         return str(self._html)
 
     def from_html_file(self, html_path):
         """
         Reads an HTML file and converts it to an `Page` object.
 
+        Warning
+        -------
+        If this method is called after the app starts running, it will call the JavaScript function `document.write()`. This
+        might lead to potential security issues so use it with care.
+
         Parameters
         ----------
         html_path: str
 
         """
         with open(html_path, "rt") as file:
             self.from_str(file.read())
@@ -220,14 +230,19 @@
 
     @_PageSignal()
     def from_bs4_soup(self, bs4_soup):
         """
         Converts a `bs4.BeautifulSoap` object to a `Page` object.
         The `bs4.BeautifulSoap` object will be copied before converting.
 
+        Warning
+        -------
+        If this method is called after the app starts running, it will call the JavaScript function `document.write()`. This
+        might lead to potential security issues so use it with care.
+
         Parameters
         ----------
         bs4_soup: bs4.BeautifulSoap
 
         See Also
         --------
         bs4
@@ -464,40 +479,76 @@
             The function that will be called when a request is sent to the URL.
 
         display_return_value: bool, default=False
             If ``True``, the browser will display the return value of the function when the URL is loaded. If ``False``,
             the return value will be ignored.
 
         """
-        def new_func():
-            original_return = self._basic_view_func()
-            session['user page'] = copy(self)
-            try:
-                user_id = self._app._user_vars._get("user-id")
-                if user_id:
-                    session['_user_id'] = user_id
-                new_return = func()
-                if display_return_value:
-                    del session['user page']
-                    return new_return
-                else:
-                    pg = session['user page']
-                    del session['user page']
-                    return pg.to_str()
-            except Exception as e:
-                if 'user page' in session:
-                    del session['user page']
-                raise e
-
+        new_func = lambda: self._on_url_request(func=func, display_return_value=display_return_value)
         self._view_func = new_func
 
+    def set_navigation_bar(self, html_str):
+        """
+        Adds a navigation bar to the page.
+
+        Parameters
+        ----------
+        html_str: str
+            HTML code of the navigation bar.
+
+        Returns
+        -------
+        None
+
+        """
+        self._navigation_bar = html_str
+
     def get_window(self):
         for window in webview.windows:
             if window.uid == self._uid:
                 return window
+            
+    def _on_url_request(self, func=None, display_return_value=False):
+        self._app._user_vars._gen_sid()
+        session['user page'] = copy(self)
+        try:
+            if func:
+                new_return = func()
+                if display_return_value:
+                    del session['user page']
+                    if "toui-response" in session:
+                        response = session['toui-response']
+                        if isinstance(new_return, Response):
+                            response.set_data(new_return.get_data())
+                        else:
+                            response.set_data(new_return)
+                        del session['toui-response']
+                        return response
+                    else:   
+                        return new_return
+            pg = session['user page']
+            body_element = pg.get_body_element()
+            if body_element:
+                body_element.set_content(pg._navigation_bar + body_element.to_str()) 
+            else:
+                pg.from_str(pg._navigation_bar + pg.to_str())
+            del session['user page']
+            if "toui-response" in session:
+                response = session['toui-response']
+                response.set_data(pg.to_str())
+                del session['toui-response']
+                return response
+            else:
+                return pg.to_str()
+        except Exception as e:
+            if 'user page' in session:
+                del session['user page']
+            if 'toui-response' in session:
+                del session['toui-response']
+            raise e
 
     def _add_script(self):
         script_tag = Element("script")
         script_content = get_script(self._app.__class__.__name__)
         script_tag.set_content(script_content)
         self.get_elements(tag_name="html")[0].add_content(script_tag)
 
@@ -566,12 +617,33 @@
             return False
 
     def _call_func(self, func_name, *args, page=None):
         """Calls a function in this class. Its return value depends on the function called. This is a private function."""
         functions = self._get_functions()
         info(f'"{func_name}" called')
         return functions[func_name](*args)
+    
+
+class RedirectingPage(Page):
+    """
+    An empty page that redirects to another page when it is loaded.
+
+    Parameters
+    ----------
+    redirect_to: str
+        The URL of the page to redirect to.
+
+    url: str
+        The URL of the empty page.
+
+    title: str, default=None
+        The title of the empty page.
+
+    """
+    def __init__(self, redirect_to, url, title=None):
+        super().__init__(url=url, title=title)
+        self.on_url_request(lambda: redirect(redirect_to), display_return_value=True)
 
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `toui-2.4.3b0/toui/structure.py` & `toui-3.0.0b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.3b0/toui.egg-info/PKG-INFO` & `toui-3.0.0b0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.4.3b0
+Version: 3.0.0b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,28 +13,41 @@
 
 ![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
 ![Latest version](https://img.shields.io/pypi/v/toui)
 ![Docs](https://img.shields.io/readthedocs/toui)
 
 # Overview
-ToUI is a Python package for creating user interfaces (websites and desktop apps)
-from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
+ToUI is a Python framework for creating user interfaces (web apps and desktop apps)
+from HTML code easily. It allows you to call your Python functions from HTML. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
-- Converts HTML files into a responsive app.
+- Converts HTML and CSS files into a fast-responsive app using Python alone.
 - Simple to understand for programmers who only know Python and HTML.
+- Edit HTML files dynamically.
 - The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to a desktop app and vice versa.
+- Contains features that will greatly support you while creating your apps, such as:
+    - **Sign-in feature**
+    - **User-specific database**
+    - **Uploading and downloading files**
+    - **Google sign in (experimental)**
+    - **Firebase (experimental)**
+    - **Password protection for your app**
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
+To install only the required dependencies, run these commands:
+```shell
+pip install --no-deps toui
+toui --minimal-reqs
+```
 
 # How to create a basic website
 Import the required classes:
 ```python
 from toui import Website, Page
 ```
 Create a `Website` object:
@@ -76,27 +89,37 @@
 main_page = Page(html_file="path/to/html", url="/")
 app.add_pages(main_page)
 
 if __name__ == "__main__":
     app.run()
 ```
 
+# Start with a template
+To start with a basic template for a ToUI project. Run the command:
+```
+toui init
+```
+Alternatively, use this [template](https://github.com/mubarakalmehairbi/BasicToUIProject).
+
 # Make the app responsive
 Check this [example](https://toui.readthedocs.io/en/latest/Examples.example_1_simple_website.html)
 and [other examples](https://toui.readthedocs.io/en/latest/Examples.html) to learn how
 to make the website / desktop app responsive.
 
 # Deploy the app
 You can deploy the web app the same way you deploy a `Flask` app ([How to deploy Flask app](https://flask.palletsprojects.com/deploying/)).
 The only difference is that you need to access the `Flask` object first:
 ```python
 app = Website(__name__)
 flask_app = app.flask_app
 ```
 Then you need to deploy the `flask_app` and not the `app`.
 
+# How to contribute
+ToUI welcomes contribution, small or big. For anyone who wants to contribute please check the [contribution page](https://toui.readthedocs.io/en/latest/CONTRIBUTING.html).
+
 # License and Copyrights
 Copyrights (c) 2023 Mubarak Almehairbi.
 This package is licensed under the MIT license.
 
 # Documentation
 You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io).
```

### Comparing `toui-2.4.3b0/toui.egg-info/SOURCES.txt` & `toui-3.0.0b0/toui.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 examples/__init__.py
 examples/advanced_example_1_toui_blueprint.py
+examples/advanced_example_2_toui_with_javascript.py
+examples/advanced_example_3_toui_with_google_sign_in.py
+examples/advanced_example_4_toui_with_firebase.py
 examples/example_1_simple_website.py
 examples/example_2_simple_desktop_app.py
 examples/example_3_updating_page.py
 examples/example_4_function_with_arg.py
 examples/example_5_user_variables.py
 examples/example_6_quick_website.py
 examples/example_7_quick_desktop_app.py
+images/icon.png
 images/logo.png
 toui/__init__.py
+toui/_cmd.py
 toui/_defaults.py
 toui/_helpers.py
 toui/_javascript_templates.py
 toui/_signals.py
 toui/apps.py
 toui/elements.py
 toui/exceptions.py
 toui/pages.py
 toui/structure.py
 toui.egg-info/PKG-INFO
 toui.egg-info/SOURCES.txt
 toui.egg-info/dependency_links.txt
+toui.egg-info/entry_points.txt
 toui.egg-info/requires.txt
 toui.egg-info/top_level.txt
```

